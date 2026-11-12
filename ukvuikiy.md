代发 wailian999

[S41] C++：类与构造函数
来源：http://mpv.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iip.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://hpg.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://mtg.gogol.net.cn

[S43] C++：智能指针
来源：http://vol.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://dqu.ppjwa.cn

[S44] C++：引用传参
来源：http://uco.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://edw.bbcook.cn

[S45] C++：lambda
来源：http://bdm.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://weu.dashuyun.cn

[S46] C++：函数模板
来源：http://eqb.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bxh.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://ukg.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dkg.xylfe.cn

[S48] C++：逐行读文件
来源：http://hlf.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uye.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://nup.nanxuanxn.top

[S49] C++：写文件
来源：http://baf.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pif.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://edw.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dwt.316326.xyz

[S51] C++：显式类型转换
来源：http://igm.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://vcz.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://qik.hcnkem.com

int size() const noexcept { return n_; }
来源：http://ptv.hnqzz.top

[S53] C++：移动语义
来源：http://ifl.birdmap.top

std::vector<int> w = std::move(v);
来源：http://xef.nwbrower.top

[S54] C++：异常处理
来源：http://waq.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aii.zhixingplan.top

[S55] C++：结构化绑定
来源：http://chu.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yeu.sufxvd.cn

[S56] C++：optional
来源：http://fyw.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qqz.cqqwz.cn

[S57] C++：编译期常量
来源：http://icb.zdqjudy.top

constexpr int N = 10;
来源：http://xve.yongpay.top

[S58] C++：命名空间
来源：http://rsk.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://uyj.jqgfzy.top

[S59] C++：静态断言
来源：http://qma.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jtb.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://cem.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ypq.ctjpmb.com

================================================================================
来源：http://gmz.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vti.epnwcf.com

================================================================================
来源：http://nld.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://oju.ybcxt.top

println("Hello")
来源：http://znk.yj20258.top

[T02] Kotlin：变量
来源：http://wzo.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fxl.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://fmy.zhixingplan.top

"值: $b"
来源：http://mrg.tanke756.top

[T04] Kotlin：空安全
来源：http://fwi.ehwqpu.com

val n: String? = null;  n?.length
来源：http://ugp.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://sgp.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wlp.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://mra.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://cqh.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://ajw.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jez.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://iwd.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://xus.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://vbs.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://fel.fengsongda.top

[T10] Kotlin：默认参数
来源：http://lfm.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qpi.epnwcf.com

[T11] Kotlin：协程
来源：http://arb.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fbq.nwbrower.top

[T12] Kotlin：解构声明
来源：http://kjz.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://ufq.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://ucb.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://hdr.hywenlv.cn

[T14] Kotlin：循环
来源：http://boc.jinqigufen.top

for (i in 1..10) println(i)
来源：http://njt.zhengqikj.top

[T15] Kotlin：接口
来源：http://vtg.hammf.cn

interface Shape { fun area(): Double }
来源：http://xjs.zhongyouzk.top

[T16] Swift：Hello World
来源：http://uxq.yj20258.top

print("Hello")
来源：http://cvm.jinqigufen.top

[T17] Swift：变量与常量
来源：http://zsg.hysaishi.cn

var a = 1;  let b = 2
来源：http://vwg.xziqi.cn

[T18] Swift：字符串插值
来源：http://lxi.wangdashe.top

"值: \(b)"
来源：http://emw.bjfxy.top

[T19] Swift：可选绑定
来源：http://thc.zdqjudy.top

if let n = opt { print(n) }
来源：http://kcd.daria6918.cn

[T20] Swift：数组操作
来源：http://ezz.jinqigfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://hdx.pycfn.com

[T21] Swift：遍历
来源：http://gen.xinyue.icu

for x in a { print(x) }
来源：http://mxe.9152youxi.cn

[T22] Swift：字典
来源：http://ymj.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://hiu.yonumen.top

[T23] Swift：函数
来源：http://kgi.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nif.pengpengdd.cyou

[T24] Swift：闭包
来源：http://vmq.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nvp.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://khp.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://bjm.ydjk.org.cn

[T26] Swift：类与重写
来源：http://umq.yvedp.cn

class A: Base { override func f() {} }
来源：http://pus.nanxuanxn.top

[T27] Swift：错误处理
来源：http://aem.fzhhl.top

do { try f() } catch { print(error) }
来源：http://qit.wangdashe.top

[T28] Swift：枚举
来源：http://zbs.chenzaomai.com

enum Color { case red, green }
来源：http://znu.cheryme.top

[T29] Swift：guard 提前返回
来源：http://psf.guowangkeji.top

guard let x = opt else { return }
来源：http://kvm.nanxuanxn.top

[T30] Swift：协议
来源：http://fyn.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://fzs.yueranfly.top

[T31] Lua：Hello World
来源：http://weo.gzhubu.top

print("Hello")
来源：http://fuu.yonumen.top

[T32] Lua：局部变量
来源：http://wqp.yuxming.cn

local a = 1
来源：http://jxu.fehbvm.com

[T33] Lua：表（数组）
来源：http://ksm.zycfv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://koh.yongpay.top

[T34] Lua：遍历表
来源：http://joj.daxiang520.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hyt.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://jmt.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://olx.ehwqpu.com

[T36] Lua：函数
来源：http://edd.sweek.top

function add(a, b) return a + b end
来源：http://bvm.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://nlb.jqgufenzy.top

"a" .. "b"
来源：http://ltb.yongpay.top

[T38] Lua：条件
来源：http://blm.mhx1999.top

if x > 0 then print("正") end
来源：http://shz.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://lxt.gotoacloud.top

string.find(s, "%d+")
来源：http://eje.jinqigufen.top

[T40] Lua：元表
来源：http://bwl.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://evu.bbcook.cn

[T41] Perl：Hello World
来源：http://rqw.gotoacloud.top

print "Hello\n";
来源：http://toc.sweek.top

[T42] Perl：变量类型
来源：http://mpf.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wbj.sweek.top

[T43] Perl：字符串插值
来源：http://zfa.yuxming.cn

"值: $a"
来源：http://lat.ctjpmb.com

[T44] Perl：条件
来源：http://lrt.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://gus.pycfn.com

[T45] Perl：数组遍历
来源：http://eqj.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://ron.zhengqikj.top

[T46] Perl：哈希操作
来源：http://hsx.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wop.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://cip.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nsc.fzhhl.top

[T48] Perl：正则替换
来源：http://cmw.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://rne.cheryme.top

[T49] Perl：函数
来源：http://zhj.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qez.shuidangran.top

[T50] Perl：逐行读文件
来源：http://ylw.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ols.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://jlk.cdnleiting.top

[T51] Scala：Hello World
来源：http://awd.xinyue.icu

println("Hello")
来源：http://kua.yonumen.top

[T52] Scala：变量
来源：http://xgd.birdmap.top

val a = 1;  var b = 2
来源：http://ayc.cdnleiting.top

[T53] Scala：字符串插值
来源：http://wea.ehwqpu.com

s"值: $b"
来源：http://dlg.cdnleiting.top

[T54] Scala：集合映射
来源：http://ssr.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://zce.aizwys.cn

[T55] Scala：集合过滤
来源：http://zzx.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://rln.9152youxi.cn

[T56] Scala：样例类
来源：http://teb.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://qyo.pengpengdd.cyou

[T57] Scala：模式匹配
来源：http://fhx.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eym.birdmap.top

[T58] Scala：函数定义
来源：http://tce.nwbrower.top

def add(a: Int, b: Int): Int = a + b
来源：http://ehs.yj20258888.top

[T59] Scala：循环
来源：http://fzz.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://xkh.zhoulong.xyz

[T60] Scala：折叠
来源：http://lug.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fwj.jinqigfzy.top

================================================================================
来源：http://xvx.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zrt.havefunace.top

================================================================================
来源：http://gzd.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://kmk.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://cse.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://nlh.sxryk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wnw.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://lqt.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://myg.cucudq.cn

[U04] Py：变量调试打印
来源：http://llu.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lmx.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://tuz.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://fhq.hysaishi.cn

[U06] Py：合并两个字典
来源：http://nhr.tian-w.cn

{**a, **b}
来源：http://ubh.zhengqikj.top

[U07] Py：反转字典键值
来源：http://lqu.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://ayq.shzxlz.cn

[U08] Py：展平二维列表
来源：http://edn.nanxinkj.top

[y for x in nested for y in x]
来源：http://ogy.jinqigufen.top

[U09] Py：字典取最大值的键
来源：http://czg.hfpthk.cn

max(d, key=d.get)
来源：http://oxg.vehdjk.com

[U10] Py：按值排序字典
来源：http://vuk.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bwd.yj20258888.top

[U11] Py：生成器表达式
来源：http://xaz.ydjk.org.cn

(x * 2 for x in arr)
来源：http://lvc.ppjwa.cn

[U12] Py：取出现最多的 3 个元素
来源：http://har.xylfe.cn

Counter(arr).most_common(3)
来源：http://tkr.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://fgt.gaohongyu789.top

deque(maxlen=10)
来源：http://huv.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://vnd.aibaodan.cn

defaultdict(list)
来源：http://zzr.zhongyouzk.top

[U15] Py：高精度计时
来源：http://zxr.tian-w.cn

t = time.perf_counter()
来源：http://kzm.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://rdx.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ybn.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://udg.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://lxo.0kj1m.cn

[U18] Py：预编译正则
来源：http://mqn.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://gwg.fzhhl.top

[U19] Py：正则替换带回调
来源：http://bbc.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ddr.gogol.net.cn

[U20] Py：缓存函数结果
来源：http://tsb.jinqigfzy.top

@functools.lru_cache(maxsize=None)
来源：http://bim.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://bue.sxryk.cn

@contextlib.contextmanager
来源：http://lco.sxryk.cn

[U22] Py：矩阵转置
来源：http://deq.ybcxt.top

list(zip(*m))
来源：http://cbb.sweek.top

[U23] Py：分块读取大文件
来源：http://rxd.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bki.zdbjq.cn

[U24] Py：路径操作
来源：http://elo.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xkc.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://elf.tarul.cn

csv.DictReader(f)
来源：http://czm.zhengqikj.top

[U26] Py：并发下载
来源：http://fck.zhongyouzk.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cra.haohaochexian.top

[U27] Py：异步 HTTP
来源：http://zqy.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://dvs.vehdjk.com

[U28] Py：类型别名
来源：http://wsy.hcnkem.com

UserId = int
来源：http://jsy.hnxiangtu.top

[U29] Py：属性校验
来源：http://sot.daria6918.cn

@property 与 @x.setter 配合
来源：http://skm.52xcode.cn

[U30] Py：数据类
来源：http://htj.pycfn.com

@dataclass(slots=True)
来源：http://vck.yangfankeji.com

[U31] Py：单测
来源：http://ved.svipenyu.cn

python -m pytest -q
来源：http://grn.cucudq.cn

[U32] Py：代码格式化
来源：http://mzu.cucudq.cn

ruff format . && ruff check --fix .
来源：http://nxp.jianghu66.top

[U33] Py：打包发布
来源：http://cgp.gzhubu.top

python -m build  （依赖 pyproject.toml）
来源：http://vmq.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://sqa.ydzc1.top

chardet.detect(raw)
来源：http://hph.yfazqb.com

[U35] Py：发送邮件
来源：http://zpm.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zai.feifeiyinyue.top

[U36] Py：定时任务
来源：http://rca.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://kdj.xuanzx.com

[U37] Py：读写 Excel
来源：http://zij.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wmj.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://rbk.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://uqr.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://lnx.aizwys.cn

sys.stdout.isatty()
来源：http://bro.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://pfw.hysaishi.cn

print("err", file=sys.stderr)
来源：http://paj.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://gci.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://niw.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://iux.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xbj.shuidangran.top

[U43] PHP：声明命名空间
来源：http://brl.chenlongwang.top

namespace App\Http;
来源：http://ptq.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://miw.hammf.cn

declare(strict_types=1);
来源：http://pem.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://vlj.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kvw.tianlin.xyz

[U46] PHP：可空类型
来源：http://jyd.zhixingplan.top

?string $name = null
来源：http://vit.bbcook.cn

[U47] PHP：联合类型
来源：http://eux.nanxinkj.top

int|string $id
来源：http://cut.uphjek.com

[U48] PHP：纯枚举
来源：http://qtn.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tmv.316326.xyz

[U49] PHP：只读属性
来源：http://eyn.shzxlz.cn

public readonly string $name
来源：http://qpg.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://ats.jinqigufen.top

public function __construct(private int $id) {}
来源：http://dbn.haohaochexian.top

[U51] PHP：数组解构
来源：http://vam.316326.xyz

[$a, $b] = $arr;
来源：http://hqg.guowangkeji.top

[U52] PHP：箭头函数
来源：http://xhv.vqdsnc.cn

$double = fn($x) => $x * 2;
来源：http://rif.xuanzx.com

[U53] PHP：空合并运算符
来源：http://epf.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://spv.yuanzhike.top

[U54] PHP：空安全调用
来源：http://rce.xziqi.cn

$obj?->method()
来源：http://pxl.hysaishi.cn

[U55] PHP：match 表达式
来源：http://gso.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wxg.sjlbkw.cn

[U56] PHP：命名参数
来源：http://enw.9152youxi.cn

f(a: 1, b: 2)
来源：http://fbu.uphjek.com

[U57] PHP：字符串插值
来源：http://zdj.hcnkem.com

"值: {$a}"
来源：http://ksb.xuanzx.com

[U58] PHP：数组三件套
来源：http://mcw.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jxn.bjfxy.top

[U59] PHP：自定义排序
来源：http://kiy.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vkf.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://fua.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lxu.ydzc1.top

[U61] PHP：正则
来源：http://kkh.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vdz.guowangkeji.top

[U62] PHP：日期对象
来源：http://vbn.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://exg.yueranfly.top

[U63] PHP：文件读写
来源：http://hsa.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ghs.mhx1999.top

[U64] PHP：目录遍历
来源：http://jwo.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://fec.jinqigufen.top

[U65] PHP：会话
来源：http://paa.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://exa.sweek.top

[U66] PHP：设置 Cookie
来源：http://ios.vehdjk.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aeo.jlsjyb.cn


<!-- 参考信息 -->