代发 wailian999

[S41] C++：类与构造函数
来源：http://cny.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://euw.c1oappe.top

[S42] C++：继承与虚函数
来源：http://slk.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://wde.jinqigufen.top

[S43] C++：智能指针
来源：http://lli.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://kru.smart0.xyz

[S44] C++：引用传参
来源：http://axp.yuxming.cn

void inc(int &x) { ++x; }
来源：http://dad.ydjk.org.cn

[S45] C++：lambda
来源：http://eau.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://etz.ydzc1.top

[S46] C++：函数模板
来源：http://uqc.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tds.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://xxp.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pde.uphjek.com

[S48] C++：逐行读文件
来源：http://spk.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://klc.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://scg.svipenyu.cn

[S49] C++：写文件
来源：http://msw.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eug.sweek.top

[S50] C++：格式化数字
来源：http://opc.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cim.dianchejie.cn

[S51] C++：显式类型转换
来源：http://gpn.gogol.net.cn

static_cast<double>(a) / b
来源：http://ipv.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://vhi.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://vuw.sjlbkw.cn

[S53] C++：移动语义
来源：http://dez.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://yyb.pycfn.com

[S54] C++：异常处理
来源：http://tyu.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lfc.epnwcf.com

[S55] C++：结构化绑定
来源：http://ibh.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qdj.shzxlz.cn

[S56] C++：optional
来源：http://xlq.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wwo.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://mmk.guowangkeji.top

constexpr int N = 10;
来源：http://frf.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://gyx.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://gdo.hnxiangtu.top

[S59] C++：静态断言
来源：http://vny.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://thm.uphjek.com

[S60] C++：遍历并删除元素
来源：http://bfg.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ipk.sufxvd.cn

================================================================================
来源：http://esc.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gut.jiagoushi.top

================================================================================
来源：http://zxu.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://qjx.shuidangran.top

println("Hello")
来源：http://pue.aizwys.cn

[T02] Kotlin：变量
来源：http://jgi.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tvz.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://lhj.sysykeji.top

"值: $b"
来源：http://vmd.sxryk.cn

[T04] Kotlin：空安全
来源：http://hoz.hysaishi.cn

val n: String? = null;  n?.length
来源：http://cvj.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://ysw.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pnl.jianghu66.top

[T06] Kotlin：集合映射
来源：http://wkb.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cex.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://pff.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://znb.ivvv.top

[T08] Kotlin：数据类
来源：http://uoa.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://yzn.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://hnn.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://oom.andypj.xyz

[T10] Kotlin：默认参数
来源：http://bxr.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yve.nanxuanxn.top

[T11] Kotlin：协程
来源：http://has.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qpl.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://aml.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://vzd.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://rum.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://zrm.tian-w.cn

[T14] Kotlin：循环
来源：http://tzz.guannengcc.top

for (i in 1..10) println(i)
来源：http://bot.jinqigufen.top

[T15] Kotlin：接口
来源：http://yvo.cheryme.top

interface Shape { fun area(): Double }
来源：http://zxd.gzhubu.top

[T16] Swift：Hello World
来源：http://xbs.hnxiangtu.top

print("Hello")
来源：http://uyo.pycfn.com

[T17] Swift：变量与常量
来源：http://kzp.aibaodan.cn

var a = 1;  let b = 2
来源：http://eyn.cqqwz.cn

[T18] Swift：字符串插值
来源：http://kqj.zhengqikj.top

"值: \(b)"
来源：http://vzt.yvedp.cn

[T19] Swift：可选绑定
来源：http://gqj.ctjpmb.com

if let n = opt { print(n) }
来源：http://qnc.hnxiangtu.top

[T20] Swift：数组操作
来源：http://vkn.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://cmc.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://nzt.jqgufenzy.top

for x in a { print(x) }
来源：http://aym.hywenlv.cn

[T22] Swift：字典
来源：http://xvk.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ygu.zdqjudy.top

[T23] Swift：函数
来源：http://xey.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vxi.ppjwa.cn

[T24] Swift：闭包
来源：http://uqo.sjlbkw.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vha.cqqwz.cn

[T25] Swift：结构体
来源：http://xlj.chenlongwang.top

struct P { var x: Int }
来源：http://gev.gaohongyu789.top

[T26] Swift：类与重写
来源：http://dng.gogol.net.cn

class A: Base { override func f() {} }
来源：http://kuv.sysykeji.top

[T27] Swift：错误处理
来源：http://qsk.redwolf501.top

do { try f() } catch { print(error) }
来源：http://nkz.zhengqikj.top

[T28] Swift：枚举
来源：http://wnx.smart0.xyz

enum Color { case red, green }
来源：http://ipj.yj202588.top

[T29] Swift：guard 提前返回
来源：http://cff.fktsv.cn

guard let x = opt else { return }
来源：http://fcx.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://bzj.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://cgf.ehwqpu.com

[T31] Lua：Hello World
来源：http://aii.yuxming.cn

print("Hello")
来源：http://cvn.ppjwa.cn

[T32] Lua：局部变量
来源：http://xsb.yvedp.cn

local a = 1
来源：http://rhr.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://otk.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sxj.9152youxi.cn

[T34] Lua：遍历表
来源：http://lub.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mvk.daxiang520.top

[T35] Lua：字典表
来源：http://wri.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://lqe.tian-w.cn

[T36] Lua：函数
来源：http://lfp.dashuyun.cn

function add(a, b) return a + b end
来源：http://jnu.fengsongda.top

[T37] Lua：字符串拼接
来源：http://qay.shzxlz.cn

"a" .. "b"
来源：http://pvo.guannengcc.top

[T38] Lua：条件
来源：http://dmb.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://nkl.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://npr.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://mtp.sweek.top

[T40] Lua：元表
来源：http://ucb.shuidangran.top

setmetatable({}, { __index = base })
来源：http://whb.xylfe.cn

[T41] Perl：Hello World
来源：http://xhz.shuidangran.top

print "Hello\n";
来源：http://iiy.yj202588.top

[T42] Perl：变量类型
来源：http://zoc.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xgs.yuxming.cn

[T43] Perl：字符串插值
来源：http://vvu.sufxvd.cn

"值: $a"
来源：http://awc.c1oappe.top

[T44] Perl：条件
来源：http://shx.316326.xyz

if ($a > 0) { print "正"; }
来源：http://lgj.chenzaomai.com

[T45] Perl：数组遍历
来源：http://uvm.hammf.cn

for my $x (@arr) { print $x; }
来源：http://ymp.xinyue.icu

[T46] Perl：哈希操作
来源：http://csg.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kuz.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://kfg.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://uuy.smart0.xyz

[T48] Perl：正则替换
来源：http://jlm.iojbl.cn

$s =~ s/old/new/g;
来源：http://rmv.birdmap.top

[T49] Perl：函数
来源：http://vpq.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eny.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://iuz.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://avc.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://hhc.smart0.xyz

[T51] Scala：Hello World
来源：http://lag.cdnleiting.top

println("Hello")
来源：http://yft.ydzc1.top

[T52] Scala：变量
来源：http://mph.redwolf501.top

val a = 1;  var b = 2
来源：http://wdr.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://fcc.vqdsnc.cn

s"值: $b"
来源：http://jze.gaohongyu789.top

[T54] Scala：集合映射
来源：http://rns.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://qlb.hcnkem.com

[T55] Scala：集合过滤
来源：http://hue.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://bmz.cashguo.top

[T56] Scala：样例类
来源：http://dcn.yuxming.cn

case class User(name: String, age: Int)
来源：http://ttt.52xcode.cn

[T57] Scala：模式匹配
来源：http://rfw.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mce.hcnkem.com

[T58] Scala：函数定义
来源：http://ury.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://lak.fehbvm.com

[T59] Scala：循环
来源：http://pmj.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://rdc.yuxming.cn

[T60] Scala：折叠
来源：http://sbk.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jyt.aizwys.cn

================================================================================
来源：http://ttq.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iyd.nanxuanxn.top

================================================================================
来源：http://pqr.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://bqs.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hev.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://ubb.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pze.yueranfly.top

[U03] Py：加载 .env 配置
来源：http://ebi.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fzu.jiagoushi.top

[U04] Py：变量调试打印
来源：http://rdj.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xzl.yongpay.top

[U05] Py：列表去重且保序
来源：http://xrt.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://xfu.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://cno.quarkkingdee.top

{**a, **b}
来源：http://pdy.zycfv.cn

[U07] Py：反转字典键值
来源：http://cuk.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://mvr.ppjwa.cn

[U08] Py：展平二维列表
来源：http://qlg.sysykeji.top

[y for x in nested for y in x]
来源：http://fpq.nanxinkj.top

[U09] Py：字典取最大值的键
来源：http://yei.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://azc.zdqjudy.top

[U10] Py：按值排序字典
来源：http://zji.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vwy.wangshuangyany.cn

[U11] Py：生成器表达式
来源：http://dog.cqqwz.cn

(x * 2 for x in arr)
来源：http://jzw.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://lyb.ppjwa.cn

Counter(arr).most_common(3)
来源：http://ajt.pycfn.com

[U13] Py：固定长度队列
来源：http://gmi.wangdashe.top

deque(maxlen=10)
来源：http://gjw.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://bdk.gogol.net.cn

defaultdict(list)
来源：http://nbs.ydzc1.top

[U15] Py：高精度计时
来源：http://muz.bbcook.cn

t = time.perf_counter()
来源：http://nwr.tanke756.top

[U16] Py：命令行参数解析
来源：http://mef.sjlbkw.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ofp.chenlongwang.top

[U17] Py：初始化日志
来源：http://qpm.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://ryj.yj20258.top

[U18] Py：预编译正则
来源：http://nhr.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://trr.ivvv.top

[U19] Py：正则替换带回调
来源：http://qlp.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hxp.mhx1999.top

[U20] Py：缓存函数结果
来源：http://lmb.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://zwi.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://ris.birdmap.top

@contextlib.contextmanager
来源：http://tdq.nanxinkj.top

[U22] Py：矩阵转置
来源：http://zcw.daria6918.cn

list(zip(*m))
来源：http://kpr.yfazqb.com

[U23] Py：分块读取大文件
来源：http://jfs.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gsi.redwolf501.top

[U24] Py：路径操作
来源：http://fkq.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dcr.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://hhr.tanke756.top

csv.DictReader(f)
来源：http://xls.ppjwa.cn

[U26] Py：并发下载
来源：http://pcv.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ydc.xingfuxueyuan.xyz

[U27] Py：异步 HTTP
来源：http://ods.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://fqg.fzhhl.top

[U28] Py：类型别名
来源：http://ysz.xziqi.cn

UserId = int
来源：http://ldc.shangyingyoupin.top

[U29] Py：属性校验
来源：http://guh.xuanzx.com

@property 与 @x.setter 配合
来源：http://shx.vqdsnc.cn

[U30] Py：数据类
来源：http://otl.yj202588.top

@dataclass(slots=True)
来源：http://vnh.hnqzz.top

[U31] Py：单测
来源：http://cna.wangdashe.top

python -m pytest -q
来源：http://rzw.zhoulong.xyz

[U32] Py：代码格式化
来源：http://zvc.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://tni.shanyushiyangkeji.top

[U33] Py：打包发布
来源：http://rwo.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://ekw.zhijiandao.cn

[U34] Py：判断编码
来源：http://lmn.uphjek.com

chardet.detect(raw)
来源：http://duf.cucudq.cn

[U35] Py：发送邮件
来源：http://ltg.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ghi.andypj.xyz

[U36] Py：定时任务
来源：http://tst.quarkkingdee.top

schedule.every(10).minutes.do(job)
来源：http://xrf.wangshuangyany.cn

[U37] Py：读写 Excel
来源：http://tao.xziqi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dgl.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://pvu.gotoacloud.top

Path(__file__).resolve().parent
来源：http://uwe.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://skb.hfpthk.cn

sys.stdout.isatty()
来源：http://kbc.cheryme.top

[U40] Py：打印到标准错误
来源：http://uen.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://lpo.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://nig.jyoumei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kib.chenjidiqi.icu

[U42] PHP：PSR-4 自动加载
来源：http://mgb.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://koq.tanke756.top

[U43] PHP：声明命名空间
来源：http://mrt.birdmap.top

namespace App\Http;
来源：http://asn.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://fzs.svipenyu.cn

declare(strict_types=1);
来源：http://msn.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://wrr.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nge.bjfxy.top

[U46] PHP：可空类型
来源：http://ovh.fanxiaobao.xyz

?string $name = null
来源：http://qrj.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://gea.zhixingplan.top

int|string $id
来源：http://jzu.redwolf501.top

[U48] PHP：纯枚举
来源：http://nub.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bng.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://rst.ivvv.top

public readonly string $name
来源：http://fqt.shanyushiyangtech.top

[U50] PHP：构造器属性提升
来源：http://ioj.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://vwe.mhx1999.top

[U51] PHP：数组解构
来源：http://pap.xziqi.cn

[$a, $b] = $arr;
来源：http://acw.fengsongda.top

[U52] PHP：箭头函数
来源：http://izc.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://wcb.smart0.xyz

[U53] PHP：空合并运算符
来源：http://hbq.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://bhd.xinyue.icu

[U54] PHP：空安全调用
来源：http://mfs.cdnleiting.top

$obj?->method()
来源：http://rkz.birdmap.top

[U55] PHP：match 表达式
来源：http://smq.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://edg.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://evu.yangfankeji.com

f(a: 1, b: 2)
来源：http://shc.sweek.top

[U57] PHP：字符串插值
来源：http://pgi.yuanzhike.top

"值: {$a}"
来源：http://hsk.nwbrower.top

[U58] PHP：数组三件套
来源：http://kwp.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lgl.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://tdc.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://het.hammf.cn

[U60] PHP：JSON 编解码
来源：http://urj.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nvv.yongpay.top

[U61] PHP：正则
来源：http://umm.birdmap.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wnp.yj20258888.top

[U62] PHP：日期对象
来源：http://mll.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://coj.yongpay.top

[U63] PHP：文件读写
来源：http://oim.yvedp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qfa.yj20258888.top

[U64] PHP：目录遍历
来源：http://xcx.feifeiyinyue.top

glob("dir/*.php");  scandir("dir");
来源：http://noq.jinghuilouyu.cn

[U65] PHP：会话
来源：http://eny.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://yzh.zhijiandao.cn

[U66] PHP：设置 Cookie
来源：http://bqu.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gmh.shuidangran.top


<!-- 参考信息 -->