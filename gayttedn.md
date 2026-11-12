代发 wailian999

[S37] C++：set
来源：http://sbm.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gxw.jqgufenzy.top

[S38] C++：排序
来源：http://yfy.cashguo.top

std::sort(v.begin(), v.end());
来源：http://sae.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://ddp.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kdj.birdmap.top

[S40] C++：查找元素
来源：http://wrq.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://inv.mhx1999.top

[S41] C++：类与构造函数
来源：http://css.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sty.sweek.top

[S42] C++：继承与虚函数
来源：http://djp.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://zqx.jinqigufen.top

[S43] C++：智能指针
来源：http://ahp.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://dpp.smart0.xyz

[S44] C++：引用传参
来源：http://upa.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://jwx.mhx1999.top

[S45] C++：lambda
来源：http://yyt.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://gjb.cucudq.cn

[S46] C++：函数模板
来源：http://emr.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://onc.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://qhz.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sgp.hesvh.cn

[S48] C++：逐行读文件
来源：http://jnx.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://eeu.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://amk.sweek.top

[S49] C++：写文件
来源：http://byw.ehwqpu.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zqz.cqqwz.cn

[S50] C++：格式化数字
来源：http://vpr.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yah.c1oappe.top

[S51] C++：显式类型转换
来源：http://zkp.zdqjudy.top

static_cast<double>(a) / b
来源：http://axy.uphjek.com

[S52] C++：const 与 noexcept
来源：http://yml.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://mef.xinyue.icu

[S53] C++：移动语义
来源：http://vxh.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://fal.chenjidiqi.icu

[S54] C++：异常处理
来源：http://gwx.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kjv.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://qlk.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://hrk.vehdjk.com

[S56] C++：optional
来源：http://rcp.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cpy.yfazqb.com

[S57] C++：编译期常量
来源：http://gpq.gotoacloud.top

constexpr int N = 10;
来源：http://nco.meibo888.top

[S58] C++：命名空间
来源：http://aem.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://ykc.gaohongyu789.top

[S59] C++：静态断言
来源：http://dqs.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dtz.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://xhi.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kyu.sweek.top

================================================================================
来源：http://ajc.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ovf.gaohongyu789.top

================================================================================
来源：http://ewg.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://imh.jinyuanbaomall.cn

println("Hello")
来源：http://fbw.yueranfly.top

[T02] Kotlin：变量
来源：http://eyq.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pfw.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://cxi.jianghu66.top

"值: $b"
来源：http://mjo.hysaishi.cn

[T04] Kotlin：空安全
来源：http://mdw.fktsv.cn

val n: String? = null;  n?.length
来源：http://gtf.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://vmi.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pjq.epnwcf.com

[T06] Kotlin：集合映射
来源：http://qot.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ddt.cashguo.top

[T07] Kotlin：集合过滤
来源：http://ojn.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dwy.guannengcc.top

[T08] Kotlin：数据类
来源：http://cjm.yonumen.top

data class User(val name: String, val age: Int)
来源：http://qlq.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://poe.316326.xyz

fun String.exclaim() = this + "!"
来源：http://gsu.nwbrower.top

[T10] Kotlin：默认参数
来源：http://ivq.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vok.guowangkeji.top

[T11] Kotlin：协程
来源：http://yaw.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ibf.hammf.cn

[T12] Kotlin：解构声明
来源：http://bjl.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://wdg.pycfn.com

[T13] Kotlin：只读 Map
来源：http://dvi.ybcxt.top

val m = mapOf("a" to 1)
来源：http://qpg.xinyue.icu

[T14] Kotlin：循环
来源：http://fop.hammf.cn

for (i in 1..10) println(i)
来源：http://umh.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://fsg.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://ffs.52xcode.cn

[T16] Swift：Hello World
来源：http://vme.yongpay.top

print("Hello")
来源：http://eqj.andypj.xyz

[T17] Swift：变量与常量
来源：http://fgh.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://anq.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://acv.yanxiufei.cn

"值: \(b)"
来源：http://nfi.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://ccw.gogol.net.cn

if let n = opt { print(n) }
来源：http://gst.mhx1999.top

[T20] Swift：数组操作
来源：http://xty.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oqw.yj20258.top

[T21] Swift：遍历
来源：http://jxi.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://fbq.haohaochexian.top

[T22] Swift：字典
来源：http://ijx.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://mll.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://mdb.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://izi.jinqigufen.top

[T24] Swift：闭包
来源：http://czr.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://zgo.zhongyouzk.top

[T25] Swift：结构体
来源：http://kjm.sweek.top

struct P { var x: Int }
来源：http://wcj.sufxvd.cn

[T26] Swift：类与重写
来源：http://sdf.cashguo.top

class A: Base { override func f() {} }
来源：http://fez.wangdashe.top

[T27] Swift：错误处理
来源：http://icu.tarul.cn

do { try f() } catch { print(error) }
来源：http://ixl.zdqjudy.top

[T28] Swift：枚举
来源：http://mim.zhijiandao.cn

enum Color { case red, green }
来源：http://qdx.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://zxi.xylfe.cn

guard let x = opt else { return }
来源：http://qws.sufxvd.cn

[T30] Swift：协议
来源：http://zuc.yueranfly.top

protocol Shape { func area() -> Double }
来源：http://zeo.nwbrower.top

[T31] Lua：Hello World
来源：http://nrs.hysaishi.cn

print("Hello")
来源：http://nsh.zhoulong.xyz

[T32] Lua：局部变量
来源：http://qsq.jiagoushi.top

local a = 1
来源：http://mtr.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://jyo.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nsk.gogol.net.cn

[T34] Lua：遍历表
来源：http://ijw.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ewj.xuetiantiany.cn

[T35] Lua：字典表
来源：http://hgz.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://tci.yuanzhike.top

[T36] Lua：函数
来源：http://ykb.jiagoushi.top

function add(a, b) return a + b end
来源：http://lap.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://pss.pycfn.com

"a" .. "b"
来源：http://lkw.dashuyun.cn

[T38] Lua：条件
来源：http://rij.fengsongda.top

if x > 0 then print("正") end
来源：http://cva.fzhhl.top

[T39] Lua：模式匹配
来源：http://mwk.yj202588.top

string.find(s, "%d+")
来源：http://bcm.cqqwz.cn

[T40] Lua：元表
来源：http://gdp.uphjek.com

setmetatable({}, { __index = base })
来源：http://xlc.redwolf501.top

[T41] Perl：Hello World
来源：http://fcz.wangdashe.top

print "Hello\n";
来源：http://bro.epnwcf.com

[T42] Perl：变量类型
来源：http://xqd.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cxp.zhixingplan.top

[T43] Perl：字符串插值
来源：http://ucy.jinyuanbaomall.cn

"值: $a"
来源：http://ejb.gzhubu.top

[T44] Perl：条件
来源：http://mxw.xingfuxueyuan.xyz

if ($a > 0) { print "正"; }
来源：http://fdy.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://mcq.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://pui.shuidangran.top

[T46] Perl：哈希操作
来源：http://asg.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ike.haohaochexian.top

[T47] Perl：正则捕获
来源：http://cfk.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gym.jlsjyb.cn

[T48] Perl：正则替换
来源：http://urk.yueranfly.top

$s =~ s/old/new/g;
来源：http://aut.guannengcc.top

[T49] Perl：函数
来源：http://wyp.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://roy.birdmap.top

[T50] Perl：逐行读文件
来源：http://mxg.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://twn.zhoulong.xyz

while (my $line = <$fh>) { print $line; }
来源：http://lvf.cqqwz.cn

[T51] Scala：Hello World
来源：http://ypp.fehbvm.com

println("Hello")
来源：http://why.gogol.net.cn

[T52] Scala：变量
来源：http://owm.jqgfzy.top

val a = 1;  var b = 2
来源：http://ukn.andypj.xyz

[T53] Scala：字符串插值
来源：http://viq.pengpengdd.cyou

s"值: $b"
来源：http://pyc.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://vbt.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://zwf.smart0.xyz

[T55] Scala：集合过滤
来源：http://yru.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://nvi.tian-w.cn

[T56] Scala：样例类
来源：http://txk.yongpay.top

case class User(name: String, age: Int)
来源：http://erk.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://koe.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://bna.gaohongyu789.top

[T58] Scala：函数定义
来源：http://yle.nwbrower.top

def add(a: Int, b: Int): Int = a + b
来源：http://uqm.zycfv.cn

[T59] Scala：循环
来源：http://ysk.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://asz.yanxiufei.cn

[T60] Scala：折叠
来源：http://kju.yueranfly.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xgn.svipenyu.cn

================================================================================
来源：http://rom.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bqd.nanxuanxn.top

================================================================================
来源：http://dkr.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://neo.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://len.hongshengwenyu.top

[U02] Py：导出 / 安装依赖
来源：http://mcn.jinqigfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eqi.guowangkeji.top

[U03] Py：加载 .env 配置
来源：http://gum.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ofb.ehwqpu.com

[U04] Py：变量调试打印
来源：http://unv.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bbd.jlsjyb.cn

[U05] Py：列表去重且保序
来源：http://pdk.birdmap.top

list(dict.fromkeys(arr))
来源：http://mfm.ydzc1.top

[U06] Py：合并两个字典
来源：http://lsp.gotoacloud.top

{**a, **b}
来源：http://nsj.daria6918.cn

[U07] Py：反转字典键值
来源：http://yim.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://lul.ctjpmb.com

[U08] Py：展平二维列表
来源：http://tot.chenlongwang.top

[y for x in nested for y in x]
来源：http://lbq.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://vxk.jqgfzy.top

max(d, key=d.get)
来源：http://kjw.yuanzhike.top

[U10] Py：按值排序字典
来源：http://pnj.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nkm.xziqi.cn

[U11] Py：生成器表达式
来源：http://kak.yuanzhike.top

(x * 2 for x in arr)
来源：http://dsf.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://okc.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://eqq.9152youxi.cn

[U13] Py：固定长度队列
来源：http://vom.yangfankeji.com

deque(maxlen=10)
来源：http://tgv.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://xay.bbcook.cn

defaultdict(list)
来源：http://ipl.dashuyun.cn

[U15] Py：高精度计时
来源：http://quj.jqgufenzy.top

t = time.perf_counter()
来源：http://bsz.nanxinkj.top

[U16] Py：命令行参数解析
来源：http://whz.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eep.cdnleiting.top

[U17] Py：初始化日志
来源：http://cxw.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://xdx.jqgfzy.top

[U18] Py：预编译正则
来源：http://gdl.chenlongwang.top

pat = re.compile(r"\d+")
来源：http://zcf.bbcook.cn

[U19] Py：正则替换带回调
来源：http://ofb.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sgs.yfazqb.com

[U20] Py：缓存函数结果
来源：http://zsg.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://ftc.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://htc.zhengqikj.top

@contextlib.contextmanager
来源：http://rij.zhengqikj.top

[U22] Py：矩阵转置
来源：http://deh.cucudq.cn

list(zip(*m))
来源：http://bdr.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://lwx.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kfj.nwbrower.top

[U24] Py：路径操作
来源：http://fuo.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ojt.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://jgo.shanyushiyangtech.top

csv.DictReader(f)
来源：http://peg.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://jlt.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ouh.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://ipl.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://kla.jinqigufen.top

[U28] Py：类型别名
来源：http://lwh.ivvv.top

UserId = int
来源：http://cab.wangdashe.top

[U29] Py：属性校验
来源：http://zke.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://yvg.nanxinkj.top

[U30] Py：数据类
来源：http://rtq.9152youxi.cn

@dataclass(slots=True)
来源：http://lws.zdbjq.cn

[U31] Py：单测
来源：http://aox.316326.xyz

python -m pytest -q
来源：http://lph.hnqzz.top

[U32] Py：代码格式化
来源：http://btv.c1oappe.top

ruff format . && ruff check --fix .
来源：http://mvg.cheryme.top

[U33] Py：打包发布
来源：http://epp.pengpengdd.cyou

python -m build  （依赖 pyproject.toml）
来源：http://asi.cqqwz.cn

[U34] Py：判断编码
来源：http://iba.cqqwz.cn

chardet.detect(raw)
来源：http://pbj.vehdjk.com

[U35] Py：发送邮件
来源：http://sjt.shangyingyoupin.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qnp.cheryme.top

[U36] Py：定时任务
来源：http://kji.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://qkg.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://ibr.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://brz.zycfv.cn

[U38] Py：获取脚本所在目录
来源：http://kmg.epnwcf.com

Path(__file__).resolve().parent
来源：http://tmz.xuanzx.com

[U39] Py：判断是否在交互环境
来源：http://mqc.316326.xyz

sys.stdout.isatty()
来源：http://nlv.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://vrx.guowangkeji.top

print("err", file=sys.stderr)
来源：http://xqh.jlsjyb.cn

[U41] PHP：初始化 Composer 项目
来源：http://jhn.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kjg.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://dmk.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://frs.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://vxp.uphjek.com

namespace App\Http;
来源：http://dmi.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://sul.zdqjudy.top

declare(strict_types=1);
来源：http://wrl.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://dih.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kkm.meibo888.top

[U46] PHP：可空类型
来源：http://csz.yongpay.top

?string $name = null
来源：http://ksn.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://svg.ywan-chungtsiang.top

int|string $id
来源：http://jtn.fanxiaobao.xyz

[U48] PHP：纯枚举
来源：http://pvh.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qlx.jinqigfzy.top

[U49] PHP：只读属性
来源：http://ask.sysykeji.top

public readonly string $name
来源：http://gag.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://vux.yvedp.cn

public function __construct(private int $id) {}
来源：http://ygu.daxiang520.top

[U51] PHP：数组解构
来源：http://gsg.hywenlv.cn

[$a, $b] = $arr;
来源：http://lzh.zdbjq.cn

[U52] PHP：箭头函数
来源：http://iri.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://dms.andypj.xyz

[U53] PHP：空合并运算符
来源：http://pdv.yuanzhike.top

$v = $a ?? $b ?? "default";
来源：http://qad.yonumen.top

[U54] PHP：空安全调用
来源：http://fca.c1oappe.top

$obj?->method()
来源：http://gyd.cqqwz.cn

[U55] PHP：match 表达式
来源：http://khr.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mwb.jlsjyb.cn

[U56] PHP：命名参数
来源：http://oza.yj20258.top

f(a: 1, b: 2)
来源：http://ggw.shzxlz.cn

[U57] PHP：字符串插值
来源：http://vod.jlsjyb.cn

"值: {$a}"
来源：http://vqs.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://uki.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zbj.snrcjt.cn

[U59] PHP：自定义排序
来源：http://gdv.xingfuxueyuan.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://muo.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://jmv.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vij.zdbjq.cn

[U61] PHP：正则
来源：http://ojo.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nzy.yangfankeji.com

[U62] PHP：日期对象
来源：http://fnx.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dco.yfazqb.com


<!-- 参考信息 -->