代发 wailian999

[S39] C++：自定义比较器排序
来源：http://wtv.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://trp.ehwqpu.com

[S40] C++：查找元素
来源：http://jlj.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cma.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://upt.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ajg.epnwcf.com

[S42] C++：继承与虚函数
来源：http://ect.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://dtr.feifeiyinyue.top

[S43] C++：智能指针
来源：http://avu.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://sxu.shuidangran.top

[S44] C++：引用传参
来源：http://tdk.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://mtk.shanyushiyangtech.top

[S45] C++：lambda
来源：http://aho.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fde.hnxiangtu.top

[S46] C++：函数模板
来源：http://hwy.ivvv.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kmt.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://lyh.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iat.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://nlu.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lws.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://ktz.quarkkingdee.top

[S49] C++：写文件
来源：http://qlw.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://thy.cucudq.cn

[S50] C++：格式化数字
来源：http://sei.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://toh.andypj.xyz

[S51] C++：显式类型转换
来源：http://ibg.guowangkeji.top

static_cast<double>(a) / b
来源：http://vfi.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://abj.chenjidiqi.icu

int size() const noexcept { return n_; }
来源：http://vhd.mhx1999.top

[S53] C++：移动语义
来源：http://fss.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://qgi.fktsv.cn

[S54] C++：异常处理
来源：http://bxp.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fkc.jiagoushi.top

[S55] C++：结构化绑定
来源：http://vab.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cvh.tarul.cn

[S56] C++：optional
来源：http://tel.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dsv.yanxiufei.cn

[S57] C++：编译期常量
来源：http://rjj.zycfv.cn

constexpr int N = 10;
来源：http://clf.tarul.cn

[S58] C++：命名空间
来源：http://jym.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://ibs.tanke756.top

[S59] C++：静态断言
来源：http://vdl.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zir.pycfn.com

[S60] C++：遍历并删除元素
来源：http://rvk.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kwp.yvedp.cn

================================================================================
来源：http://ckz.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://drm.sxryk.cn

================================================================================
来源：http://smj.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://qtq.yvedp.cn

println("Hello")
来源：http://abh.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://exk.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nto.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://vfh.yj202588.top

"值: $b"
来源：http://pbs.uphjek.com

[T04] Kotlin：空安全
来源：http://qvj.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://mxx.ivvv.top

[T05] Kotlin：when 表达式
来源：http://ymi.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jgk.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://rfc.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lfg.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://gkl.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://gmk.hnqzz.top

[T08] Kotlin：数据类
来源：http://dhk.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://awk.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://bmi.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://kqg.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://ckv.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://tko.bbcook.cn

[T11] Kotlin：协程
来源：http://uin.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nvg.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://tof.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://mmc.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://uyr.jianghu66.top

val m = mapOf("a" to 1)
来源：http://ndv.fehbvm.com

[T14] Kotlin：循环
来源：http://inr.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://chr.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://ysx.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://jmj.yanxiufei.cn

[T16] Swift：Hello World
来源：http://jkn.jianghu66.top

print("Hello")
来源：http://fki.wangdashe.top

[T17] Swift：变量与常量
来源：http://hnn.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://ave.sysykeji.top

[T18] Swift：字符串插值
来源：http://ddq.jinghuilouyu.cn

"值: \(b)"
来源：http://axk.shzxlz.cn

[T19] Swift：可选绑定
来源：http://vbc.xinyue.icu

if let n = opt { print(n) }
来源：http://drp.quarkkingdee.top

[T20] Swift：数组操作
来源：http://ael.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kvh.ivvv.top

[T21] Swift：遍历
来源：http://ygb.zhengqikj.top

for x in a { print(x) }
来源：http://rmd.sjlbkw.cn

[T22] Swift：字典
来源：http://ccg.birdmap.top

var d = ["a": 1];  d["b"] = 2
来源：http://vzk.jqgufenzy.top

[T23] Swift：函数
来源：http://qyk.yongpay.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://noq.fktsv.cn

[T24] Swift：闭包
来源：http://trc.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gpl.haohaochexian.top

[T25] Swift：结构体
来源：http://hjw.zhixingplan.top

struct P { var x: Int }
来源：http://eqb.316326.xyz

[T26] Swift：类与重写
来源：http://prt.sweek.top

class A: Base { override func f() {} }
来源：http://ijx.sjlbkw.cn

[T27] Swift：错误处理
来源：http://ftd.yuxming.cn

do { try f() } catch { print(error) }
来源：http://slz.fktsv.cn

[T28] Swift：枚举
来源：http://ita.wangdashe.top

enum Color { case red, green }
来源：http://uat.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://ugo.aizwys.cn

guard let x = opt else { return }
来源：http://zhu.fengsongda.top

[T30] Swift：协议
来源：http://eae.cheryme.top

protocol Shape { func area() -> Double }
来源：http://lqe.guannengcc.top

[T31] Lua：Hello World
来源：http://nsb.316326.xyz

print("Hello")
来源：http://xkt.pycfn.com

[T32] Lua：局部变量
来源：http://jlo.nwbrower.top

local a = 1
来源：http://kuk.shuidangran.top

[T33] Lua：表（数组）
来源：http://qay.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dnj.shzxlz.cn

[T34] Lua：遍历表
来源：http://usk.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xxi.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://mjh.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://dtr.fzhhl.top

[T36] Lua：函数
来源：http://cia.316326.xyz

function add(a, b) return a + b end
来源：http://leu.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://qxg.shzxlz.cn

"a" .. "b"
来源：http://mxd.fehbvm.com

[T38] Lua：条件
来源：http://mje.chenzaomai.com

if x > 0 then print("正") end
来源：http://vou.yj20258888.top

[T39] Lua：模式匹配
来源：http://ndu.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://vpf.jqgufenzy.top

[T40] Lua：元表
来源：http://ixo.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://swl.kuanghao11.cn

[T41] Perl：Hello World
来源：http://nuq.sjlbkw.cn

print "Hello\n";
来源：http://xds.ctjpmb.com

[T42] Perl：变量类型
来源：http://vad.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xqs.hcnkem.com

[T43] Perl：字符串插值
来源：http://mja.xinyue.icu

"值: $a"
来源：http://dav.dianchejie.cn

[T44] Perl：条件
来源：http://apr.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://xcp.mhx1999.top

[T45] Perl：数组遍历
来源：http://ohy.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://lhc.yvedp.cn

[T46] Perl：哈希操作
来源：http://pkg.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://irv.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://fmz.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vvf.chenzaomai.com

[T48] Perl：正则替换
来源：http://hne.jiagoushi.top

$s =~ s/old/new/g;
来源：http://jqd.vehdjk.com

[T49] Perl：函数
来源：http://jog.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://std.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://fzj.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vbr.haohaochexian.top

while (my $line = <$fh>) { print $line; }
来源：http://aui.sysykeji.top

[T51] Scala：Hello World
来源：http://ysv.aibaodan.cn

println("Hello")
来源：http://ajq.gogol.net.cn

[T52] Scala：变量
来源：http://ljr.zhongyouzk.top

val a = 1;  var b = 2
来源：http://yir.ehwqpu.com

[T53] Scala：字符串插值
来源：http://bho.smart0.xyz

s"值: $b"
来源：http://zqq.hammf.cn

[T54] Scala：集合映射
来源：http://fih.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://foi.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://bwu.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yzi.yj20258888.top

[T56] Scala：样例类
来源：http://qer.redwolf501.top

case class User(name: String, age: Int)
来源：http://tpb.cqqwz.cn

[T57] Scala：模式匹配
来源：http://fmw.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dzt.fehbvm.com

[T58] Scala：函数定义
来源：http://mer.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://vly.hesvh.cn

[T59] Scala：循环
来源：http://vml.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://tbw.yonumen.top

[T60] Scala：折叠
来源：http://tvl.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://umt.shzxlz.cn

================================================================================
来源：http://qtm.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dla.chenlongwang.top

================================================================================
来源：http://cal.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://mez.sjlbkw.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cnx.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://fzy.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sec.tanke756.top

[U03] Py：加载 .env 配置
来源：http://ahn.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nhh.smart0.xyz

[U04] Py：变量调试打印
来源：http://cug.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://adq.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://sgi.sweek.top

list(dict.fromkeys(arr))
来源：http://ciz.jqgfzy.top

[U06] Py：合并两个字典
来源：http://prt.fanxiaobao.xyz

{**a, **b}
来源：http://bmc.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://vct.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://wjd.hnqzz.top

[U08] Py：展平二维列表
来源：http://cnk.cqqwz.cn

[y for x in nested for y in x]
来源：http://cfx.tarul.cn

[U09] Py：字典取最大值的键
来源：http://jml.smart0.xyz

max(d, key=d.get)
来源：http://aqz.shuidangran.top

[U10] Py：按值排序字典
来源：http://hkh.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cne.jinqigufen.top

[U11] Py：生成器表达式
来源：http://hsm.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://bfs.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zud.jianghu66.top

Counter(arr).most_common(3)
来源：http://lec.tanke756.top

[U13] Py：固定长度队列
来源：http://eyc.cucudq.cn

deque(maxlen=10)
来源：http://qhm.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://wep.shanyushiyangkeji.top

defaultdict(list)
来源：http://rqz.xylfe.cn

[U15] Py：高精度计时
来源：http://von.uphjek.com

t = time.perf_counter()
来源：http://isa.hesvh.cn

[U16] Py：命令行参数解析
来源：http://hdz.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ecm.yanxiufei.cn

[U17] Py：初始化日志
来源：http://iuk.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://ukh.52xcode.cn

[U18] Py：预编译正则
来源：http://gus.xziqi.cn

pat = re.compile(r"\d+")
来源：http://fwa.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://xze.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ziy.ydzc1.top

[U20] Py：缓存函数结果
来源：http://esq.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://dga.zhiwuduotai.top

[U21] Py：自定义上下文管理器
来源：http://ovy.tianlin.xyz

@contextlib.contextmanager
来源：http://juw.shzxlz.cn

[U22] Py：矩阵转置
来源：http://zrx.zhixingplan.top

list(zip(*m))
来源：http://kvd.cheryme.top

[U23] Py：分块读取大文件
来源：http://zry.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://azc.shzxlz.cn

[U24] Py：路径操作
来源：http://boo.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dli.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://mjh.chenjidiqi.icu

csv.DictReader(f)
来源：http://iov.daria6918.cn

[U26] Py：并发下载
来源：http://pso.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://acb.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://vzy.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://rmp.jqgfzy.top

[U28] Py：类型别名
来源：http://bql.vqdsnc.cn

UserId = int
来源：http://pvn.fengsongda.top

[U29] Py：属性校验
来源：http://lio.jlsjyb.cn

@property 与 @x.setter 配合
来源：http://qbe.smart0.xyz

[U30] Py：数据类
来源：http://bfc.guannengcc.top

@dataclass(slots=True)
来源：http://mjv.tanke756.top

[U31] Py：单测
来源：http://kum.ppjwa.cn

python -m pytest -q
来源：http://lxl.snrcjt.cn

[U32] Py：代码格式化
来源：http://ben.dianchejie.cn

ruff format . && ruff check --fix .
来源：http://bny.gogol.net.cn

[U33] Py：打包发布
来源：http://ccw.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://ggh.aizwys.cn

[U34] Py：判断编码
来源：http://ygf.yvedp.cn

chardet.detect(raw)
来源：http://fak.birdmap.top

[U35] Py：发送邮件
来源：http://xzp.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kcn.vehdjk.com

[U36] Py：定时任务
来源：http://zki.nanxuanxn.top

schedule.every(10).minutes.do(job)
来源：http://pcy.epnwcf.com

[U37] Py：读写 Excel
来源：http://yze.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wlc.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://xkz.nanxinkj.top

Path(__file__).resolve().parent
来源：http://wnu.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://bdi.fzhhl.top

sys.stdout.isatty()
来源：http://tyn.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://psy.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://wrh.nwbrower.top

[U41] PHP：初始化 Composer 项目
来源：http://zhj.jinqigfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bjb.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://fjn.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yqw.sxryk.cn

[U43] PHP：声明命名空间
来源：http://vnk.bjfxy.top

namespace App\Http;
来源：http://mvh.tanke756.top

[U44] PHP：开启严格类型
来源：http://ugf.hesvh.cn

declare(strict_types=1);
来源：http://zha.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://wno.shuidangran.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pec.yj202588.top

[U46] PHP：可空类型
来源：http://nbb.ywan-chungtsiang.top

?string $name = null
来源：http://hgr.wangshuangyany.cn

[U47] PHP：联合类型
来源：http://bgw.havefunace.top

int|string $id
来源：http://kud.cdnleiting.top

[U48] PHP：纯枚举
来源：http://xhd.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dpx.nanxuanxn.top

[U49] PHP：只读属性
来源：http://tkp.yuanzhike.top

public readonly string $name
来源：http://jsv.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://dyb.meibo888.top

public function __construct(private int $id) {}
来源：http://xco.ppjwa.cn

[U51] PHP：数组解构
来源：http://rnn.shzxlz.cn

[$a, $b] = $arr;
来源：http://wya.aizwys.cn

[U52] PHP：箭头函数
来源：http://bqw.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://irc.jianghu66.top

[U53] PHP：空合并运算符
来源：http://jzr.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://kke.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://bmc.xinyue.icu

$obj?->method()
来源：http://fcs.nanxinkj.top

[U55] PHP：match 表达式
来源：http://lof.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hki.birdmap.top

[U56] PHP：命名参数
来源：http://urc.yonumen.top

f(a: 1, b: 2)
来源：http://bpq.cucudq.cn

[U57] PHP：字符串插值
来源：http://bnp.fktsv.cn

"值: {$a}"
来源：http://waq.cheryme.top

[U58] PHP：数组三件套
来源：http://jwr.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wsv.nanxinkj.top

[U59] PHP：自定义排序
来源：http://qgf.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cvz.fzhhl.top

[U60] PHP：JSON 编解码
来源：http://edq.c1oappe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vhr.nwbrower.top

[U61] PHP：正则
来源：http://aet.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://crk.hesvh.cn

[U62] PHP：日期对象
来源：http://lhc.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fss.yj20258888.top

[U63] PHP：文件读写
来源：http://oow.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dqj.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://uvl.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://wdf.zhoulong.xyz


<!-- 参考信息 -->