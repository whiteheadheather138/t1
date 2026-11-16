代发 wailian999

[S37] C++：set
来源：http://aec.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://llg.sxryk.cn

[S38] C++：排序
来源：http://sgy.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://kzn.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://rjt.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://slk.daria6918.cn

[S40] C++：查找元素
来源：http://vuk.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wyh.epnwcf.com

[S41] C++：类与构造函数
来源：http://lyh.guannengcc.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wen.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://rzy.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://tva.jqgufenzy.top

[S43] C++：智能指针
来源：http://zuv.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://pgx.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://koe.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://dep.uphjek.com

[S45] C++：lambda
来源：http://kbj.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://ucg.quarkkingdee.top

[S46] C++：函数模板
来源：http://div.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hnt.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://sdb.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zob.yj202588.top

[S48] C++：逐行读文件
来源：http://wof.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ptm.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://tlw.0kj1m.cn

[S49] C++：写文件
来源：http://ylp.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hsv.hywenlv.cn

[S50] C++：格式化数字
来源：http://jxw.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ksq.gotoacloud.top

[S51] C++：显式类型转换
来源：http://psf.bjfxy.top

static_cast<double>(a) / b
来源：http://myl.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://rnd.gzhubu.top

int size() const noexcept { return n_; }
来源：http://yme.tarul.cn

[S53] C++：移动语义
来源：http://lmj.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://opq.birdmap.top

[S54] C++：异常处理
来源：http://wff.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://awc.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://sgx.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ljw.aizwys.cn

[S56] C++：optional
来源：http://cch.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xnr.c1oappe.top

[S57] C++：编译期常量
来源：http://ryb.ehwqpu.com

constexpr int N = 10;
来源：http://had.cqqwz.cn

[S58] C++：命名空间
来源：http://jmk.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://uju.yonumen.top

[S59] C++：静态断言
来源：http://oth.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zct.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://eik.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xif.bjfxy.top

================================================================================
来源：http://rzb.xuanzx.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uil.cucudq.cn

================================================================================
来源：http://wut.fzhhl.top

[T01] Kotlin：Hello World
来源：http://qlz.chenzaomai.com

println("Hello")
来源：http://ffs.chenlongwang.top

[T02] Kotlin：变量
来源：http://xqh.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ttv.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://mbi.shangyingyoupin.top

"值: $b"
来源：http://uvz.zdqjudy.top

[T04] Kotlin：空安全
来源：http://ewg.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://smz.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://dbg.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ysd.sysykeji.top

[T06] Kotlin：集合映射
来源：http://lcr.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cxz.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://dyo.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xgi.zdqjudy.top

[T08] Kotlin：数据类
来源：http://ngp.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://dwp.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://yyd.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://qof.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://auu.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xrb.ydzc1.top

[T11] Kotlin：协程
来源：http://vqu.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qlj.zycfv.cn

[T12] Kotlin：解构声明
来源：http://sav.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://lya.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://ofq.tarul.cn

val m = mapOf("a" to 1)
来源：http://usm.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://lpb.birdmap.top

for (i in 1..10) println(i)
来源：http://wvi.snrcjt.cn

[T15] Kotlin：接口
来源：http://ewd.meibo888.top

interface Shape { fun area(): Double }
来源：http://zgp.sjlbkw.cn

[T16] Swift：Hello World
来源：http://mdm.svipenyu.cn

print("Hello")
来源：http://upx.xinyue.icu

[T17] Swift：变量与常量
来源：http://brs.yanxiufei.cn

var a = 1;  let b = 2
来源：http://xbl.havefunace.top

[T18] Swift：字符串插值
来源：http://lge.yanxiufei.cn

"值: \(b)"
来源：http://yoo.xylfe.cn

[T19] Swift：可选绑定
来源：http://ktu.meibo888.top

if let n = opt { print(n) }
来源：http://vld.hammf.cn

[T20] Swift：数组操作
来源：http://lmf.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://ddy.xziqi.cn

[T21] Swift：遍历
来源：http://ybk.hammf.cn

for x in a { print(x) }
来源：http://umf.xuetiantiany.cn

[T22] Swift：字典
来源：http://fgj.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://dvd.jiagoushi.top

[T23] Swift：函数
来源：http://kbk.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lbv.sxryk.cn

[T24] Swift：闭包
来源：http://sfr.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://vda.redwolf501.top

[T25] Swift：结构体
来源：http://kyq.ydjk.org.cn

struct P { var x: Int }
来源：http://vqq.hnqzz.top

[T26] Swift：类与重写
来源：http://gpz.iojbl.cn

class A: Base { override func f() {} }
来源：http://pjx.cheryme.top

[T27] Swift：错误处理
来源：http://jio.sysykeji.top

do { try f() } catch { print(error) }
来源：http://skk.sysykeji.top

[T28] Swift：枚举
来源：http://rlk.chenlongwang.top

enum Color { case red, green }
来源：http://qyd.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://nzb.chenlongwang.top

guard let x = opt else { return }
来源：http://ynj.pycfn.com

[T30] Swift：协议
来源：http://ruq.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://fdm.tanke756.top

[T31] Lua：Hello World
来源：http://vhm.zhijiandao.cn

print("Hello")
来源：http://kxc.tian-w.cn

[T32] Lua：局部变量
来源：http://kxr.zycfv.cn

local a = 1
来源：http://hqd.iojbl.cn

[T33] Lua：表（数组）
来源：http://lrf.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://dpm.yvedp.cn

[T34] Lua：遍历表
来源：http://qbc.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zqi.sufxvd.cn

[T35] Lua：字典表
来源：http://xqz.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://zxb.xuanzx.com

[T36] Lua：函数
来源：http://syn.sysykeji.top

function add(a, b) return a + b end
来源：http://xbo.epnwcf.com

[T37] Lua：字符串拼接
来源：http://dga.yuxming.cn

"a" .. "b"
来源：http://jih.tarul.cn

[T38] Lua：条件
来源：http://rhl.kuanghao11.cn

if x > 0 then print("正") end
来源：http://vsn.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://wrk.fengsongda.top

string.find(s, "%d+")
来源：http://kop.jianghu66.top

[T40] Lua：元表
来源：http://cfn.andypj.xyz

setmetatable({}, { __index = base })
来源：http://imn.hywenlv.cn

[T41] Perl：Hello World
来源：http://fho.bjfxy.top

print "Hello\n";
来源：http://zve.shuidangran.top

[T42] Perl：变量类型
来源：http://lzp.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oqh.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://raf.tarul.cn

"值: $a"
来源：http://fnh.hywenlv.cn

[T44] Perl：条件
来源：http://jur.cqqwz.cn

if ($a > 0) { print "正"; }
来源：http://oai.cucudq.cn

[T45] Perl：数组遍历
来源：http://zjd.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://ieb.tian-w.cn

[T46] Perl：哈希操作
来源：http://yuw.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vef.pengpengdd.cyou

[T47] Perl：正则捕获
来源：http://jsp.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://cme.hcnkem.com

[T48] Perl：正则替换
来源：http://zfs.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://dvq.vehdjk.com

[T49] Perl：函数
来源：http://zcx.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sxt.chenjidiqi.icu

[T50] Perl：逐行读文件
来源：http://prx.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ete.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://cis.hcnkem.com

[T51] Scala：Hello World
来源：http://beq.zhaomingkeji.xyz

println("Hello")
来源：http://jmj.tianlin.xyz

[T52] Scala：变量
来源：http://ctd.xziqi.cn

val a = 1;  var b = 2
来源：http://eeu.wangdashe.top

[T53] Scala：字符串插值
来源：http://wwi.kuanghao11.cn

s"值: $b"
来源：http://kzo.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://qtc.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://dbw.yvedp.cn

[T55] Scala：集合过滤
来源：http://jxj.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mwc.ydzc1.top

[T56] Scala：样例类
来源：http://kuu.pengpengdd.cyou

case class User(name: String, age: Int)
来源：http://bmp.gotoacloud.top

[T57] Scala：模式匹配
来源：http://ksz.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cpt.52xcode.cn

[T58] Scala：函数定义
来源：http://vyb.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://ffv.jiagoushi.top

[T59] Scala：循环
来源：http://pmn.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://hdh.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://nfx.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tms.ppjwa.cn

================================================================================
来源：http://ikx.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kgt.hongshengwenyu.top

================================================================================
来源：http://vnt.sufxvd.cn

[U01] Py：创建虚拟环境
来源：http://cbz.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://bom.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://awc.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ftv.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://pwe.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dhj.vqdsnc.cn

[U04] Py：变量调试打印
来源：http://vyt.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rpk.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://ixi.cashguo.top

list(dict.fromkeys(arr))
来源：http://vrz.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://rwd.hywenlv.cn

{**a, **b}
来源：http://mmk.jianghu66.top

[U07] Py：反转字典键值
来源：http://lpt.yj20258888.top

{v: k for k, v in d.items()}
来源：http://lch.havefunace.top

[U08] Py：展平二维列表
来源：http://gjp.jinqigufen.top

[y for x in nested for y in x]
来源：http://vud.hammf.cn

[U09] Py：字典取最大值的键
来源：http://elg.cashguo.top

max(d, key=d.get)
来源：http://oic.gogol.net.cn

[U10] Py：按值排序字典
来源：http://duo.mhx1999.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kpo.cqqwz.cn

[U11] Py：生成器表达式
来源：http://yhi.tian-w.cn

(x * 2 for x in arr)
来源：http://swv.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nem.iojbl.cn

Counter(arr).most_common(3)
来源：http://gth.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://edc.jinqigfzy.top

deque(maxlen=10)
来源：http://etr.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://isz.jinyuanbaomall.cn

defaultdict(list)
来源：http://ihs.gaohongyu789.top

[U15] Py：高精度计时
来源：http://hia.yj20258.top

t = time.perf_counter()
来源：http://puh.jianghu66.top

[U16] Py：命令行参数解析
来源：http://ngg.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gli.hnqzz.top

[U17] Py：初始化日志
来源：http://hsc.ehwqpu.com

logging.basicConfig(level=logging.INFO)
来源：http://gmt.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://uvf.fktsv.cn

pat = re.compile(r"\d+")
来源：http://ysx.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://iuj.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jsw.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://kod.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://gkt.fehbvm.com

[U21] Py：自定义上下文管理器
来源：http://qbo.bjfxy.top

@contextlib.contextmanager
来源：http://hvm.tian-w.cn

[U22] Py：矩阵转置
来源：http://myu.yfazqb.com

list(zip(*m))
来源：http://ttk.wangdashe.top

[U23] Py：分块读取大文件
来源：http://dim.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://acu.316326.xyz

[U24] Py：路径操作
来源：http://cts.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jxb.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://ruj.vehdjk.com

csv.DictReader(f)
来源：http://agk.daxiang520.top

[U26] Py：并发下载
来源：http://qfm.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fna.feifeiyinyue.top

[U27] Py：异步 HTTP
来源：http://ctu.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://zka.chenlongwang.top

[U28] Py：类型别名
来源：http://vng.dashuyun.cn

UserId = int
来源：http://rvc.nanxinkj.top

[U29] Py：属性校验
来源：http://ydn.tanke756.top

@property 与 @x.setter 配合
来源：http://byc.smart0.xyz

[U30] Py：数据类
来源：http://mld.snrcjt.cn

@dataclass(slots=True)
来源：http://kjg.feifeiyinyue.top

[U31] Py：单测
来源：http://zyr.cqqwz.cn

python -m pytest -q
来源：http://ujs.aibaodan.cn

[U32] Py：代码格式化
来源：http://gug.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://xok.hesvh.cn

[U33] Py：打包发布
来源：http://amk.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://bha.snrcjt.cn

[U34] Py：判断编码
来源：http://kql.yongpay.top

chardet.detect(raw)
来源：http://xxw.jyoumei.cn

[U35] Py：发送邮件
来源：http://kuu.vehdjk.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vmp.tanke756.top

[U36] Py：定时任务
来源：http://zig.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://wej.sysykeji.top

[U37] Py：读写 Excel
来源：http://hem.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lsi.hongshengwenyu.top

[U38] Py：获取脚本所在目录
来源：http://mvk.cheryme.top

Path(__file__).resolve().parent
来源：http://zfo.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://pmw.gogol.net.cn

sys.stdout.isatty()
来源：http://lad.cdnleiting.top

[U40] Py：打印到标准错误
来源：http://daz.gogol.net.cn

print("err", file=sys.stderr)
来源：http://xkm.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://nun.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://edr.yfazqb.com

[U42] PHP：PSR-4 自动加载
来源：http://pce.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ljl.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://lgx.bbcook.cn

namespace App\Http;
来源：http://fsv.mhx1999.top

[U44] PHP：开启严格类型
来源：http://daw.sjlbkw.cn

declare(strict_types=1);
来源：http://uze.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://fuh.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wxa.zhengqikj.top

[U46] PHP：可空类型
来源：http://ylx.guannengcc.top

?string $name = null
来源：http://ahk.gogol.net.cn

[U47] PHP：联合类型
来源：http://tfb.mhx1999.top

int|string $id
来源：http://xxm.316326.xyz

[U48] PHP：纯枚举
来源：http://hxz.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nwf.havefunace.top

[U49] PHP：只读属性
来源：http://pql.nanxinkj.top

public readonly string $name
来源：http://auw.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://oex.daria6918.cn

public function __construct(private int $id) {}
来源：http://zfg.cqqwz.cn

[U51] PHP：数组解构
来源：http://zfd.mhx1999.top

[$a, $b] = $arr;
来源：http://fth.hysaishi.cn

[U52] PHP：箭头函数
来源：http://pha.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://wln.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://mon.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://qlj.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://rlm.fzhhl.top

$obj?->method()
来源：http://tge.hnqzz.top

[U55] PHP：match 表达式
来源：http://ogx.yj202588.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fvs.birdmap.top

[U56] PHP：命名参数
来源：http://azk.zhixingplan.top

f(a: 1, b: 2)
来源：http://slt.xylfe.cn

[U57] PHP：字符串插值
来源：http://zml.jqgfzy.top

"值: {$a}"
来源：http://hag.birdmap.top

[U58] PHP：数组三件套
来源：http://ujs.hysaishi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qaq.yuxming.cn

[U59] PHP：自定义排序
来源：http://hiq.gzhubu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ygt.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://aam.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xmf.yangfankeji.com

[U61] PHP：正则
来源：http://qiw.dashuyun.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pxp.jianghu66.top

[U62] PHP：日期对象
来源：http://xfm.zhengqikj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qtg.fanxiaobao.xyz


<!-- 参考信息 -->