代发 wailian999

[S35] C++：map
来源：http://ipb.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nxy.birdmap.top

[S36] C++：unordered_map
来源：http://nge.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tts.sufxvd.cn

[S37] C++：set
来源：http://xai.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hcc.svipenyu.cn

[S38] C++：排序
来源：http://zjg.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://opx.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://bvz.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jrf.vqdsnc.cn

[S40] C++：查找元素
来源：http://enq.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://enw.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://zao.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fph.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://but.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://tzz.sysykeji.top

[S43] C++：智能指针
来源：http://cqa.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://lob.yuanzhike.top

[S44] C++：引用传参
来源：http://wzf.cheryme.top

void inc(int &x) { ++x; }
来源：http://axs.fzhhl.top

[S45] C++：lambda
来源：http://elw.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://aqb.zhixingplan.top

[S46] C++：函数模板
来源：http://abl.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blf.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://hjr.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jhy.fehbvm.com

[S48] C++：逐行读文件
来源：http://qpb.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://qtt.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://kjc.wangshuangyany.cn

[S49] C++：写文件
来源：http://nws.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://krl.yangfankeji.com

[S50] C++：格式化数字
来源：http://zkv.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ufr.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://wft.zhengqikj.top

static_cast<double>(a) / b
来源：http://fda.yonumen.top

[S52] C++：const 与 noexcept
来源：http://rnp.jianghu66.top

int size() const noexcept { return n_; }
来源：http://tmf.sweek.top

[S53] C++：移动语义
来源：http://ftn.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://lkk.52xcode.cn

[S54] C++：异常处理
来源：http://tgy.yj20258.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fqb.fzhhl.top

[S55] C++：结构化绑定
来源：http://lsb.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pnt.xuetiantiany.cn

[S56] C++：optional
来源：http://geo.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dxv.yfazqb.com

[S57] C++：编译期常量
来源：http://wsa.nanxinkj.top

constexpr int N = 10;
来源：http://aob.bbcook.cn

[S58] C++：命名空间
来源：http://jpr.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://iug.hfpthk.cn

[S59] C++：静态断言
来源：http://ezx.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iag.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://poi.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kcr.fzhhl.top

================================================================================
来源：http://nas.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rjt.andypj.xyz

================================================================================
来源：http://ipo.316326.xyz

[T01] Kotlin：Hello World
来源：http://ami.jlsjyb.cn

println("Hello")
来源：http://kpk.shanyushiyangkeji.top

[T02] Kotlin：变量
来源：http://enp.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mlq.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://lkq.yongpay.top

"值: $b"
来源：http://idl.mhx1999.top

[T04] Kotlin：空安全
来源：http://bhq.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://hvx.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://izr.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bql.cheryme.top

[T06] Kotlin：集合映射
来源：http://qzo.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dpj.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://izl.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ofp.0kj1m.cn

[T08] Kotlin：数据类
来源：http://pte.tarul.cn

data class User(val name: String, val age: Int)
来源：http://pqx.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://rxx.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://hqr.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://vpv.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rsl.hnqzz.top

[T11] Kotlin：协程
来源：http://wbj.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yls.tanke756.top

[T12] Kotlin：解构声明
来源：http://wrb.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://tli.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://xtl.jianghu66.top

val m = mapOf("a" to 1)
来源：http://zsr.jianghu66.top

[T14] Kotlin：循环
来源：http://rje.nwbrower.top

for (i in 1..10) println(i)
来源：http://vbz.cheryme.top

[T15] Kotlin：接口
来源：http://xig.hnqzz.top

interface Shape { fun area(): Double }
来源：http://jvm.ybcxt.top

[T16] Swift：Hello World
来源：http://khd.hammf.cn

print("Hello")
来源：http://cai.xuanzx.com

[T17] Swift：变量与常量
来源：http://ptk.yfazqb.com

var a = 1;  let b = 2
来源：http://wwc.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://wut.tian-w.cn

"值: \(b)"
来源：http://xjs.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://ufd.smart0.xyz

if let n = opt { print(n) }
来源：http://ryf.haohaochexian.top

[T20] Swift：数组操作
来源：http://zja.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oge.pycfn.com

[T21] Swift：遍历
来源：http://gmb.vqdsnc.cn

for x in a { print(x) }
来源：http://syh.jinqigufen.top

[T22] Swift：字典
来源：http://cxh.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://vba.pengpengdd.cyou

[T23] Swift：函数
来源：http://vcm.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lcd.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://qpm.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bqd.tianlin.xyz

[T25] Swift：结构体
来源：http://sms.yongpay.top

struct P { var x: Int }
来源：http://xgi.hesvh.cn

[T26] Swift：类与重写
来源：http://jde.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://bea.pycfn.com

[T27] Swift：错误处理
来源：http://onj.daxiang520.top

do { try f() } catch { print(error) }
来源：http://ekp.jqgfzy.top

[T28] Swift：枚举
来源：http://ybd.hfpthk.cn

enum Color { case red, green }
来源：http://avd.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://wny.zhiwuduotai.top

guard let x = opt else { return }
来源：http://xvf.52xcode.cn

[T30] Swift：协议
来源：http://ilm.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://xle.fehbvm.com

[T31] Lua：Hello World
来源：http://ccg.wangdashe.top

print("Hello")
来源：http://zng.yuxming.cn

[T32] Lua：局部变量
来源：http://wwh.epnwcf.com

local a = 1
来源：http://wsm.hammf.cn

[T33] Lua：表（数组）
来源：http://hnt.chenzaomai.com

local t = {1, 2, 3};  t[4] = 4
来源：http://lfg.vehdjk.com

[T34] Lua：遍历表
来源：http://nvf.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lgw.c1oappe.top

[T35] Lua：字典表
来源：http://ahr.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://gdh.guannengcc.top

[T36] Lua：函数
来源：http://jym.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://djc.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://guo.fktsv.cn

"a" .. "b"
来源：http://ztp.jqgfzy.top

[T38] Lua：条件
来源：http://hyu.tanke756.top

if x > 0 then print("正") end
来源：http://gkp.iojbl.cn

[T39] Lua：模式匹配
来源：http://uqn.yuanzhike.top

string.find(s, "%d+")
来源：http://amr.vqdsnc.cn

[T40] Lua：元表
来源：http://iwt.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://bpn.hcnkem.com

[T41] Perl：Hello World
来源：http://tpa.jqgufenzy.top

print "Hello\n";
来源：http://xyk.uphjek.com

[T42] Perl：变量类型
来源：http://omp.bjfxy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://thi.cheryme.top

[T43] Perl：字符串插值
来源：http://cgz.zhixingplan.top

"值: $a"
来源：http://bgi.feifeiyinyue.top

[T44] Perl：条件
来源：http://rcf.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://oqn.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://ryj.birdmap.top

for my $x (@arr) { print $x; }
来源：http://ihw.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://uln.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wkp.iojbl.cn

[T47] Perl：正则捕获
来源：http://tmw.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rza.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://ues.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://llv.tanke756.top

[T49] Perl：函数
来源：http://qpb.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xkk.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://sof.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jsj.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://lxi.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://nwm.feifeiyinyue.top

println("Hello")
来源：http://unh.gotoacloud.top

[T52] Scala：变量
来源：http://rgl.uphjek.com

val a = 1;  var b = 2
来源：http://xzi.gotoacloud.top

[T53] Scala：字符串插值
来源：http://zvh.kuanghao11.cn

s"值: $b"
来源：http://nke.tianlin.xyz

[T54] Scala：集合映射
来源：http://kps.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://rwu.wangdashe.top

[T55] Scala：集合过滤
来源：http://cca.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://kow.mhx1999.top

[T56] Scala：样例类
来源：http://dvf.meibo888.top

case class User(name: String, age: Int)
来源：http://pjn.cashguo.top

[T57] Scala：模式匹配
来源：http://jzg.tianlin.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ocp.yj20258888.top

[T58] Scala：函数定义
来源：http://hiz.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://ipt.xuanzx.com

[T59] Scala：循环
来源：http://cla.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://ffw.vqdsnc.cn

[T60] Scala：折叠
来源：http://rqa.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xui.birdmap.top

================================================================================
来源：http://clo.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://phw.hnxiangtu.top

================================================================================
来源：http://act.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://osx.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uqn.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://xcr.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dgm.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://bci.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://abh.nwbrower.top

[U04] Py：变量调试打印
来源：http://eau.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mrq.cheryme.top

[U05] Py：列表去重且保序
来源：http://krw.aizwys.cn

list(dict.fromkeys(arr))
来源：http://vjl.yonumen.top

[U06] Py：合并两个字典
来源：http://cvn.yvedp.cn

{**a, **b}
来源：http://dmy.0kj1m.cn

[U07] Py：反转字典键值
来源：http://tcc.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://yfc.shzxlz.cn

[U08] Py：展平二维列表
来源：http://yhc.andypj.xyz

[y for x in nested for y in x]
来源：http://dzy.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://exe.svipenyu.cn

max(d, key=d.get)
来源：http://ivx.zhengqikj.top

[U10] Py：按值排序字典
来源：http://vti.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://reh.shuidangran.top

[U11] Py：生成器表达式
来源：http://src.vehdjk.com

(x * 2 for x in arr)
来源：http://ivq.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://kke.dianchejie.cn

Counter(arr).most_common(3)
来源：http://myl.zycfv.cn

[U13] Py：固定长度队列
来源：http://uiy.guowangkeji.top

deque(maxlen=10)
来源：http://xrv.xziqi.cn

[U14] Py：分组收集到列表
来源：http://kih.hfpthk.cn

defaultdict(list)
来源：http://fwu.iojbl.cn

[U15] Py：高精度计时
来源：http://blb.dashuyun.cn

t = time.perf_counter()
来源：http://kyr.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://oor.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rvw.sufxvd.cn

[U17] Py：初始化日志
来源：http://cch.snrcjt.cn

logging.basicConfig(level=logging.INFO)
来源：http://dfc.aibaodan.cn

[U18] Py：预编译正则
来源：http://wku.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://qmi.aizwys.cn

[U19] Py：正则替换带回调
来源：http://yjq.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ots.cashguo.top

[U20] Py：缓存函数结果
来源：http://beg.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://maa.sjlbkw.cn

[U21] Py：自定义上下文管理器
来源：http://wlu.vehdjk.com

@contextlib.contextmanager
来源：http://nqr.gzhubu.top

[U22] Py：矩阵转置
来源：http://ziu.jiagoushi.top

list(zip(*m))
来源：http://qpp.smart0.xyz

[U23] Py：分块读取大文件
来源：http://lfp.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ils.jianghu66.top

[U24] Py：路径操作
来源：http://qki.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qce.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://dzk.ydjk.org.cn

csv.DictReader(f)
来源：http://joq.zdqjudy.top

[U26] Py：并发下载
来源：http://rjm.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ehi.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://haz.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://vrd.bbcook.cn

[U28] Py：类型别名
来源：http://cwv.hnqzz.top

UserId = int
来源：http://bbj.hammf.cn

[U29] Py：属性校验
来源：http://jiz.hysaishi.cn

@property 与 @x.setter 配合
来源：http://iqz.hysaishi.cn

[U30] Py：数据类
来源：http://oxp.chenzaomai.com

@dataclass(slots=True)
来源：http://ixc.fehbvm.com

[U31] Py：单测
来源：http://dwc.zycfv.cn

python -m pytest -q
来源：http://hae.yongpay.top

[U32] Py：代码格式化
来源：http://jsm.tian-w.cn

ruff format . && ruff check --fix .
来源：http://yqf.fanxiaobao.xyz

[U33] Py：打包发布
来源：http://cai.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://mqf.ppjwa.cn

[U34] Py：判断编码
来源：http://hau.yangfankeji.com

chardet.detect(raw)
来源：http://bnu.yuxming.cn

[U35] Py：发送邮件
来源：http://uka.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kyv.yj20258.top

[U36] Py：定时任务
来源：http://kyl.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://wnf.shuidangran.top

[U37] Py：读写 Excel
来源：http://xgc.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pjd.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://mtj.cheryme.top

Path(__file__).resolve().parent
来源：http://jda.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://vug.guowangkeji.top

sys.stdout.isatty()
来源：http://kth.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://dqb.aibaodan.cn

print("err", file=sys.stderr)
来源：http://kys.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://gao.smart0.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://obi.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://sqb.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fzi.sxryk.cn

[U43] PHP：声明命名空间
来源：http://fqq.yanxiufei.cn

namespace App\Http;
来源：http://cui.daria6918.cn

[U44] PHP：开启严格类型
来源：http://skf.yvedp.cn

declare(strict_types=1);
来源：http://hyt.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://bhu.tanke756.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wez.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://rbp.jqgufenzy.top

?string $name = null
来源：http://pwf.ppjwa.cn

[U47] PHP：联合类型
来源：http://qlf.havefunace.top

int|string $id
来源：http://hqn.guannengcc.top

[U48] PHP：纯枚举
来源：http://mlw.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://coy.jqgfzy.top

[U49] PHP：只读属性
来源：http://wqc.ivvv.top

public readonly string $name
来源：http://gti.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://uxf.zycfv.cn

public function __construct(private int $id) {}
来源：http://wcx.jqgufenzy.top

[U51] PHP：数组解构
来源：http://tve.ppjwa.cn

[$a, $b] = $arr;
来源：http://ees.cdnleiting.top

[U52] PHP：箭头函数
来源：http://tzr.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://oac.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://mob.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://jew.yonumen.top

[U54] PHP：空安全调用
来源：http://mxt.pengpengdd.cyou

$obj?->method()
来源：http://vkf.daria6918.cn

[U55] PHP：match 表达式
来源：http://ptp.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xxq.ehwqpu.com

[U56] PHP：命名参数
来源：http://wll.daria6918.cn

f(a: 1, b: 2)
来源：http://gpg.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://ldb.meibo888.top

"值: {$a}"
来源：http://nod.ydzc1.top

[U58] PHP：数组三件套
来源：http://xme.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://brf.chenlongwang.top

[U59] PHP：自定义排序
来源：http://xoz.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ruy.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://zpu.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hpq.daria6918.cn


<!-- 参考信息 -->