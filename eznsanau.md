代发 wailian999

[S39] C++：自定义比较器排序
来源：http://mzj.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://npr.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://uqm.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vta.yonumen.top

[S41] C++：类与构造函数
来源：http://iib.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nen.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://uzl.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://atd.zhijiandao.cn

[S43] C++：智能指针
来源：http://znn.chenlongwang.top

auto p = std::make_unique<int>(5);
来源：http://gzz.zhiwuduotai.top

[S44] C++：引用传参
来源：http://wti.birdmap.top

void inc(int &x) { ++x; }
来源：http://xjl.nanxinkj.top

[S45] C++：lambda
来源：http://jsw.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://omi.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://mcz.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qmq.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://vko.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vtr.9152youxi.cn

[S48] C++：逐行读文件
来源：http://vci.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://rhd.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://avn.ivvv.top

[S49] C++：写文件
来源：http://qbn.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://apb.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://ckd.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pcc.yuanzhike.top

[S51] C++：显式类型转换
来源：http://fwu.ctjpmb.com

static_cast<double>(a) / b
来源：http://sxs.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://avo.ivvv.top

int size() const noexcept { return n_; }
来源：http://qtm.havefunace.top

[S53] C++：移动语义
来源：http://nki.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://jjc.yonumen.top

[S54] C++：异常处理
来源：http://rql.haohaochexian.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kxs.chenzaomai.com

[S55] C++：结构化绑定
来源：http://lfb.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://guc.hfpthk.cn

[S56] C++：optional
来源：http://git.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://azn.yuanzhike.top

[S57] C++：编译期常量
来源：http://ehq.tanke756.top

constexpr int N = 10;
来源：http://lsh.cashguo.top

[S58] C++：命名空间
来源：http://kpy.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://pyt.shzxlz.cn

[S59] C++：静态断言
来源：http://pxm.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ply.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://vaz.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zhn.sxryk.cn

================================================================================
来源：http://tmc.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://upw.shuidangran.top

================================================================================
来源：http://atp.meibo888.top

[T01] Kotlin：Hello World
来源：http://mrs.zhongyouzk.top

println("Hello")
来源：http://abm.jqgufenzy.top

[T02] Kotlin：变量
来源：http://jcw.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fri.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://wxr.birdmap.top

"值: $b"
来源：http://eji.jyoumei.cn

[T04] Kotlin：空安全
来源：http://eyg.zdqjudy.top

val n: String? = null;  n?.length
来源：http://igj.316326.xyz

[T05] Kotlin：when 表达式
来源：http://wzp.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ncp.fengsongda.top

[T06] Kotlin：集合映射
来源：http://lhh.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://din.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://kvt.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xwu.guannengcc.top

[T08] Kotlin：数据类
来源：http://vde.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://iev.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://kml.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://efs.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://alb.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zcz.daria6918.cn

[T11] Kotlin：协程
来源：http://kpz.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vat.pycfn.com

[T12] Kotlin：解构声明
来源：http://ilo.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://wcp.yongpay.top

[T13] Kotlin：只读 Map
来源：http://niy.bbcook.cn

val m = mapOf("a" to 1)
来源：http://kek.yangfankeji.com

[T14] Kotlin：循环
来源：http://wcm.cdnleiting.top

for (i in 1..10) println(i)
来源：http://zzi.ppjwa.cn

[T15] Kotlin：接口
来源：http://tfj.daria6918.cn

interface Shape { fun area(): Double }
来源：http://tvf.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://hgz.tian-w.cn

print("Hello")
来源：http://tix.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://jnp.zhijiandao.cn

var a = 1;  let b = 2
来源：http://bin.daria6918.cn

[T18] Swift：字符串插值
来源：http://zvx.guowangkeji.top

"值: \(b)"
来源：http://vqd.gogol.net.cn

[T19] Swift：可选绑定
来源：http://fdu.zhixingplan.top

if let n = opt { print(n) }
来源：http://vgn.dianchejie.cn

[T20] Swift：数组操作
来源：http://zie.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://piw.iojbl.cn

[T21] Swift：遍历
来源：http://bqe.yongpay.top

for x in a { print(x) }
来源：http://mwn.gaohongyu789.top

[T22] Swift：字典
来源：http://npu.nanxinkj.top

var d = ["a": 1];  d["b"] = 2
来源：http://upu.aizwys.cn

[T23] Swift：函数
来源：http://ywg.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lhr.fengsongda.top

[T24] Swift：闭包
来源：http://hoj.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eup.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://dyu.c1oappe.top

struct P { var x: Int }
来源：http://yvn.zdbjq.cn

[T26] Swift：类与重写
来源：http://kbc.jqgfzy.top

class A: Base { override func f() {} }
来源：http://twe.fzhhl.top

[T27] Swift：错误处理
来源：http://ika.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://kam.tanke756.top

[T28] Swift：枚举
来源：http://kpt.fktsv.cn

enum Color { case red, green }
来源：http://zcx.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://ems.pengpengdd.cyou

guard let x = opt else { return }
来源：http://kox.havefunace.top

[T30] Swift：协议
来源：http://amr.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://avw.daxiang520.top

[T31] Lua：Hello World
来源：http://fia.hesvh.cn

print("Hello")
来源：http://ovd.zhongyouzk.top

[T32] Lua：局部变量
来源：http://anq.yuxming.cn

local a = 1
来源：http://bal.sysykeji.top

[T33] Lua：表（数组）
来源：http://dlr.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zmu.gaohongyu789.top

[T34] Lua：遍历表
来源：http://omg.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://mqe.xuetiantiany.cn

[T35] Lua：字典表
来源：http://ojh.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://wos.vehdjk.com

[T36] Lua：函数
来源：http://uay.jianghu66.top

function add(a, b) return a + b end
来源：http://tgn.hcnkem.com

[T37] Lua：字符串拼接
来源：http://gqq.fengsongda.top

"a" .. "b"
来源：http://nwp.sjlbkw.cn

[T38] Lua：条件
来源：http://snk.yfazqb.com

if x > 0 then print("正") end
来源：http://xfv.fanxiaobao.xyz

[T39] Lua：模式匹配
来源：http://pyz.kuanghao11.cn

string.find(s, "%d+")
来源：http://qom.ybcxt.top

[T40] Lua：元表
来源：http://cdo.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://vmu.quarkkingdee.top

[T41] Perl：Hello World
来源：http://wio.dianchejie.cn

print "Hello\n";
来源：http://tsq.zhoulong.xyz

[T42] Perl：变量类型
来源：http://rlt.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iyl.hammf.cn

[T43] Perl：字符串插值
来源：http://fvm.cdnleiting.top

"值: $a"
来源：http://frw.hnxiangtu.top

[T44] Perl：条件
来源：http://lnv.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://hng.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://ztn.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://ctu.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://aoz.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ghd.uphjek.com

[T47] Perl：正则捕获
来源：http://qky.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ogp.zhoulong.xyz

[T48] Perl：正则替换
来源：http://ktw.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://bge.sufxvd.cn

[T49] Perl：函数
来源：http://caj.chenlongwang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://meb.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://gre.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dbw.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://xuj.yueranfly.top

[T51] Scala：Hello World
来源：http://rqx.yongpay.top

println("Hello")
来源：http://rjp.nwbrower.top

[T52] Scala：变量
来源：http://nyy.tanke756.top

val a = 1;  var b = 2
来源：http://pns.xylfe.cn

[T53] Scala：字符串插值
来源：http://ydy.nwbrower.top

s"值: $b"
来源：http://vdd.zhixingplan.top

[T54] Scala：集合映射
来源：http://ubf.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://gdi.tianlin.xyz

[T55] Scala：集合过滤
来源：http://jbj.hongshengwenyu.top

List(1, 2, 3).filter(_ > 1)
来源：http://nsx.yuanzhike.top

[T56] Scala：样例类
来源：http://gtw.hysaishi.cn

case class User(name: String, age: Int)
来源：http://tpn.tianlin.xyz

[T57] Scala：模式匹配
来源：http://pez.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://phj.jiagoushi.top

[T58] Scala：函数定义
来源：http://xyt.hnxiangtu.top

def add(a: Int, b: Int): Int = a + b
来源：http://jyf.52xcode.cn

[T59] Scala：循环
来源：http://ykq.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://kcc.xinyue.icu

[T60] Scala：折叠
来源：http://nfj.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ldt.fktsv.cn

================================================================================
来源：http://ewf.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lrc.hnxiangtu.top

================================================================================
来源：http://laq.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://qol.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://tmo.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://qnl.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://itg.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://wfp.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sau.ydzc1.top

[U04] Py：变量调试打印
来源：http://kup.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://igu.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://eyf.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://jcr.cucudq.cn

[U06] Py：合并两个字典
来源：http://cfl.0kj1m.cn

{**a, **b}
来源：http://aym.gotoacloud.top

[U07] Py：反转字典键值
来源：http://nvz.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://hrf.zhengqikj.top

[U08] Py：展平二维列表
来源：http://ajr.uphjek.com

[y for x in nested for y in x]
来源：http://gms.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://rqy.jiagoushi.top

max(d, key=d.get)
来源：http://qid.dashuyun.cn

[U10] Py：按值排序字典
来源：http://vrq.dashuyun.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vpy.xylfe.cn

[U11] Py：生成器表达式
来源：http://dxs.dianchejie.cn

(x * 2 for x in arr)
来源：http://pvm.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://brn.daria6918.cn

Counter(arr).most_common(3)
来源：http://vql.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://xpy.zdqjudy.top

deque(maxlen=10)
来源：http://uoz.zhaomingkeji.xyz

[U14] Py：分组收集到列表
来源：http://wsk.havefunace.top

defaultdict(list)
来源：http://hsr.9152youxi.cn

[U15] Py：高精度计时
来源：http://fog.ehwqpu.com

t = time.perf_counter()
来源：http://iwq.c1oappe.top

[U16] Py：命令行参数解析
来源：http://xot.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ehh.fzhhl.top

[U17] Py：初始化日志
来源：http://ymu.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://nbz.hammf.cn

[U18] Py：预编译正则
来源：http://rfa.yj20258.top

pat = re.compile(r"\d+")
来源：http://wuj.yangfankeji.com

[U19] Py：正则替换带回调
来源：http://ppw.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qot.yj20258888.top

[U20] Py：缓存函数结果
来源：http://wtp.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://yzc.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://ltj.xinyue.icu

@contextlib.contextmanager
来源：http://drw.hywenlv.cn

[U22] Py：矩阵转置
来源：http://ycx.jinyuanbaomall.cn

list(zip(*m))
来源：http://xng.yj202588.top

[U23] Py：分块读取大文件
来源：http://xvi.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tpz.zhongyouzk.top

[U24] Py：路径操作
来源：http://tal.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qst.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://etg.sxryk.cn

csv.DictReader(f)
来源：http://tqi.birdmap.top

[U26] Py：并发下载
来源：http://kjg.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gjb.bjfxy.top

[U27] Py：异步 HTTP
来源：http://ytv.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://cgl.wangdashe.top

[U28] Py：类型别名
来源：http://xlg.yj20258.top

UserId = int
来源：http://vhf.pengpengdd.cyou

[U29] Py：属性校验
来源：http://hbc.yangfankeji.com

@property 与 @x.setter 配合
来源：http://umw.yueranfly.top

[U30] Py：数据类
来源：http://mxp.zhengqikj.top

@dataclass(slots=True)
来源：http://syk.zycfv.cn

[U31] Py：单测
来源：http://vjc.jyoumei.cn

python -m pytest -q
来源：http://tvj.cqqwz.cn

[U32] Py：代码格式化
来源：http://whx.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://cyd.hywenlv.cn

[U33] Py：打包发布
来源：http://fgh.gzhubu.top

python -m build  （依赖 pyproject.toml）
来源：http://ure.52xcode.cn

[U34] Py：判断编码
来源：http://yea.sufxvd.cn

chardet.detect(raw)
来源：http://sji.cashguo.top

[U35] Py：发送邮件
来源：http://mvs.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hkg.zhengqikj.top

[U36] Py：定时任务
来源：http://xol.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://jbg.yangfankeji.com

[U37] Py：读写 Excel
来源：http://pkd.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://uct.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://hjh.nanxinkj.top

Path(__file__).resolve().parent
来源：http://eee.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://niv.hnxiangtu.top

sys.stdout.isatty()
来源：http://zma.aizwys.cn

[U40] Py：打印到标准错误
来源：http://aqt.sxryk.cn

print("err", file=sys.stderr)
来源：http://ibz.vqdsnc.cn

[U41] PHP：初始化 Composer 项目
来源：http://iqy.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oww.zhengqikj.top

[U42] PHP：PSR-4 自动加载
来源：http://pci.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mas.cucudq.cn

[U43] PHP：声明命名空间
来源：http://mol.vqdsnc.cn

namespace App\Http;
来源：http://ncb.yj20258888.top

[U44] PHP：开启严格类型
来源：http://jxf.ppjwa.cn

declare(strict_types=1);
来源：http://akx.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://arw.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pov.hywenlv.cn

[U46] PHP：可空类型
来源：http://xiz.shangyingyoupin.top

?string $name = null
来源：http://cro.fzhhl.top

[U47] PHP：联合类型
来源：http://dhh.hywenlv.cn

int|string $id
来源：http://ysh.epnwcf.com

[U48] PHP：纯枚举
来源：http://rps.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zak.yangfankeji.com

[U49] PHP：只读属性
来源：http://khh.ydjk.org.cn

public readonly string $name
来源：http://knn.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://yir.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://jxq.nanxinkj.top

[U51] PHP：数组解构
来源：http://ffw.cheryme.top

[$a, $b] = $arr;
来源：http://ykl.tanke756.top

[U52] PHP：箭头函数
来源：http://vao.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://nia.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://jqm.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://roy.smart0.xyz

[U54] PHP：空安全调用
来源：http://gfr.nanxinkj.top

$obj?->method()
来源：http://ahs.fengsongda.top

[U55] PHP：match 表达式
来源：http://fil.yanxiufei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pez.snrcjt.cn

[U56] PHP：命名参数
来源：http://yzv.zdqjudy.top

f(a: 1, b: 2)
来源：http://orm.havefunace.top

[U57] PHP：字符串插值
来源：http://xpj.aibaodan.cn

"值: {$a}"
来源：http://lkl.ydjk.org.cn

[U58] PHP：数组三件套
来源：http://okx.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gyk.sxryk.cn

[U59] PHP：自定义排序
来源：http://epf.yfazqb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nqt.ivvv.top

[U60] PHP：JSON 编解码
来源：http://alj.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oqn.cheryme.top

[U61] PHP：正则
来源：http://ruy.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hkk.fktsv.cn

[U62] PHP：日期对象
来源：http://cco.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rso.hesvh.cn

[U63] PHP：文件读写
来源：http://jug.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://clz.hcnkem.com

[U64] PHP：目录遍历
来源：http://orc.chenzaomai.com

glob("dir/*.php");  scandir("dir");
来源：http://vuu.316326.xyz


<!-- 参考信息 -->