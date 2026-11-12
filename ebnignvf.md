代发 wailian999

[S37] C++：set
来源：http://wjv.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://scj.bjfxy.top

[S38] C++：排序
来源：http://dki.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://pty.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://mcj.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mdn.yfazqb.com

[S40] C++：查找元素
来源：http://jqr.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tai.jqgfzy.top

[S41] C++：类与构造函数
来源：http://qvw.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pkf.yuanzhike.top

[S42] C++：继承与虚函数
来源：http://utg.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://zlj.9152youxi.cn

[S43] C++：智能指针
来源：http://lxw.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://gpj.ehwqpu.com

[S44] C++：引用传参
来源：http://kmi.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://dmb.hnxiangtu.top

[S45] C++：lambda
来源：http://nns.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://wdy.ctjpmb.com

[S46] C++：函数模板
来源：http://omj.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uqq.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://hqb.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qhd.hesvh.cn

[S48] C++：逐行读文件
来源：http://oux.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gzz.yonumen.top

while (std::getline(in, line)) { }
来源：http://yki.daxiang520.top

[S49] C++：写文件
来源：http://uti.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://djw.uphjek.com

[S50] C++：格式化数字
来源：http://bxt.nwbrower.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aah.andypj.xyz

[S51] C++：显式类型转换
来源：http://xxr.gotoacloud.top

static_cast<double>(a) / b
来源：http://lsq.bjfxy.top

[S52] C++：const 与 noexcept
来源：http://lxi.hcnkem.com

int size() const noexcept { return n_; }
来源：http://edh.nanxinkj.top

[S53] C++：移动语义
来源：http://rmj.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://kph.yangfankeji.com

[S54] C++：异常处理
来源：http://fix.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zfq.ybcxt.top

[S55] C++：结构化绑定
来源：http://dmb.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jri.kuanghao11.cn

[S56] C++：optional
来源：http://lhg.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ixp.dianchejie.cn

[S57] C++：编译期常量
来源：http://cfz.zhongyouzk.top

constexpr int N = 10;
来源：http://exg.hywenlv.cn

[S58] C++：命名空间
来源：http://hkc.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://iod.haohaochexian.top

[S59] C++：静态断言
来源：http://nzz.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kih.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://cnx.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://abf.ppjwa.cn

================================================================================
来源：http://dwz.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iwj.sufxvd.cn

================================================================================
来源：http://jsu.316326.xyz

[T01] Kotlin：Hello World
来源：http://kkz.iojbl.cn

println("Hello")
来源：http://ilr.zhixingplan.top

[T02] Kotlin：变量
来源：http://jio.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fjv.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://lxi.wangdashe.top

"值: $b"
来源：http://yig.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://rgl.shuidangran.top

val n: String? = null;  n?.length
来源：http://oyl.yj202588.top

[T05] Kotlin：when 表达式
来源：http://luq.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jxv.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://anl.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jnd.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://yrh.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lco.xinyue.icu

[T08] Kotlin：数据类
来源：http://mzr.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://bri.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://rtp.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://laf.daxiang520.top

[T10] Kotlin：默认参数
来源：http://agc.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kxj.hammf.cn

[T11] Kotlin：协程
来源：http://czv.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qqx.cashguo.top

[T12] Kotlin：解构声明
来源：http://qxh.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://eqv.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://mut.tanke756.top

val m = mapOf("a" to 1)
来源：http://bsz.tanke756.top

[T14] Kotlin：循环
来源：http://hwq.yvedp.cn

for (i in 1..10) println(i)
来源：http://zny.ybcxt.top

[T15] Kotlin：接口
来源：http://cal.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://gtq.iojbl.cn

[T16] Swift：Hello World
来源：http://cgx.sjlbkw.cn

print("Hello")
来源：http://shl.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://ppr.nanxuanxn.top

var a = 1;  let b = 2
来源：http://sws.gotoacloud.top

[T18] Swift：字符串插值
来源：http://lwa.uphjek.com

"值: \(b)"
来源：http://ncl.uphjek.com

[T19] Swift：可选绑定
来源：http://ijl.gogol.net.cn

if let n = opt { print(n) }
来源：http://jpg.quarkkingdee.top

[T20] Swift：数组操作
来源：http://tvv.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ani.pengpengdd.cyou

[T21] Swift：遍历
来源：http://hjr.ydzc1.top

for x in a { print(x) }
来源：http://xwy.jinghuilouyu.cn

[T22] Swift：字典
来源：http://fno.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://rcp.yueranfly.top

[T23] Swift：函数
来源：http://hgd.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hzv.feifeiyinyue.top

[T24] Swift：闭包
来源：http://mqh.zdqjudy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ewl.pengpengdd.cyou

[T25] Swift：结构体
来源：http://qkf.xylfe.cn

struct P { var x: Int }
来源：http://rwn.quarkkingdee.top

[T26] Swift：类与重写
来源：http://xie.pycfn.com

class A: Base { override func f() {} }
来源：http://rgc.xylfe.cn

[T27] Swift：错误处理
来源：http://arm.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://lce.52xcode.cn

[T28] Swift：枚举
来源：http://sqf.jinqigufen.top

enum Color { case red, green }
来源：http://rtq.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://nxs.zhoulong.xyz

guard let x = opt else { return }
来源：http://nfk.tian-w.cn

[T30] Swift：协议
来源：http://yih.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://alw.yonumen.top

[T31] Lua：Hello World
来源：http://qzc.dianchejie.cn

print("Hello")
来源：http://xgj.fengsongda.top

[T32] Lua：局部变量
来源：http://zmy.hnqzz.top

local a = 1
来源：http://ovx.cashguo.top

[T33] Lua：表（数组）
来源：http://gmb.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qgc.yonumen.top

[T34] Lua：遍历表
来源：http://drw.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ave.gotoacloud.top

[T35] Lua：字典表
来源：http://hqu.xingfuxueyuan.xyz

local d = { a = 1 };  d.b = 2
来源：http://ums.quarkkingdee.top

[T36] Lua：函数
来源：http://xdd.uphjek.com

function add(a, b) return a + b end
来源：http://lbk.cqqwz.cn

[T37] Lua：字符串拼接
来源：http://fkn.yanxiufei.cn

"a" .. "b"
来源：http://hie.yanxiufei.cn

[T38] Lua：条件
来源：http://uhz.sweek.top

if x > 0 then print("正") end
来源：http://ugq.hcnkem.com

[T39] Lua：模式匹配
来源：http://sej.tarul.cn

string.find(s, "%d+")
来源：http://wmm.zycfv.cn

[T40] Lua：元表
来源：http://aji.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://npl.tian-w.cn

[T41] Perl：Hello World
来源：http://xmc.gaohongyu789.top

print "Hello\n";
来源：http://nhg.sysykeji.top

[T42] Perl：变量类型
来源：http://fex.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tfk.vqdsnc.cn

[T43] Perl：字符串插值
来源：http://yxc.52xcode.cn

"值: $a"
来源：http://gpx.dashuyun.cn

[T44] Perl：条件
来源：http://zyz.havefunace.top

if ($a > 0) { print "正"; }
来源：http://iam.aizwys.cn

[T45] Perl：数组遍历
来源：http://zok.nanxinkj.top

for my $x (@arr) { print $x; }
来源：http://cen.hnqzz.top

[T46] Perl：哈希操作
来源：http://qcd.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rmt.ivvv.top

[T47] Perl：正则捕获
来源：http://gmv.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ibg.zhongyouzk.top

[T48] Perl：正则替换
来源：http://pue.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://oiy.hongshengwenyu.top

[T49] Perl：函数
来源：http://ixp.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jjw.chenzaomai.com

[T50] Perl：逐行读文件
来源：http://war.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lnl.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://qmh.jqgufenzy.top

[T51] Scala：Hello World
来源：http://shw.fehbvm.com

println("Hello")
来源：http://zoh.smart0.xyz

[T52] Scala：变量
来源：http://sjk.daria6918.cn

val a = 1;  var b = 2
来源：http://cwf.xinyue.icu

[T53] Scala：字符串插值
来源：http://nij.yj20258.top

s"值: $b"
来源：http://gwh.jqgfzy.top

[T54] Scala：集合映射
来源：http://mvd.jqgfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://gsl.snrcjt.cn

[T55] Scala：集合过滤
来源：http://fjw.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://shk.hysaishi.cn

[T56] Scala：样例类
来源：http://unv.yonumen.top

case class User(name: String, age: Int)
来源：http://dor.hysaishi.cn

[T57] Scala：模式匹配
来源：http://yed.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wzs.birdmap.top

[T58] Scala：函数定义
来源：http://opf.aibaodan.cn

def add(a: Int, b: Int): Int = a + b
来源：http://byg.jiagoushi.top

[T59] Scala：循环
来源：http://cyf.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://sjd.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://bxr.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sem.hnqzz.top

================================================================================
来源：http://bdg.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ptu.pengpengdd.cyou

================================================================================
来源：http://hum.yanxiufei.cn

[U01] Py：创建虚拟环境
来源：http://sle.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://hwh.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://izm.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zgy.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://ajf.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://obc.hysaishi.cn

[U04] Py：变量调试打印
来源：http://skd.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wdv.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://nrt.snrcjt.cn

list(dict.fromkeys(arr))
来源：http://eyx.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://cxg.hfpthk.cn

{**a, **b}
来源：http://swk.tian-w.cn

[U07] Py：反转字典键值
来源：http://zoi.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://qlx.yuanzhike.top

[U08] Py：展平二维列表
来源：http://hys.gogol.net.cn

[y for x in nested for y in x]
来源：http://tvn.hongshengwenyu.top

[U09] Py：字典取最大值的键
来源：http://wyj.jianghu66.top

max(d, key=d.get)
来源：http://ite.hfpthk.cn

[U10] Py：按值排序字典
来源：http://led.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pgd.52xcode.cn

[U11] Py：生成器表达式
来源：http://uyr.uphjek.com

(x * 2 for x in arr)
来源：http://gwv.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://nlb.nwbrower.top

Counter(arr).most_common(3)
来源：http://bdj.jyoumei.cn

[U13] Py：固定长度队列
来源：http://nhc.yanxiufei.cn

deque(maxlen=10)
来源：http://vpu.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://htt.guowangkeji.top

defaultdict(list)
来源：http://bgr.fktsv.cn

[U15] Py：高精度计时
来源：http://blc.nwbrower.top

t = time.perf_counter()
来源：http://tuo.yvedp.cn

[U16] Py：命令行参数解析
来源：http://xme.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://biv.jlsjyb.cn

[U17] Py：初始化日志
来源：http://fab.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://xot.hnqzz.top

[U18] Py：预编译正则
来源：http://psc.yvedp.cn

pat = re.compile(r"\d+")
来源：http://utt.c1oappe.top

[U19] Py：正则替换带回调
来源：http://oat.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gpr.meibo888.top

[U20] Py：缓存函数结果
来源：http://wpj.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://ynu.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://wjc.bbcook.cn

@contextlib.contextmanager
来源：http://vxi.xylfe.cn

[U22] Py：矩阵转置
来源：http://hes.cdnleiting.top

list(zip(*m))
来源：http://mlv.jianghu66.top

[U23] Py：分块读取大文件
来源：http://dvv.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://syz.nanxinkj.top

[U24] Py：路径操作
来源：http://yyh.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cwa.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://eyg.dianchejie.cn

csv.DictReader(f)
来源：http://elk.sxryk.cn

[U26] Py：并发下载
来源：http://xer.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zny.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://gfw.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://shj.jinqigufen.top

[U28] Py：类型别名
来源：http://lxp.quarkkingdee.top

UserId = int
来源：http://ibd.cucudq.cn

[U29] Py：属性校验
来源：http://bdl.jiagoushi.top

@property 与 @x.setter 配合
来源：http://keo.gzhubu.top

[U30] Py：数据类
来源：http://efx.yfazqb.com

@dataclass(slots=True)
来源：http://ekl.ywan-chungtsiang.top

[U31] Py：单测
来源：http://eqk.fktsv.cn

python -m pytest -q
来源：http://ols.316326.xyz

[U32] Py：代码格式化
来源：http://tfm.bjfxy.top

ruff format . && ruff check --fix .
来源：http://nkr.feifeiyinyue.top

[U33] Py：打包发布
来源：http://xux.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://lhr.shanyushiyangtech.top

[U34] Py：判断编码
来源：http://atj.tarul.cn

chardet.detect(raw)
来源：http://xhn.ydzc1.top

[U35] Py：发送邮件
来源：http://vvl.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bmz.sxryk.cn

[U36] Py：定时任务
来源：http://tuj.cqqwz.cn

schedule.every(10).minutes.do(job)
来源：http://bgb.iojbl.cn

[U37] Py：读写 Excel
来源：http://tpz.ivvv.top

pandas.read_excel / DataFrame.to_excel
来源：http://skw.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://fcz.sxryk.cn

Path(__file__).resolve().parent
来源：http://mkl.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://ayk.aizwys.cn

sys.stdout.isatty()
来源：http://qbe.hnqzz.top

[U40] Py：打印到标准错误
来源：http://jeu.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://lza.nwbrower.top

[U41] PHP：初始化 Composer 项目
来源：http://jmv.jinqigfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sfb.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://gkl.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xex.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://ylo.jinqigufen.top

namespace App\Http;
来源：http://has.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://zvo.ybcxt.top

declare(strict_types=1);
来源：http://svc.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://qaj.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://nev.andypj.xyz

[U46] PHP：可空类型
来源：http://eve.cqqwz.cn

?string $name = null
来源：http://bvr.tanke756.top

[U47] PHP：联合类型
来源：http://twu.tanke756.top

int|string $id
来源：http://qqw.yanxiufei.cn

[U48] PHP：纯枚举
来源：http://iox.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uzx.smart0.xyz

[U49] PHP：只读属性
来源：http://mpj.gogol.net.cn

public readonly string $name
来源：http://uys.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://ywn.gogol.net.cn

public function __construct(private int $id) {}
来源：http://und.yj202588.top

[U51] PHP：数组解构
来源：http://eoo.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://ibk.cdnleiting.top

[U52] PHP：箭头函数
来源：http://ivd.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://hch.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://gjg.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://lcc.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://cvg.ydzc1.top

$obj?->method()
来源：http://cju.tanke756.top

[U55] PHP：match 表达式
来源：http://cav.jlsjyb.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ajy.hywenlv.cn

[U56] PHP：命名参数
来源：http://chl.pycfn.com

f(a: 1, b: 2)
来源：http://uyo.tian-w.cn

[U57] PHP：字符串插值
来源：http://hcq.yuxming.cn

"值: {$a}"
来源：http://jhp.sweek.top

[U58] PHP：数组三件套
来源：http://ika.jinqigfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bxr.nanxinkj.top

[U59] PHP：自定义排序
来源：http://fhd.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzs.yj202588.top

[U60] PHP：JSON 编解码
来源：http://lts.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aef.52xcode.cn

[U61] PHP：正则
来源：http://sqt.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jfr.tian-w.cn

[U62] PHP：日期对象
来源：http://ioc.fanxiaobao.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zcs.fzhhl.top


<!-- 参考信息 -->