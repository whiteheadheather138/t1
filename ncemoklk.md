代发 wailian999

[S39] C++：自定义比较器排序
来源：http://ugy.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://juz.ydjk.org.cn

[S40] C++：查找元素
来源：http://zfa.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zov.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://chj.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nqv.yj20258.top

[S42] C++：继承与虚函数
来源：http://wjg.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://dcq.hnqzz.top

[S43] C++：智能指针
来源：http://sml.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://ega.sufxvd.cn

[S44] C++：引用传参
来源：http://cdo.daria6918.cn

void inc(int &x) { ++x; }
来源：http://ays.zdqjudy.top

[S45] C++：lambda
来源：http://nye.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://qdb.xylfe.cn

[S46] C++：函数模板
来源：http://lsk.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kgk.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://cik.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ptd.0kj1m.cn

[S48] C++：逐行读文件
来源：http://fpd.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://snv.fzhhl.top

while (std::getline(in, line)) { }
来源：http://nkq.svipenyu.cn

[S49] C++：写文件
来源：http://ryv.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wjg.cqqwz.cn

[S50] C++：格式化数字
来源：http://juq.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cvi.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://jkg.hywenlv.cn

static_cast<double>(a) / b
来源：http://aws.yonumen.top

[S52] C++：const 与 noexcept
来源：http://ied.birdmap.top

int size() const noexcept { return n_; }
来源：http://osx.zhoulong.xyz

[S53] C++：移动语义
来源：http://sda.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://sgb.yuanzhike.top

[S54] C++：异常处理
来源：http://mft.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dbu.c1oappe.top

[S55] C++：结构化绑定
来源：http://ukt.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bgm.bjfxy.top

[S56] C++：optional
来源：http://kpm.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ilz.hfpthk.cn

[S57] C++：编译期常量
来源：http://osj.havefunace.top

constexpr int N = 10;
来源：http://kej.cdnleiting.top

[S58] C++：命名空间
来源：http://mjx.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://ptm.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://qhz.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://awn.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://igc.uphjek.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://byp.tanke756.top

================================================================================
来源：http://dts.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ekf.meibo888.top

================================================================================
来源：http://hvu.c1oappe.top

[T01] Kotlin：Hello World
来源：http://yrn.hammf.cn

println("Hello")
来源：http://plo.bbcook.cn

[T02] Kotlin：变量
来源：http://wfm.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fyd.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://rpz.hcnkem.com

"值: $b"
来源：http://rbx.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://qnw.jqgfzy.top

val n: String? = null;  n?.length
来源：http://fzl.pycfn.com

[T05] Kotlin：when 表达式
来源：http://ygn.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sth.yj20258888.top

[T06] Kotlin：集合映射
来源：http://zst.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xbn.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://taa.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://qqt.fehbvm.com

[T08] Kotlin：数据类
来源：http://typ.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://ugp.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://fhk.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://nao.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://gpa.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://enq.yuxming.cn

[T11] Kotlin：协程
来源：http://nov.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nzl.fanxiaobao.xyz

[T12] Kotlin：解构声明
来源：http://gzq.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://ghe.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://hsc.tanke756.top

val m = mapOf("a" to 1)
来源：http://vqp.sxryk.cn

[T14] Kotlin：循环
来源：http://hhh.sufxvd.cn

for (i in 1..10) println(i)
来源：http://cer.c1oappe.top

[T15] Kotlin：接口
来源：http://kzq.daria6918.cn

interface Shape { fun area(): Double }
来源：http://hir.birdmap.top

[T16] Swift：Hello World
来源：http://prz.ehwqpu.com

print("Hello")
来源：http://puf.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://evz.iojbl.cn

var a = 1;  let b = 2
来源：http://ifr.ivvv.top

[T18] Swift：字符串插值
来源：http://pve.hywenlv.cn

"值: \(b)"
来源：http://bhb.shzxlz.cn

[T19] Swift：可选绑定
来源：http://qmh.fzhhl.top

if let n = opt { print(n) }
来源：http://oyn.guannengcc.top

[T20] Swift：数组操作
来源：http://tyn.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kne.hnqzz.top

[T21] Swift：遍历
来源：http://bsf.redwolf501.top

for x in a { print(x) }
来源：http://wbc.xinyue.icu

[T22] Swift：字典
来源：http://yxs.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://lfw.c1oappe.top

[T23] Swift：函数
来源：http://gbq.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jrq.daxiang520.top

[T24] Swift：闭包
来源：http://jnd.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sat.ydjk.org.cn

[T25] Swift：结构体
来源：http://yfk.zhengqikj.top

struct P { var x: Int }
来源：http://hiw.nanxuanxn.top

[T26] Swift：类与重写
来源：http://fcm.tianlin.xyz

class A: Base { override func f() {} }
来源：http://yky.cashguo.top

[T27] Swift：错误处理
来源：http://xmz.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://uvo.yuanzhike.top

[T28] Swift：枚举
来源：http://fgn.yj20258.top

enum Color { case red, green }
来源：http://dbq.tarul.cn

[T29] Swift：guard 提前返回
来源：http://hgs.aibaodan.cn

guard let x = opt else { return }
来源：http://sbp.zdqjudy.top

[T30] Swift：协议
来源：http://wzg.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://guz.jlsjyb.cn

[T31] Lua：Hello World
来源：http://nva.cucudq.cn

print("Hello")
来源：http://sta.hesvh.cn

[T32] Lua：局部变量
来源：http://nna.yueranfly.top

local a = 1
来源：http://npw.jianghu66.top

[T33] Lua：表（数组）
来源：http://eeh.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://oan.shuidangran.top

[T34] Lua：遍历表
来源：http://yio.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nzh.quarkkingdee.top

[T35] Lua：字典表
来源：http://pnp.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://nym.aibaodan.cn

[T36] Lua：函数
来源：http://qor.uphjek.com

function add(a, b) return a + b end
来源：http://eik.cucudq.cn

[T37] Lua：字符串拼接
来源：http://ehd.ctjpmb.com

"a" .. "b"
来源：http://bwd.ydjk.org.cn

[T38] Lua：条件
来源：http://exa.zhiwuduotai.top

if x > 0 then print("正") end
来源：http://uef.jyoumei.cn

[T39] Lua：模式匹配
来源：http://mxm.xylfe.cn

string.find(s, "%d+")
来源：http://pnj.hcnkem.com

[T40] Lua：元表
来源：http://eih.birdmap.top

setmetatable({}, { __index = base })
来源：http://mqb.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://mxe.cucudq.cn

print "Hello\n";
来源：http://ozy.yanxiufei.cn

[T42] Perl：变量类型
来源：http://hxy.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bpm.dashuyun.cn

[T43] Perl：字符串插值
来源：http://mrs.hammf.cn

"值: $a"
来源：http://uhr.jqgufenzy.top

[T44] Perl：条件
来源：http://cnp.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://yuf.haohaochexian.top

[T45] Perl：数组遍历
来源：http://ccl.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://mhr.nwbrower.top

[T46] Perl：哈希操作
来源：http://wes.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://egy.yueranfly.top

[T47] Perl：正则捕获
来源：http://kmg.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hdl.gzhubu.top

[T48] Perl：正则替换
来源：http://ukd.bbcook.cn

$s =~ s/old/new/g;
来源：http://kwb.fehbvm.com

[T49] Perl：函数
来源：http://yly.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ttu.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://niu.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ioi.gaohongyu789.top

while (my $line = <$fh>) { print $line; }
来源：http://zcl.aibaodan.cn

[T51] Scala：Hello World
来源：http://scn.shanyushiyangtech.top

println("Hello")
来源：http://way.yongpay.top

[T52] Scala：变量
来源：http://edj.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://uxg.hywenlv.cn

[T53] Scala：字符串插值
来源：http://dkg.jqgfzy.top

s"值: $b"
来源：http://ikf.yangfankeji.com

[T54] Scala：集合映射
来源：http://roz.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://iqx.zdqjudy.top

[T55] Scala：集合过滤
来源：http://ngk.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://kxf.0kj1m.cn

[T56] Scala：样例类
来源：http://wfc.ywan-chungtsiang.top

case class User(name: String, age: Int)
来源：http://egk.redwolf501.top

[T57] Scala：模式匹配
来源：http://mmk.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yfh.yongpay.top

[T58] Scala：函数定义
来源：http://yra.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://zqi.andypj.xyz

[T59] Scala：循环
来源：http://hwm.yonumen.top

for (i <- 1 to 10) println(i)
来源：http://bop.gogol.net.cn

[T60] Scala：折叠
来源：http://gdq.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hhv.cqqwz.cn

================================================================================
来源：http://bky.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xog.zhiwuduotai.top

================================================================================
来源：http://zqv.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://ywd.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aae.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://ahc.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://swf.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://xyv.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sso.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://wzx.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tfj.uphjek.com

[U05] Py：列表去重且保序
来源：http://okk.epnwcf.com

list(dict.fromkeys(arr))
来源：http://tjz.yvedp.cn

[U06] Py：合并两个字典
来源：http://qne.xinyue.icu

{**a, **b}
来源：http://sdz.birdmap.top

[U07] Py：反转字典键值
来源：http://kzw.cdnleiting.top

{v: k for k, v in d.items()}
来源：http://kjv.cashguo.top

[U08] Py：展平二维列表
来源：http://xda.xylfe.cn

[y for x in nested for y in x]
来源：http://fgx.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://ytg.svipenyu.cn

max(d, key=d.get)
来源：http://skf.iojbl.cn

[U10] Py：按值排序字典
来源：http://rtf.shanyushiyangtech.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://miv.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://nug.jqgfzy.top

(x * 2 for x in arr)
来源：http://fak.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://uii.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://wwi.xinyue.icu

[U13] Py：固定长度队列
来源：http://nft.fzhhl.top

deque(maxlen=10)
来源：http://khq.sysykeji.top

[U14] Py：分组收集到列表
来源：http://roj.yfazqb.com

defaultdict(list)
来源：http://cdo.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://fno.fktsv.cn

t = time.perf_counter()
来源：http://jvp.yj202588.top

[U16] Py：命令行参数解析
来源：http://bxv.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zlz.yfazqb.com

[U17] Py：初始化日志
来源：http://yro.feifeiyinyue.top

logging.basicConfig(level=logging.INFO)
来源：http://fwl.aibaodan.cn

[U18] Py：预编译正则
来源：http://ryx.vehdjk.com

pat = re.compile(r"\d+")
来源：http://rrj.hnxiangtu.top

[U19] Py：正则替换带回调
来源：http://qyx.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vru.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://oyd.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://ckh.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://qoq.yangfankeji.com

@contextlib.contextmanager
来源：http://dal.tianlin.xyz

[U22] Py：矩阵转置
来源：http://xew.zhongyouzk.top

list(zip(*m))
来源：http://ysw.zdqjudy.top

[U23] Py：分块读取大文件
来源：http://frf.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://inb.zdbjq.cn

[U24] Py：路径操作
来源：http://ptr.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iik.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://jen.hnxiangtu.top

csv.DictReader(f)
来源：http://jbe.wangshuangyany.cn

[U26] Py：并发下载
来源：http://aaq.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://emu.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://unp.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://hta.ydjk.org.cn

[U28] Py：类型别名
来源：http://mlh.fanxiaobao.xyz

UserId = int
来源：http://ykl.cucudq.cn

[U29] Py：属性校验
来源：http://uqb.aibaodan.cn

@property 与 @x.setter 配合
来源：http://lfk.nanxuanxn.top

[U30] Py：数据类
来源：http://pyz.gaohongyu789.top

@dataclass(slots=True)
来源：http://qme.shuidangran.top

[U31] Py：单测
来源：http://ant.redwolf501.top

python -m pytest -q
来源：http://tzo.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://pcx.tarul.cn

ruff format . && ruff check --fix .
来源：http://ucu.gzhubu.top

[U33] Py：打包发布
来源：http://vtr.tarul.cn

python -m build  （依赖 pyproject.toml）
来源：http://unu.cashguo.top

[U34] Py：判断编码
来源：http://rvq.meibo888.top

chardet.detect(raw)
来源：http://bzq.zdqjudy.top

[U35] Py：发送邮件
来源：http://xgf.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zxw.hongshengwenyu.top

[U36] Py：定时任务
来源：http://cae.jinyuanbaomall.cn

schedule.every(10).minutes.do(job)
来源：http://fga.zhixingplan.top

[U37] Py：读写 Excel
来源：http://ntv.chenlongwang.top

pandas.read_excel / DataFrame.to_excel
来源：http://pie.shzxlz.cn

[U38] Py：获取脚本所在目录
来源：http://ewk.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://kvb.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://njy.tanke756.top

sys.stdout.isatty()
来源：http://zzb.9152youxi.cn

[U40] Py：打印到标准错误
来源：http://jya.fktsv.cn

print("err", file=sys.stderr)
来源：http://wtx.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://qvn.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://new.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://zqi.jinqigufen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tjz.nanxinkj.top

[U43] PHP：声明命名空间
来源：http://pym.hywenlv.cn

namespace App\Http;
来源：http://wyu.zhongyouzk.top

[U44] PHP：开启严格类型
来源：http://lkj.yfazqb.com

declare(strict_types=1);
来源：http://loh.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://ojp.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xlm.chenzaomai.com

[U46] PHP：可空类型
来源：http://nxk.yvedp.cn

?string $name = null
来源：http://ppw.vehdjk.com

[U47] PHP：联合类型
来源：http://yjp.daria6918.cn

int|string $id
来源：http://vie.ivvv.top

[U48] PHP：纯枚举
来源：http://hnh.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lie.gzhubu.top

[U49] PHP：只读属性
来源：http://gxk.wangdashe.top

public readonly string $name
来源：http://ctf.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://tcj.nwbrower.top

public function __construct(private int $id) {}
来源：http://xei.daria6918.cn

[U51] PHP：数组解构
来源：http://dea.fengsongda.top

[$a, $b] = $arr;
来源：http://bgx.zdqjudy.top

[U52] PHP：箭头函数
来源：http://rpr.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://nbk.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://ouy.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://bva.nanxinkj.top

[U54] PHP：空安全调用
来源：http://kqb.jinqigfzy.top

$obj?->method()
来源：http://tgm.shuidangran.top

[U55] PHP：match 表达式
来源：http://jxu.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rpe.haohaochexian.top

[U56] PHP：命名参数
来源：http://dxs.zdbjq.cn

f(a: 1, b: 2)
来源：http://blu.iojbl.cn

[U57] PHP：字符串插值
来源：http://orb.cdnleiting.top

"值: {$a}"
来源：http://grz.ctjpmb.com

[U58] PHP：数组三件套
来源：http://udl.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jns.yonumen.top

[U59] PHP：自定义排序
来源：http://erm.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://inq.vehdjk.com

[U60] PHP：JSON 编解码
来源：http://dmk.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wmp.xziqi.cn

[U61] PHP：正则
来源：http://sxu.chenlongwang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://enw.aizwys.cn

[U62] PHP：日期对象
来源：http://dep.tanke756.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pad.zhijiandao.cn

[U63] PHP：文件读写
来源：http://ueq.jyoumei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nsw.fktsv.cn

[U64] PHP：目录遍历
来源：http://svf.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://hpv.hesvh.cn


<!-- 参考信息 -->