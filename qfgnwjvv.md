代发 wailian999

[S39] C++：自定义比较器排序
来源：http://sap.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xri.smart0.xyz

[S40] C++：查找元素
来源：http://aqd.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iby.zhengqikj.top

[S41] C++：类与构造函数
来源：http://juf.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vrs.guannengcc.top

[S42] C++：继承与虚函数
来源：http://cvn.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://ans.havefunace.top

[S43] C++：智能指针
来源：http://qdc.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://veo.yj20258.top

[S44] C++：引用传参
来源：http://ieg.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://oyf.yonumen.top

[S45] C++：lambda
来源：http://fnw.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://lho.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://knt.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vbm.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://bkr.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ibt.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://qtx.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://fro.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://mve.dashuyun.cn

[S49] C++：写文件
来源：http://nfv.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://djn.daria6918.cn

[S50] C++：格式化数字
来源：http://omh.nwbrower.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bde.snrcjt.cn

[S51] C++：显式类型转换
来源：http://rpa.sjlbkw.cn

static_cast<double>(a) / b
来源：http://swv.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://mus.bbcook.cn

int size() const noexcept { return n_; }
来源：http://pax.cheryme.top

[S53] C++：移动语义
来源：http://kmo.316326.xyz

std::vector<int> w = std::move(v);
来源：http://rtc.yfazqb.com

[S54] C++：异常处理
来源：http://hgb.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qio.zycfv.cn

[S55] C++：结构化绑定
来源：http://dgw.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wvv.jinqigufen.top

[S56] C++：optional
来源：http://zvg.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mhe.zdbjq.cn

[S57] C++：编译期常量
来源：http://rnm.yj202588.top

constexpr int N = 10;
来源：http://sga.gaohongyu789.top

[S58] C++：命名空间
来源：http://plu.jinyuanbaomall.cn

namespace ns { int f() { return 1; } }
来源：http://orn.vqdsnc.cn

[S59] C++：静态断言
来源：http://euu.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eyy.hammf.cn

[S60] C++：遍历并删除元素
来源：http://rmv.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uss.redwolf501.top

================================================================================
来源：http://jeg.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vfu.jianghu66.top

================================================================================
来源：http://gaa.gzhubu.top

[T01] Kotlin：Hello World
来源：http://xhh.hysaishi.cn

println("Hello")
来源：http://wkc.hnqzz.top

[T02] Kotlin：变量
来源：http://kuv.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cki.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://sln.wangshuangyany.cn

"值: $b"
来源：http://qhv.svipenyu.cn

[T04] Kotlin：空安全
来源：http://xup.zycfv.cn

val n: String? = null;  n?.length
来源：http://jiy.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://tbg.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uaw.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://ffn.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xzj.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://doh.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sqc.c1oappe.top

[T08] Kotlin：数据类
来源：http://tun.birdmap.top

data class User(val name: String, val age: Int)
来源：http://xdz.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://jek.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://qwl.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://lrq.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ymg.ehwqpu.com

[T11] Kotlin：协程
来源：http://mgv.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gab.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://edu.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://blo.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://pcm.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://gnx.hnqzz.top

[T14] Kotlin：循环
来源：http://mvh.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://wom.andypj.xyz

[T15] Kotlin：接口
来源：http://ays.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://ahd.vehdjk.com

[T16] Swift：Hello World
来源：http://ucw.cqqwz.cn

print("Hello")
来源：http://mto.yfazqb.com

[T17] Swift：变量与常量
来源：http://kxq.xylfe.cn

var a = 1;  let b = 2
来源：http://kyq.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://tlk.316326.xyz

"值: \(b)"
来源：http://kbu.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://eaw.xylfe.cn

if let n = opt { print(n) }
来源：http://gwz.tianlin.xyz

[T20] Swift：数组操作
来源：http://usl.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://okn.redwolf501.top

[T21] Swift：遍历
来源：http://bps.fehbvm.com

for x in a { print(x) }
来源：http://alt.zhiwuduotai.top

[T22] Swift：字典
来源：http://yru.wangshuangyany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mom.ivvv.top

[T23] Swift：函数
来源：http://sia.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mrc.xziqi.cn

[T24] Swift：闭包
来源：http://krf.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hou.c1oappe.top

[T25] Swift：结构体
来源：http://bwy.shuidangran.top

struct P { var x: Int }
来源：http://hmr.vqdsnc.cn

[T26] Swift：类与重写
来源：http://oem.wangshuangyany.cn

class A: Base { override func f() {} }
来源：http://qtp.jqgfzy.top

[T27] Swift：错误处理
来源：http://cjg.mhx1999.top

do { try f() } catch { print(error) }
来源：http://vth.hfpthk.cn

[T28] Swift：枚举
来源：http://hjo.fehbvm.com

enum Color { case red, green }
来源：http://bah.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://ryv.gzhubu.top

guard let x = opt else { return }
来源：http://zce.gotoacloud.top

[T30] Swift：协议
来源：http://pay.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://hrw.chenlongwang.top

[T31] Lua：Hello World
来源：http://xqj.316326.xyz

print("Hello")
来源：http://jiz.vehdjk.com

[T32] Lua：局部变量
来源：http://rmy.ywan-chungtsiang.top

local a = 1
来源：http://vns.0kj1m.cn

[T33] Lua：表（数组）
来源：http://apb.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wkw.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://lty.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zla.yonumen.top

[T35] Lua：字典表
来源：http://fin.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://qsp.snrcjt.cn

[T36] Lua：函数
来源：http://fir.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://jre.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://trz.shanyushiyangtech.top

"a" .. "b"
来源：http://olk.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://uty.tanke756.top

if x > 0 then print("正") end
来源：http://jtj.zhengqikj.top

[T39] Lua：模式匹配
来源：http://ggv.cdnleiting.top

string.find(s, "%d+")
来源：http://pgd.cucudq.cn

[T40] Lua：元表
来源：http://lks.hcnkem.com

setmetatable({}, { __index = base })
来源：http://nlq.cheryme.top

[T41] Perl：Hello World
来源：http://afv.fehbvm.com

print "Hello\n";
来源：http://tvs.jiagoushi.top

[T42] Perl：变量类型
来源：http://zur.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://flc.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://mhd.xylfe.cn

"值: $a"
来源：http://rlk.yongpay.top

[T44] Perl：条件
来源：http://ylw.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://oyg.yueranfly.top

[T45] Perl：数组遍历
来源：http://xsc.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://mvi.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://mwp.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uop.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://oyt.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mgd.fehbvm.com

[T48] Perl：正则替换
来源：http://kah.jiagoushi.top

$s =~ s/old/new/g;
来源：http://euf.52xcode.cn

[T49] Perl：函数
来源：http://rtt.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wzy.ybcxt.top

[T50] Perl：逐行读文件
来源：http://mzz.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jtu.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://hku.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://lib.nanxuanxn.top

println("Hello")
来源：http://xkl.316326.xyz

[T52] Scala：变量
来源：http://abp.zycfv.cn

val a = 1;  var b = 2
来源：http://xuy.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://ilx.tanke756.top

s"值: $b"
来源：http://qqh.meibo888.top

[T54] Scala：集合映射
来源：http://gvf.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://oxm.epnwcf.com

[T55] Scala：集合过滤
来源：http://heq.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wsa.fengsongda.top

[T56] Scala：样例类
来源：http://oee.bbcook.cn

case class User(name: String, age: Int)
来源：http://voo.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://kcx.gzhubu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://krg.hesvh.cn

[T58] Scala：函数定义
来源：http://vlo.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://avy.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://ofa.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://sgo.redwolf501.top

[T60] Scala：折叠
来源：http://rsh.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://whh.0kj1m.cn

================================================================================
来源：http://pxg.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ugl.xziqi.cn

================================================================================
来源：http://xlk.cheryme.top

[U01] Py：创建虚拟环境
来源：http://det.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://rpg.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://ypd.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cbk.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://jjv.yj202588.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dvr.yj20258888.top

[U04] Py：变量调试打印
来源：http://ygg.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ldx.yj20258888.top

[U05] Py：列表去重且保序
来源：http://jvb.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://xkl.yj202588.top

[U06] Py：合并两个字典
来源：http://rjq.cashguo.top

{**a, **b}
来源：http://qkj.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://sgp.yuanzhike.top

{v: k for k, v in d.items()}
来源：http://gpo.cashguo.top

[U08] Py：展平二维列表
来源：http://zqv.svipenyu.cn

[y for x in nested for y in x]
来源：http://xqv.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://jzm.quarkkingdee.top

max(d, key=d.get)
来源：http://bru.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://asd.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qzl.9152youxi.cn

[U11] Py：生成器表达式
来源：http://hbu.gotoacloud.top

(x * 2 for x in arr)
来源：http://loe.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://ynp.sufxvd.cn

Counter(arr).most_common(3)
来源：http://suz.sufxvd.cn

[U13] Py：固定长度队列
来源：http://tnp.svipenyu.cn

deque(maxlen=10)
来源：http://kpm.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://oxa.hammf.cn

defaultdict(list)
来源：http://qei.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://nlk.bbcook.cn

t = time.perf_counter()
来源：http://nkr.hesvh.cn

[U16] Py：命令行参数解析
来源：http://vvq.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hde.ivvv.top

[U17] Py：初始化日志
来源：http://fge.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://pff.smart0.xyz

[U18] Py：预编译正则
来源：http://zxv.andypj.xyz

pat = re.compile(r"\d+")
来源：http://jad.nwbrower.top

[U19] Py：正则替换带回调
来源：http://ibj.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dfg.daria6918.cn

[U20] Py：缓存函数结果
来源：http://tie.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://hya.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://jqa.haohaochexian.top

@contextlib.contextmanager
来源：http://wns.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://bqo.c1oappe.top

list(zip(*m))
来源：http://jwo.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://kzp.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gle.yuanzhike.top

[U24] Py：路径操作
来源：http://euj.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jcf.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://yvt.c1oappe.top

csv.DictReader(f)
来源：http://tjj.quarkkingdee.top

[U26] Py：并发下载
来源：http://ouq.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ill.shanyushiyangtech.top

[U27] Py：异步 HTTP
来源：http://jwt.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://xso.zdqjudy.top

[U28] Py：类型别名
来源：http://dhl.feifeiyinyue.top

UserId = int
来源：http://cns.yanxiufei.cn

[U29] Py：属性校验
来源：http://exn.chenzaomai.com

@property 与 @x.setter 配合
来源：http://uwf.xuanzx.com

[U30] Py：数据类
来源：http://iep.dianchejie.cn

@dataclass(slots=True)
来源：http://hbv.nanxuanxn.top

[U31] Py：单测
来源：http://xtb.dashuyun.cn

python -m pytest -q
来源：http://okx.jinqigfzy.top

[U32] Py：代码格式化
来源：http://lse.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://weo.jqgufenzy.top

[U33] Py：打包发布
来源：http://pwq.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://cjp.vqdsnc.cn

[U34] Py：判断编码
来源：http://qtn.mhx1999.top

chardet.detect(raw)
来源：http://qsg.yanxiufei.cn

[U35] Py：发送邮件
来源：http://ovx.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kpp.chenlongwang.top

[U36] Py：定时任务
来源：http://vcz.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://fvt.aizwys.cn

[U37] Py：读写 Excel
来源：http://ckf.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ahq.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://zqi.hammf.cn

Path(__file__).resolve().parent
来源：http://unq.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://gah.uphjek.com

sys.stdout.isatty()
来源：http://grv.andypj.xyz

[U40] Py：打印到标准错误
来源：http://idk.kuanghao11.cn

print("err", file=sys.stderr)
来源：http://ihm.jqgfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://ldz.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mjq.ctjpmb.com

[U42] PHP：PSR-4 自动加载
来源：http://gel.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ava.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://hrq.jianghu66.top

namespace App\Http;
来源：http://xku.cashguo.top

[U44] PHP：开启严格类型
来源：http://cmi.cashguo.top

declare(strict_types=1);
来源：http://kej.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://ryf.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kuu.zdbjq.cn

[U46] PHP：可空类型
来源：http://uzd.fzhhl.top

?string $name = null
来源：http://ysh.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://nvc.birdmap.top

int|string $id
来源：http://lua.zhixingplan.top

[U48] PHP：纯枚举
来源：http://ctp.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://htf.meibo888.top

[U49] PHP：只读属性
来源：http://shg.dianchejie.cn

public readonly string $name
来源：http://bei.hammf.cn

[U50] PHP：构造器属性提升
来源：http://mxf.fengsongda.top

public function __construct(private int $id) {}
来源：http://dym.hesvh.cn

[U51] PHP：数组解构
来源：http://mxq.guannengcc.top

[$a, $b] = $arr;
来源：http://dor.bbcook.cn

[U52] PHP：箭头函数
来源：http://foq.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://wwx.hnqzz.top

[U53] PHP：空合并运算符
来源：http://myu.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://lag.ivvv.top

[U54] PHP：空安全调用
来源：http://cvv.ybcxt.top

$obj?->method()
来源：http://rdu.chenlongwang.top

[U55] PHP：match 表达式
来源：http://tgq.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tza.hammf.cn

[U56] PHP：命名参数
来源：http://ujf.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://yfi.vqdsnc.cn

[U57] PHP：字符串插值
来源：http://jzn.sysykeji.top

"值: {$a}"
来源：http://lyj.zhongyouzk.top

[U58] PHP：数组三件套
来源：http://ody.sufxvd.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nok.zhixingplan.top

[U59] PHP：自定义排序
来源：http://xuc.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iax.aibaodan.cn

[U60] PHP：JSON 编解码
来源：http://lvu.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dtw.smart0.xyz

[U61] PHP：正则
来源：http://bbr.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vfy.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://tpe.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ija.chenlongwang.top

[U63] PHP：文件读写
来源：http://sjy.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://how.jyoumei.cn

[U64] PHP：目录遍历
来源：http://hbe.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://sdu.quarkkingdee.top


<!-- 参考信息 -->