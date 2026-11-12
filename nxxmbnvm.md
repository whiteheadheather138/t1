代发 wailian999

#include <iostream>
来源：http://smd.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://njs.cqqwz.cn

[S32] C++：字符串
来源：http://pvu.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://wfq.tanke756.top

[S33] C++：vector 增删
来源：http://tgq.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zzv.yvedp.cn

[S34] C++：遍历 vector
来源：http://hvl.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://jih.jiagoushi.top

[S35] C++：map
来源：http://sfj.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://soz.yonumen.top

[S36] C++：unordered_map
来源：http://uqy.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jvt.havefunace.top

[S37] C++：set
来源：http://hqk.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wcf.sxryk.cn

[S38] C++：排序
来源：http://hvc.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://hct.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://mwh.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qbp.zhongyouzk.top

[S40] C++：查找元素
来源：http://vqd.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lwk.fehbvm.com

[S41] C++：类与构造函数
来源：http://ifc.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jwd.pycfn.com

[S42] C++：继承与虚函数
来源：http://lre.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://alp.gaohongyu789.top

[S43] C++：智能指针
来源：http://xdb.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://hnl.jinqigfzy.top

[S44] C++：引用传参
来源：http://evb.cashguo.top

void inc(int &x) { ++x; }
来源：http://zyu.tian-w.cn

[S45] C++：lambda
来源：http://sxj.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://bgu.uphjek.com

[S46] C++：函数模板
来源：http://xqq.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vst.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://koo.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zoe.shzxlz.cn

[S48] C++：逐行读文件
来源：http://qeq.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://sgn.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://eav.yuanzhike.top

[S49] C++：写文件
来源：http://hcj.xuanzx.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kiw.52xcode.cn

[S50] C++：格式化数字
来源：http://uwv.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qaw.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://rtt.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://yyx.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://jyk.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://til.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://cmp.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://lgp.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://imb.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gyq.andypj.xyz

[S55] C++：结构化绑定
来源：http://msh.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xzl.316326.xyz

[S56] C++：optional
来源：http://tau.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ksn.jlsjyb.cn

[S57] C++：编译期常量
来源：http://qei.zhongyouzk.top

constexpr int N = 10;
来源：http://pwt.316326.xyz

[S58] C++：命名空间
来源：http://ddh.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://zaq.dianchejie.cn

[S59] C++：静态断言
来源：http://bov.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://luh.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://msd.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sad.ctjpmb.com

================================================================================
来源：http://mgx.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qqa.chenlongwang.top

================================================================================
来源：http://hqy.bjfxy.top

[T01] Kotlin：Hello World
来源：http://tfy.9152youxi.cn

println("Hello")
来源：http://bql.jqgfzy.top

[T02] Kotlin：变量
来源：http://iqd.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vkk.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://aes.ppjwa.cn

"值: $b"
来源：http://eal.xuanzx.com

[T04] Kotlin：空安全
来源：http://axn.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://ffy.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://nxh.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hre.yj20258888.top

[T06] Kotlin：集合映射
来源：http://wid.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fxl.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://xsm.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://rir.jiagoushi.top

[T08] Kotlin：数据类
来源：http://hmo.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://zhj.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://prx.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://wfr.cheryme.top

[T10] Kotlin：默认参数
来源：http://bnz.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pnc.gzhubu.top

[T11] Kotlin：协程
来源：http://mzb.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hag.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://nvs.cashguo.top

val (a, b) = Pair(1, 2)
来源：http://kdj.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://wal.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://siy.yj20258.top

[T14] Kotlin：循环
来源：http://ubn.ydzc1.top

for (i in 1..10) println(i)
来源：http://eyz.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://nvr.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://blw.zdbjq.cn

[T16] Swift：Hello World
来源：http://dhs.cashguo.top

print("Hello")
来源：http://iaq.shanyushiyangkeji.top

[T17] Swift：变量与常量
来源：http://mpv.chenzaomai.com

var a = 1;  let b = 2
来源：http://ccl.zhengqikj.top

[T18] Swift：字符串插值
来源：http://iqe.sufxvd.cn

"值: \(b)"
来源：http://uob.hongshengwenyu.top

[T19] Swift：可选绑定
来源：http://axw.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://tzl.jqgfzy.top

[T20] Swift：数组操作
来源：http://top.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://fxy.xuanzx.com

[T21] Swift：遍历
来源：http://ljo.0kj1m.cn

for x in a { print(x) }
来源：http://hcd.cashguo.top

[T22] Swift：字典
来源：http://orj.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://vof.hesvh.cn

[T23] Swift：函数
来源：http://dti.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tvc.birdmap.top

[T24] Swift：闭包
来源：http://ezr.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ktx.jianghu66.top

[T25] Swift：结构体
来源：http://oxt.gogol.net.cn

struct P { var x: Int }
来源：http://rmq.epnwcf.com

[T26] Swift：类与重写
来源：http://uul.chenlongwang.top

class A: Base { override func f() {} }
来源：http://znt.cashguo.top

[T27] Swift：错误处理
来源：http://wsu.fengsongda.top

do { try f() } catch { print(error) }
来源：http://rqh.fzhhl.top

[T28] Swift：枚举
来源：http://wah.nwbrower.top

enum Color { case red, green }
来源：http://fsq.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://hfa.redwolf501.top

guard let x = opt else { return }
来源：http://gjo.haohaochexian.top

[T30] Swift：协议
来源：http://tle.cheryme.top

protocol Shape { func area() -> Double }
来源：http://wcl.bbcook.cn

[T31] Lua：Hello World
来源：http://mxc.bbcook.cn

print("Hello")
来源：http://fkq.daria6918.cn

[T32] Lua：局部变量
来源：http://pzx.aibaodan.cn

local a = 1
来源：http://dhg.havefunace.top

[T33] Lua：表（数组）
来源：http://voy.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fca.jinghuilouyu.cn

[T34] Lua：遍历表
来源：http://jof.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://utp.smart0.xyz

[T35] Lua：字典表
来源：http://oge.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://ayt.fanxiaobao.xyz

[T36] Lua：函数
来源：http://jjk.shzxlz.cn

function add(a, b) return a + b end
来源：http://xia.yj20258.top

[T37] Lua：字符串拼接
来源：http://wwy.aibaodan.cn

"a" .. "b"
来源：http://rkd.jianghu66.top

[T38] Lua：条件
来源：http://rxs.iojbl.cn

if x > 0 then print("正") end
来源：http://kqi.0kj1m.cn

[T39] Lua：模式匹配
来源：http://htg.guannengcc.top

string.find(s, "%d+")
来源：http://ons.yuxming.cn

[T40] Lua：元表
来源：http://rsr.epnwcf.com

setmetatable({}, { __index = base })
来源：http://ljq.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://oyh.sjlbkw.cn

print "Hello\n";
来源：http://zem.zdbjq.cn

[T42] Perl：变量类型
来源：http://hbo.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rkk.hammf.cn

[T43] Perl：字符串插值
来源：http://rii.nwbrower.top

"值: $a"
来源：http://amr.hesvh.cn

[T44] Perl：条件
来源：http://qvz.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://uqe.cheryme.top

[T45] Perl：数组遍历
来源：http://zdw.sweek.top

for my $x (@arr) { print $x; }
来源：http://bou.cdnleiting.top

[T46] Perl：哈希操作
来源：http://ecp.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fdi.smart0.xyz

[T47] Perl：正则捕获
来源：http://ois.sxryk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rwl.yvedp.cn

[T48] Perl：正则替换
来源：http://cka.tianlin.xyz

$s =~ s/old/new/g;
来源：http://vcv.yueranfly.top

[T49] Perl：函数
来源：http://teg.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://guz.mhx1999.top

[T50] Perl：逐行读文件
来源：http://sik.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pjm.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://jos.guannengcc.top

[T51] Scala：Hello World
来源：http://nkc.zhengqikj.top

println("Hello")
来源：http://jnq.ppjwa.cn

[T52] Scala：变量
来源：http://joa.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://nnl.tianlin.xyz

[T53] Scala：字符串插值
来源：http://jfx.svipenyu.cn

s"值: $b"
来源：http://nof.jiagoushi.top

[T54] Scala：集合映射
来源：http://tik.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://cab.cdnleiting.top

[T55] Scala：集合过滤
来源：http://sbn.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lut.vqdsnc.cn

[T56] Scala：样例类
来源：http://kca.sufxvd.cn

case class User(name: String, age: Int)
来源：http://uyt.cdnleiting.top

[T57] Scala：模式匹配
来源：http://uis.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://uiq.yj20258.top

[T58] Scala：函数定义
来源：http://occ.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://gia.tianlin.xyz

[T59] Scala：循环
来源：http://yjv.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://pwg.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://lkk.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jpp.haohaochexian.top

================================================================================
来源：http://etv.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lxe.cqqwz.cn

================================================================================
来源：http://awn.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://avt.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rwt.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://odu.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kbm.daria6918.cn

[U03] Py：加载 .env 配置
来源：http://rvc.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yqp.andypj.xyz

[U04] Py：变量调试打印
来源：http://wry.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pco.meibo888.top

[U05] Py：列表去重且保序
来源：http://qqt.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://lci.sysykeji.top

[U06] Py：合并两个字典
来源：http://gie.redwolf501.top

{**a, **b}
来源：http://ivw.0kj1m.cn

[U07] Py：反转字典键值
来源：http://pvp.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://xjs.uphjek.com

[U08] Py：展平二维列表
来源：http://sut.jlsjyb.cn

[y for x in nested for y in x]
来源：http://vwy.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://dlx.yonumen.top

max(d, key=d.get)
来源：http://hgv.daxiang520.top

[U10] Py：按值排序字典
来源：http://iax.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fii.pycfn.com

[U11] Py：生成器表达式
来源：http://nou.cucudq.cn

(x * 2 for x in arr)
来源：http://zjq.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://kpu.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://ooz.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://xbm.c1oappe.top

deque(maxlen=10)
来源：http://flo.daxiang520.top

[U14] Py：分组收集到列表
来源：http://fjz.aibaodan.cn

defaultdict(list)
来源：http://sko.9152youxi.cn

[U15] Py：高精度计时
来源：http://tcz.ydjk.org.cn

t = time.perf_counter()
来源：http://nds.xziqi.cn

[U16] Py：命令行参数解析
来源：http://uwz.dashuyun.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ger.sufxvd.cn

[U17] Py：初始化日志
来源：http://wsx.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://bri.fzhhl.top

[U18] Py：预编译正则
来源：http://jon.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://nex.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://fec.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://whb.fzhhl.top

[U20] Py：缓存函数结果
来源：http://hdo.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://pye.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://gpq.jiagoushi.top

@contextlib.contextmanager
来源：http://spq.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://owr.hnqzz.top

list(zip(*m))
来源：http://eov.ctjpmb.com

[U23] Py：分块读取大文件
来源：http://bjj.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wks.cheryme.top

[U24] Py：路径操作
来源：http://hqa.pengpengdd.cyou

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gez.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://eix.zdbjq.cn

csv.DictReader(f)
来源：http://pot.mhx1999.top

[U26] Py：并发下载
来源：http://nun.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ims.yuxming.cn

[U27] Py：异步 HTTP
来源：http://ysm.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://kcu.jinghuilouyu.cn

[U28] Py：类型别名
来源：http://zrh.jqgufenzy.top

UserId = int
来源：http://clj.jqgufenzy.top

[U29] Py：属性校验
来源：http://xsm.9152youxi.cn

@property 与 @x.setter 配合
来源：http://usb.wangdashe.top

[U30] Py：数据类
来源：http://uqv.316326.xyz

@dataclass(slots=True)
来源：http://ekz.dashuyun.cn

[U31] Py：单测
来源：http://yhm.yuxming.cn

python -m pytest -q
来源：http://lkw.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://iuu.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://eox.ybcxt.top

[U33] Py：打包发布
来源：http://rla.jqgufenzy.top

python -m build  （依赖 pyproject.toml）
来源：http://tay.uphjek.com

[U34] Py：判断编码
来源：http://dzb.xuanzx.com

chardet.detect(raw)
来源：http://wfl.xziqi.cn

[U35] Py：发送邮件
来源：http://mit.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sgr.sysykeji.top

[U36] Py：定时任务
来源：http://cln.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://znj.cqqwz.cn

[U37] Py：读写 Excel
来源：http://ics.jyoumei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ddy.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://tpk.smart0.xyz

Path(__file__).resolve().parent
来源：http://hcq.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://jcw.tanke756.top

sys.stdout.isatty()
来源：http://vus.cdnleiting.top

[U40] Py：打印到标准错误
来源：http://xpi.9152youxi.cn

print("err", file=sys.stderr)
来源：http://frn.jqgfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://xcr.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://khf.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://uby.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dcp.bjfxy.top

[U43] PHP：声明命名空间
来源：http://ncv.yuxming.cn

namespace App\Http;
来源：http://cmz.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://hon.jyoumei.cn

declare(strict_types=1);
来源：http://vrl.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://vtz.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://bpc.xylfe.cn

[U46] PHP：可空类型
来源：http://hcg.ywan-chungtsiang.top

?string $name = null
来源：http://acx.jiagoushi.top

[U47] PHP：联合类型
来源：http://mkh.dashuyun.cn

int|string $id
来源：http://iaw.gotoacloud.top

[U48] PHP：纯枚举
来源：http://apk.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pie.hfpthk.cn

[U49] PHP：只读属性
来源：http://mxx.zhijiandao.cn

public readonly string $name
来源：http://ksk.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://yxg.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://okc.guannengcc.top

[U51] PHP：数组解构
来源：http://qij.52xcode.cn

[$a, $b] = $arr;
来源：http://lvu.jianghu66.top

[U52] PHP：箭头函数
来源：http://ujt.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://kfu.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://znc.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://adk.guannengcc.top

[U54] PHP：空安全调用
来源：http://hom.redwolf501.top

$obj?->method()
来源：http://idr.zycfv.cn

[U55] PHP：match 表达式
来源：http://fry.hywenlv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://szv.yanxiufei.cn

[U56] PHP：命名参数
来源：http://gbe.yuanzhike.top

f(a: 1, b: 2)
来源：http://fdl.meibo888.top


<!-- 参考信息 -->