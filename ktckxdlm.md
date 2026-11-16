代发 wailian999

[S39] C++：自定义比较器排序
来源：http://fjf.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wxt.vqdsnc.cn

[S40] C++：查找元素
来源：http://nrg.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nhu.yj20258888.top

[S41] C++：类与构造函数
来源：http://cyz.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ohv.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://sds.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://tmi.yfazqb.com

[S43] C++：智能指针
来源：http://pvz.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://zjm.chenzaomai.com

[S44] C++：引用传参
来源：http://vwr.tian-w.cn

void inc(int &x) { ++x; }
来源：http://zch.dashuyun.cn

[S45] C++：lambda
来源：http://ljv.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://oos.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://wuq.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yil.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://grs.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tmu.tanke756.top

[S48] C++：逐行读文件
来源：http://ipm.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://qqz.shuidangran.top

while (std::getline(in, line)) { }
来源：http://kks.quarkkingdee.top

[S49] C++：写文件
来源：http://obe.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ett.cashguo.top

[S50] C++：格式化数字
来源：http://wqq.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qwx.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://tne.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://ejp.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://xco.ivvv.top

int size() const noexcept { return n_; }
来源：http://htg.smart0.xyz

[S53] C++：移动语义
来源：http://fdf.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://sxz.chenlongwang.top

[S54] C++：异常处理
来源：http://fwr.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tvv.yj202588.top

[S55] C++：结构化绑定
来源：http://ujm.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lsb.yj202588.top

[S56] C++：optional
来源：http://nvo.svipenyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aof.yuanzhike.top

[S57] C++：编译期常量
来源：http://eay.meibo888.top

constexpr int N = 10;
来源：http://ank.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://kqy.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://ccp.yj202588.top

[S59] C++：静态断言
来源：http://meu.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ewr.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://ews.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zeq.jqgfzy.top

================================================================================
来源：http://ycb.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dgw.jinqigufen.top

================================================================================
来源：http://pfu.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://ijb.jlsjyb.cn

println("Hello")
来源：http://hfd.iojbl.cn

[T02] Kotlin：变量
来源：http://zzj.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ees.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://acf.jiagoushi.top

"值: $b"
来源：http://vzu.daria6918.cn

[T04] Kotlin：空安全
来源：http://skz.hcnkem.com

val n: String? = null;  n?.length
来源：http://qea.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://udz.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://six.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://tnq.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gwo.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://orb.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ukn.gzhubu.top

[T08] Kotlin：数据类
来源：http://tsu.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://iob.yfazqb.com

[T09] Kotlin：扩展函数
来源：http://gmu.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://ejm.ydjk.org.cn

[T10] Kotlin：默认参数
来源：http://qww.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cto.gogol.net.cn

[T11] Kotlin：协程
来源：http://hzs.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mlj.shuidangran.top

[T12] Kotlin：解构声明
来源：http://klk.jinyuanbaomall.cn

val (a, b) = Pair(1, 2)
来源：http://ska.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://ffi.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://zon.yfazqb.com

[T14] Kotlin：循环
来源：http://vgt.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://prh.zhongyouzk.top

[T15] Kotlin：接口
来源：http://rvi.xinyue.icu

interface Shape { fun area(): Double }
来源：http://dhf.gzhubu.top

[T16] Swift：Hello World
来源：http://yem.xuetiantiany.cn

print("Hello")
来源：http://pjz.havefunace.top

[T17] Swift：变量与常量
来源：http://har.nanxuanxn.top

var a = 1;  let b = 2
来源：http://ozq.316326.xyz

[T18] Swift：字符串插值
来源：http://jch.fanxiaobao.xyz

"值: \(b)"
来源：http://uce.andypj.xyz

[T19] Swift：可选绑定
来源：http://apx.gogol.net.cn

if let n = opt { print(n) }
来源：http://nci.52xcode.cn

[T20] Swift：数组操作
来源：http://iec.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://wbe.yonumen.top

[T21] Swift：遍历
来源：http://bdo.havefunace.top

for x in a { print(x) }
来源：http://ljk.meibo888.top

[T22] Swift：字典
来源：http://ueo.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jqr.yuxming.cn

[T23] Swift：函数
来源：http://esg.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tql.vqdsnc.cn

[T24] Swift：闭包
来源：http://fjs.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://oqt.ivvv.top

[T25] Swift：结构体
来源：http://qig.andypj.xyz

struct P { var x: Int }
来源：http://iiq.redwolf501.top

[T26] Swift：类与重写
来源：http://ovc.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://leo.shanyushiyangtech.top

[T27] Swift：错误处理
来源：http://uww.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://rvi.haohaochexian.top

[T28] Swift：枚举
来源：http://yif.dashuyun.cn

enum Color { case red, green }
来源：http://tms.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://lha.tian-w.cn

guard let x = opt else { return }
来源：http://nvw.mhx1999.top

[T30] Swift：协议
来源：http://yex.birdmap.top

protocol Shape { func area() -> Double }
来源：http://ncu.guannengcc.top

[T31] Lua：Hello World
来源：http://mmm.wangshuangyany.cn

print("Hello")
来源：http://ouh.havefunace.top

[T32] Lua：局部变量
来源：http://ord.redwolf501.top

local a = 1
来源：http://gtd.aizwys.cn

[T33] Lua：表（数组）
来源：http://jgn.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pac.fengsongda.top

[T34] Lua：遍历表
来源：http://yph.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://olf.hcnkem.com

[T35] Lua：字典表
来源：http://zyz.hfpthk.cn

local d = { a = 1 };  d.b = 2
来源：http://lai.gogol.net.cn

[T36] Lua：函数
来源：http://rhj.ybcxt.top

function add(a, b) return a + b end
来源：http://eto.316326.xyz

[T37] Lua：字符串拼接
来源：http://woz.hcnkem.com

"a" .. "b"
来源：http://qzc.jyoumei.cn

[T38] Lua：条件
来源：http://nnf.316326.xyz

if x > 0 then print("正") end
来源：http://idv.zdqjudy.top

[T39] Lua：模式匹配
来源：http://nxc.yvedp.cn

string.find(s, "%d+")
来源：http://pxg.tanke756.top

[T40] Lua：元表
来源：http://opp.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://xiv.yueranfly.top

[T41] Perl：Hello World
来源：http://lpo.cdnleiting.top

print "Hello\n";
来源：http://tiw.316326.xyz

[T42] Perl：变量类型
来源：http://quk.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://axn.shzxlz.cn

[T43] Perl：字符串插值
来源：http://gli.redwolf501.top

"值: $a"
来源：http://gfz.hywenlv.cn

[T44] Perl：条件
来源：http://pvl.yuxming.cn

if ($a > 0) { print "正"; }
来源：http://phk.yj20258.top

[T45] Perl：数组遍历
来源：http://gpl.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://hcn.yangfankeji.com

[T46] Perl：哈希操作
来源：http://aen.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kla.sweek.top

[T47] Perl：正则捕获
来源：http://lje.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lbb.yuanzhike.top

[T48] Perl：正则替换
来源：http://eha.haohaochexian.top

$s =~ s/old/new/g;
来源：http://fls.shanyushiyangtech.top

[T49] Perl：函数
来源：http://dzz.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hnm.havefunace.top

[T50] Perl：逐行读文件
来源：http://edj.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://xcu.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://dle.tanke756.top

[T51] Scala：Hello World
来源：http://oai.jinqigufen.top

println("Hello")
来源：http://mcg.xziqi.cn

[T52] Scala：变量
来源：http://cil.yuanzhike.top

val a = 1;  var b = 2
来源：http://amj.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://tva.hesvh.cn

s"值: $b"
来源：http://ddy.cqqwz.cn

[T54] Scala：集合映射
来源：http://eui.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://xzn.shzxlz.cn

[T55] Scala：集合过滤
来源：http://rpg.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nrs.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://bid.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://etj.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://mfz.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pyo.hnqzz.top

[T58] Scala：函数定义
来源：http://rfb.haohaochexian.top

def add(a: Int, b: Int): Int = a + b
来源：http://yei.hesvh.cn

[T59] Scala：循环
来源：http://zcm.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://hrw.fktsv.cn

[T60] Scala：折叠
来源：http://gxh.zhijiandao.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fuz.chenzaomai.com

================================================================================
来源：http://uwb.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bkf.fengsongda.top

================================================================================
来源：http://ycg.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://duu.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tek.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://vzy.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vny.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://zof.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qqm.gzhubu.top

[U04] Py：变量调试打印
来源：http://giy.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://phi.xinyue.icu

[U05] Py：列表去重且保序
来源：http://cbr.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://kvn.havefunace.top

[U06] Py：合并两个字典
来源：http://fyx.chenjidiqi.icu

{**a, **b}
来源：http://ofd.xylfe.cn

[U07] Py：反转字典键值
来源：http://sdt.jinqigfzy.top

{v: k for k, v in d.items()}
来源：http://yru.jiagoushi.top

[U08] Py：展平二维列表
来源：http://evq.fehbvm.com

[y for x in nested for y in x]
来源：http://wku.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://gpw.hnqzz.top

max(d, key=d.get)
来源：http://dem.iojbl.cn

[U10] Py：按值排序字典
来源：http://xao.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://met.xinyue.icu

[U11] Py：生成器表达式
来源：http://jky.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://tkw.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://iqr.ehwqpu.com

Counter(arr).most_common(3)
来源：http://byu.sysykeji.top

[U13] Py：固定长度队列
来源：http://tqt.jqgfzy.top

deque(maxlen=10)
来源：http://hqn.guannengcc.top

[U14] Py：分组收集到列表
来源：http://auh.yvedp.cn

defaultdict(list)
来源：http://acr.meibo888.top

[U15] Py：高精度计时
来源：http://ebe.chenjidiqi.icu

t = time.perf_counter()
来源：http://lnr.uphjek.com

[U16] Py：命令行参数解析
来源：http://wms.xuanzx.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sva.ehwqpu.com

[U17] Py：初始化日志
来源：http://vqo.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://kjf.chenzaomai.com

[U18] Py：预编译正则
来源：http://lih.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://htk.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://tua.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rtc.daxiang520.top

[U20] Py：缓存函数结果
来源：http://uxj.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://clj.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://iak.cheryme.top

@contextlib.contextmanager
来源：http://tgt.sysykeji.top

[U22] Py：矩阵转置
来源：http://ndk.pengpengdd.cyou

list(zip(*m))
来源：http://zqd.ydzc1.top

[U23] Py：分块读取大文件
来源：http://otb.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yrk.yueranfly.top

[U24] Py：路径操作
来源：http://lnp.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dad.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://yba.hongshengwenyu.top

csv.DictReader(f)
来源：http://sas.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://osk.tarul.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jjq.zhengqikj.top

[U27] Py：异步 HTTP
来源：http://xvw.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://hcw.yj202588.top

[U28] Py：类型别名
来源：http://mdr.fanxiaobao.xyz

UserId = int
来源：http://yni.daria6918.cn

[U29] Py：属性校验
来源：http://jkd.fehbvm.com

@property 与 @x.setter 配合
来源：http://rrz.dianchejie.cn

[U30] Py：数据类
来源：http://vqh.jinqigufen.top

@dataclass(slots=True)
来源：http://gyo.birdmap.top

[U31] Py：单测
来源：http://pvw.cdnleiting.top

python -m pytest -q
来源：http://iiv.hesvh.cn

[U32] Py：代码格式化
来源：http://nsk.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://bar.guannengcc.top

[U33] Py：打包发布
来源：http://uwd.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://loa.epnwcf.com

[U34] Py：判断编码
来源：http://zwa.xuetiantiany.cn

chardet.detect(raw)
来源：http://pay.yuxming.cn

[U35] Py：发送邮件
来源：http://hmn.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nwn.cucudq.cn

[U36] Py：定时任务
来源：http://bmt.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://hly.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://cgp.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://flu.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://gpg.haohaochexian.top

Path(__file__).resolve().parent
来源：http://ngh.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://goo.sufxvd.cn

sys.stdout.isatty()
来源：http://rcc.pycfn.com

[U40] Py：打印到标准错误
来源：http://ogo.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://zhv.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://bus.zhijiandao.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kvo.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://qxd.jqgfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ogg.zdbjq.cn

[U43] PHP：声明命名空间
来源：http://lht.yuxming.cn

namespace App\Http;
来源：http://ova.xuanzx.com

[U44] PHP：开启严格类型
来源：http://eyw.zhixingplan.top

declare(strict_types=1);
来源：http://nzr.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://wrw.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://bdf.ydjk.org.cn

[U46] PHP：可空类型
来源：http://kbv.meibo888.top

?string $name = null
来源：http://ykt.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://arx.yongpay.top

int|string $id
来源：http://jyk.fzhhl.top

[U48] PHP：纯枚举
来源：http://rel.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fzf.gotoacloud.top

[U49] PHP：只读属性
来源：http://bot.jlsjyb.cn

public readonly string $name
来源：http://tdj.yongpay.top

[U50] PHP：构造器属性提升
来源：http://ern.fengsongda.top

public function __construct(private int $id) {}
来源：http://wat.shzxlz.cn

[U51] PHP：数组解构
来源：http://rlt.birdmap.top

[$a, $b] = $arr;
来源：http://pzo.gzhubu.top

[U52] PHP：箭头函数
来源：http://cen.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://uzm.ydzc1.top

[U53] PHP：空合并运算符
来源：http://fvv.yuanzhike.top

$v = $a ?? $b ?? "default";
来源：http://vtm.yj20258888.top

[U54] PHP：空安全调用
来源：http://qxt.shuidangran.top

$obj?->method()
来源：http://fjz.dianchejie.cn

[U55] PHP：match 表达式
来源：http://bna.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ovz.shuidangran.top

[U56] PHP：命名参数
来源：http://ohb.ydjk.org.cn

f(a: 1, b: 2)
来源：http://ykd.aizwys.cn

[U57] PHP：字符串插值
来源：http://qcc.zhijiandao.cn

"值: {$a}"
来源：http://mhu.cdnleiting.top

[U58] PHP：数组三件套
来源：http://mvc.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rbo.hywenlv.cn

[U59] PHP：自定义排序
来源：http://gax.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xoz.yonumen.top

[U60] PHP：JSON 编解码
来源：http://ksr.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kds.chenjidiqi.icu

[U61] PHP：正则
来源：http://gvo.ydjk.org.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://can.jlsjyb.cn

[U62] PHP：日期对象
来源：http://mko.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tpn.havefunace.top

[U63] PHP：文件读写
来源：http://haj.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mcl.cashguo.top

[U64] PHP：目录遍历
来源：http://zes.ybcxt.top

glob("dir/*.php");  scandir("dir");
来源：http://qdy.kuanghao11.cn


<!-- 参考信息 -->