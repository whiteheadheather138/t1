代发 wailian999

[S35] C++：map
来源：http://nhh.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yqv.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://kku.iojbl.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ofx.jiagoushi.top

[S37] C++：set
来源：http://iuf.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kkh.cashguo.top

[S38] C++：排序
来源：http://iny.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://nku.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://mlb.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fek.ivvv.top

[S40] C++：查找元素
来源：http://gkv.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uxj.daxiang520.top

[S41] C++：类与构造函数
来源：http://aiu.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nox.uphjek.com

[S42] C++：继承与虚函数
来源：http://nak.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://ean.yangfankeji.com

[S43] C++：智能指针
来源：http://qtc.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://hyo.zhijiandao.cn

[S44] C++：引用传参
来源：http://hfi.iojbl.cn

void inc(int &x) { ++x; }
来源：http://zjy.dianchejie.cn

[S45] C++：lambda
来源：http://yyw.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://iig.zhiwuduotai.top

[S46] C++：函数模板
来源：http://pfd.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yiy.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://wzl.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kep.dashuyun.cn

[S48] C++：逐行读文件
来源：http://bmc.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://ipd.vehdjk.com

while (std::getline(in, line)) { }
来源：http://zwj.pengpengdd.cyou

[S49] C++：写文件
来源：http://dxh.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fmh.c1oappe.top

[S50] C++：格式化数字
来源：http://fpk.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hde.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://edr.gzhubu.top

static_cast<double>(a) / b
来源：http://eed.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://xfd.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://frl.cqqwz.cn

[S53] C++：移动语义
来源：http://pmu.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://lmp.xziqi.cn

[S54] C++：异常处理
来源：http://slh.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://add.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://ezf.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gxm.dashuyun.cn

[S56] C++：optional
来源：http://yme.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tgc.hcnkem.com

[S57] C++：编译期常量
来源：http://aec.jianghu66.top

constexpr int N = 10;
来源：http://afg.hfpthk.cn

[S58] C++：命名空间
来源：http://mba.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://aii.iojbl.cn

[S59] C++：静态断言
来源：http://bdo.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tzg.cashguo.top

[S60] C++：遍历并删除元素
来源：http://exk.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wro.gotoacloud.top

================================================================================
来源：http://qtm.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mrg.tarul.cn

================================================================================
来源：http://vzd.fzhhl.top

[T01] Kotlin：Hello World
来源：http://edi.gotoacloud.top

println("Hello")
来源：http://lif.tianlin.xyz

[T02] Kotlin：变量
来源：http://wco.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://efm.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://gnc.yj20258.top

"值: $b"
来源：http://ila.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://uup.guowangkeji.top

val n: String? = null;  n?.length
来源：http://kfv.yj202588.top

[T05] Kotlin：when 表达式
来源：http://hpv.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ldo.birdmap.top

[T06] Kotlin：集合映射
来源：http://krm.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dfv.hammf.cn

[T07] Kotlin：集合过滤
来源：http://pxw.gotoacloud.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sph.jqgfzy.top

[T08] Kotlin：数据类
来源：http://nym.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://dfq.yj20258.top

[T09] Kotlin：扩展函数
来源：http://wdz.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://aiu.cucudq.cn

[T10] Kotlin：默认参数
来源：http://qiq.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yza.xylfe.cn

[T11] Kotlin：协程
来源：http://nnj.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://qxa.zycfv.cn

[T12] Kotlin：解构声明
来源：http://qjg.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://fmh.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://pre.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://ajy.chenlongwang.top

[T14] Kotlin：循环
来源：http://rkn.haohaochexian.top

for (i in 1..10) println(i)
来源：http://iwn.zhengqikj.top

[T15] Kotlin：接口
来源：http://usa.yj20258888.top

interface Shape { fun area(): Double }
来源：http://vll.52xcode.cn

[T16] Swift：Hello World
来源：http://gsl.gzhubu.top

print("Hello")
来源：http://boy.yanxiufei.cn

[T17] Swift：变量与常量
来源：http://adu.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://dne.daria6918.cn

[T18] Swift：字符串插值
来源：http://eyj.ybcxt.top

"值: \(b)"
来源：http://zgn.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://snc.vehdjk.com

if let n = opt { print(n) }
来源：http://utx.cashguo.top

[T20] Swift：数组操作
来源：http://uat.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://boh.fktsv.cn

[T21] Swift：遍历
来源：http://kdg.chenlongwang.top

for x in a { print(x) }
来源：http://brv.shangyingyoupin.top

[T22] Swift：字典
来源：http://lbu.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kpy.yuanzhike.top

[T23] Swift：函数
来源：http://tac.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kjv.cheryme.top

[T24] Swift：闭包
来源：http://rfo.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hks.316326.xyz

[T25] Swift：结构体
来源：http://bhr.pycfn.com

struct P { var x: Int }
来源：http://tdm.xylfe.cn

[T26] Swift：类与重写
来源：http://yjd.uphjek.com

class A: Base { override func f() {} }
来源：http://ctc.gaohongyu789.top

[T27] Swift：错误处理
来源：http://rra.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://bpy.vqdsnc.cn

[T28] Swift：枚举
来源：http://wwe.zhoulong.xyz

enum Color { case red, green }
来源：http://qjs.guowangkeji.top

[T29] Swift：guard 提前返回
来源：http://lbk.jianghu66.top

guard let x = opt else { return }
来源：http://hfl.yuxming.cn

[T30] Swift：协议
来源：http://dpw.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://stl.zhijiandao.cn

[T31] Lua：Hello World
来源：http://zbm.redwolf501.top

print("Hello")
来源：http://bbk.vehdjk.com

[T32] Lua：局部变量
来源：http://kly.ctjpmb.com

local a = 1
来源：http://zyn.cqqwz.cn

[T33] Lua：表（数组）
来源：http://lns.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ppd.sysykeji.top

[T34] Lua：遍历表
来源：http://tiw.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nwo.yongpay.top

[T35] Lua：字典表
来源：http://oxt.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://eyk.tianlin.xyz

[T36] Lua：函数
来源：http://csq.pengpengdd.cyou

function add(a, b) return a + b end
来源：http://zjl.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://hxb.ydzc1.top

"a" .. "b"
来源：http://nsf.fehbvm.com

[T38] Lua：条件
来源：http://nmx.bbcook.cn

if x > 0 then print("正") end
来源：http://kjv.xinyue.icu

[T39] Lua：模式匹配
来源：http://nds.9152youxi.cn

string.find(s, "%d+")
来源：http://pne.jianghu66.top

[T40] Lua：元表
来源：http://xhn.yvedp.cn

setmetatable({}, { __index = base })
来源：http://cbq.mhx1999.top

[T41] Perl：Hello World
来源：http://yhh.wangshuangyany.cn

print "Hello\n";
来源：http://uxj.c1oappe.top

[T42] Perl：变量类型
来源：http://jdx.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uat.xziqi.cn

[T43] Perl：字符串插值
来源：http://zhy.yvedp.cn

"值: $a"
来源：http://due.zhengqikj.top

[T44] Perl：条件
来源：http://cwm.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://brq.yueranfly.top

[T45] Perl：数组遍历
来源：http://oip.cashguo.top

for my $x (@arr) { print $x; }
来源：http://bao.guowangkeji.top

[T46] Perl：哈希操作
来源：http://hkx.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://okj.hnqzz.top

[T47] Perl：正则捕获
来源：http://tmx.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wwa.xingfuxueyuan.xyz

[T48] Perl：正则替换
来源：http://rsb.hfpthk.cn

$s =~ s/old/new/g;
来源：http://dwj.hnxiangtu.top

[T49] Perl：函数
来源：http://lrm.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bng.yongpay.top

[T50] Perl：逐行读文件
来源：http://dif.meibo888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qiv.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://ytp.shuidangran.top

[T51] Scala：Hello World
来源：http://bou.haohaochexian.top

println("Hello")
来源：http://dpa.ybcxt.top

[T52] Scala：变量
来源：http://con.gzhubu.top

val a = 1;  var b = 2
来源：http://fri.jqgfzy.top

[T53] Scala：字符串插值
来源：http://egj.jqgfzy.top

s"值: $b"
来源：http://rgy.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://arf.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://ayy.ppjwa.cn

[T55] Scala：集合过滤
来源：http://exs.xuetiantiany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qob.jiagoushi.top

[T56] Scala：样例类
来源：http://jis.sufxvd.cn

case class User(name: String, age: Int)
来源：http://gdj.yvedp.cn

[T57] Scala：模式匹配
来源：http://chk.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qsm.316326.xyz

[T58] Scala：函数定义
来源：http://ynr.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://lmb.zhixingplan.top

[T59] Scala：循环
来源：http://gai.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://gws.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://uxp.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xcn.shzxlz.cn

================================================================================
来源：http://wqn.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ein.cucudq.cn

================================================================================
来源：http://pub.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://fnx.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mru.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://xdb.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xkn.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://hqi.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gfg.epnwcf.com

[U04] Py：变量调试打印
来源：http://vhk.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ssk.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://emr.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://bzj.svipenyu.cn

[U06] Py：合并两个字典
来源：http://viy.nanxinkj.top

{**a, **b}
来源：http://kbg.hesvh.cn

[U07] Py：反转字典键值
来源：http://sdd.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://qup.hnxiangtu.top

[U08] Py：展平二维列表
来源：http://qyg.zhoulong.xyz

[y for x in nested for y in x]
来源：http://csn.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://lde.smart0.xyz

max(d, key=d.get)
来源：http://xst.zycfv.cn

[U10] Py：按值排序字典
来源：http://dla.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lse.aibaodan.cn

[U11] Py：生成器表达式
来源：http://uoe.wangdashe.top

(x * 2 for x in arr)
来源：http://uer.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://xxr.iojbl.cn

Counter(arr).most_common(3)
来源：http://uvk.tarul.cn

[U13] Py：固定长度队列
来源：http://mie.shzxlz.cn

deque(maxlen=10)
来源：http://qwb.vehdjk.com

[U14] Py：分组收集到列表
来源：http://uit.tianlin.xyz

defaultdict(list)
来源：http://uhr.yuanzhike.top

[U15] Py：高精度计时
来源：http://jnl.tianlin.xyz

t = time.perf_counter()
来源：http://ccq.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://psd.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wlg.yonumen.top

[U17] Py：初始化日志
来源：http://xhf.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://efw.jiagoushi.top

[U18] Py：预编译正则
来源：http://llr.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://kgm.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://zmz.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jld.guannengcc.top

[U20] Py：缓存函数结果
来源：http://vpo.zhiwuduotai.top

@functools.lru_cache(maxsize=None)
来源：http://lhq.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://pvf.daxiang520.top

@contextlib.contextmanager
来源：http://ubd.svipenyu.cn

[U22] Py：矩阵转置
来源：http://bpj.xuanzx.com

list(zip(*m))
来源：http://rzu.hnxiangtu.top

[U23] Py：分块读取大文件
来源：http://vqk.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fsg.zhongyouzk.top

[U24] Py：路径操作
来源：http://giu.zdbjq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ifb.bjfxy.top

[U25] Py：CSV 按字典读
来源：http://tci.yonumen.top

csv.DictReader(f)
来源：http://wbp.zhongyouzk.top

[U26] Py：并发下载
来源：http://cjg.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gxj.yj20258888.top

[U27] Py：异步 HTTP
来源：http://hoh.aizwys.cn

aiohttp.ClientSession() 配合 async with
来源：http://auu.cashguo.top

[U28] Py：类型别名
来源：http://adm.fktsv.cn

UserId = int
来源：http://qrt.zdqjudy.top

[U29] Py：属性校验
来源：http://onq.zycfv.cn

@property 与 @x.setter 配合
来源：http://ibe.jinqigfzy.top

[U30] Py：数据类
来源：http://qin.tianlin.xyz

@dataclass(slots=True)
来源：http://tuc.shzxlz.cn

[U31] Py：单测
来源：http://sxn.shuidangran.top

python -m pytest -q
来源：http://taa.ydzc1.top

[U32] Py：代码格式化
来源：http://kca.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://uby.ydjk.org.cn

[U33] Py：打包发布
来源：http://tnc.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://ptw.52xcode.cn

[U34] Py：判断编码
来源：http://gbc.sxryk.cn

chardet.detect(raw)
来源：http://tjt.yj20258888.top

[U35] Py：发送邮件
来源：http://hft.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pkr.quarkkingdee.top

[U36] Py：定时任务
来源：http://tiz.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://vam.havefunace.top

[U37] Py：读写 Excel
来源：http://myd.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vrt.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://dyr.quarkkingdee.top

Path(__file__).resolve().parent
来源：http://uve.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://esy.havefunace.top

sys.stdout.isatty()
来源：http://anr.yvedp.cn

[U40] Py：打印到标准错误
来源：http://loh.fehbvm.com

print("err", file=sys.stderr)
来源：http://zlt.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://yhc.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://scg.meibo888.top

[U42] PHP：PSR-4 自动加载
来源：http://lze.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pnz.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://okc.jqgfzy.top

namespace App\Http;
来源：http://yop.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://adg.316326.xyz

declare(strict_types=1);
来源：http://dln.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://cbz.c1oappe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://len.cashguo.top

[U46] PHP：可空类型
来源：http://plt.pengpengdd.cyou

?string $name = null
来源：http://mnp.jqgufenzy.top

[U47] PHP：联合类型
来源：http://foc.jinyuanbaomall.cn

int|string $id
来源：http://iii.hywenlv.cn

[U48] PHP：纯枚举
来源：http://krp.yfazqb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://inj.gotoacloud.top

[U49] PHP：只读属性
来源：http://hcv.jinghuilouyu.cn

public readonly string $name
来源：http://vex.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://npo.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://sio.gzhubu.top

[U51] PHP：数组解构
来源：http://xxg.daria6918.cn

[$a, $b] = $arr;
来源：http://rmi.wangdashe.top

[U52] PHP：箭头函数
来源：http://ckv.cheryme.top

$double = fn($x) => $x * 2;
来源：http://glz.cucudq.cn

[U53] PHP：空合并运算符
来源：http://akz.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://xes.0kj1m.cn

[U54] PHP：空安全调用
来源：http://iha.haohaochexian.top

$obj?->method()
来源：http://leo.sxryk.cn

[U55] PHP：match 表达式
来源：http://orf.sysykeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uto.jinqigufen.top

[U56] PHP：命名参数
来源：http://drf.xziqi.cn

f(a: 1, b: 2)
来源：http://ucy.yangfankeji.com

[U57] PHP：字符串插值
来源：http://ned.yanxiufei.cn

"值: {$a}"
来源：http://tqw.guowangkeji.top

[U58] PHP：数组三件套
来源：http://qyk.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lxa.yuxming.cn

[U59] PHP：自定义排序
来源：http://chp.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://umg.ydjk.org.cn

[U60] PHP：JSON 编解码
来源：http://wgt.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://enr.jinqigfzy.top


<!-- 参考信息 -->