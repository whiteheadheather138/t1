代发 wailian999

[S41] C++：类与构造函数
来源：http://byv.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://msw.hnxiangtu.top

[S42] C++：继承与虚函数
来源：http://oln.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://tsy.ydzc1.top

[S43] C++：智能指针
来源：http://vbl.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://enj.cqqwz.cn

[S44] C++：引用传参
来源：http://siv.fktsv.cn

void inc(int &x) { ++x; }
来源：http://fbw.yj20258.top

[S45] C++：lambda
来源：http://lfn.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://duy.guowangkeji.top

[S46] C++：函数模板
来源：http://mtc.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xfb.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://pky.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sxs.hcnkem.com

[S48] C++：逐行读文件
来源：http://ebg.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hvx.tian-w.cn

while (std::getline(in, line)) { }
来源：http://gbm.tarul.cn

[S49] C++：写文件
来源：http://ipx.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gkb.zhoulong.xyz

[S50] C++：格式化数字
来源：http://xpy.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xnl.nwbrower.top

[S51] C++：显式类型转换
来源：http://msj.guowangkeji.top

static_cast<double>(a) / b
来源：http://zix.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://jnx.pycfn.com

int size() const noexcept { return n_; }
来源：http://cnp.ydzc1.top

[S53] C++：移动语义
来源：http://ztj.ivvv.top

std::vector<int> w = std::move(v);
来源：http://kgt.hfpthk.cn

[S54] C++：异常处理
来源：http://ovj.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nfx.daxiang520.top

[S55] C++：结构化绑定
来源：http://plq.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sho.meibo888.top

[S56] C++：optional
来源：http://lmt.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oxy.zdbjq.cn

[S57] C++：编译期常量
来源：http://mue.c1oappe.top

constexpr int N = 10;
来源：http://ahf.0kj1m.cn

[S58] C++：命名空间
来源：http://vae.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://pwo.snrcjt.cn

[S59] C++：静态断言
来源：http://oke.sxryk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sye.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://xmf.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dbz.cucudq.cn

================================================================================
来源：http://opt.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yjg.ydjk.org.cn

================================================================================
来源：http://tmz.yonumen.top

[T01] Kotlin：Hello World
来源：http://btv.wangshuangyany.cn

println("Hello")
来源：http://uwa.jqgfzy.top

[T02] Kotlin：变量
来源：http://pft.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://geq.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://non.gotoacloud.top

"值: $b"
来源：http://cej.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://aka.hysaishi.cn

val n: String? = null;  n?.length
来源：http://iam.yongpay.top

[T05] Kotlin：when 表达式
来源：http://nwi.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://isw.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://pyi.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qfg.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://imo.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://lcx.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://lhr.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://uqr.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://fwe.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://adp.tanke756.top

[T10] Kotlin：默认参数
来源：http://vwh.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://htz.sufxvd.cn

[T11] Kotlin：协程
来源：http://zho.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://snl.fengsongda.top

[T12] Kotlin：解构声明
来源：http://qsp.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://bom.yongpay.top

[T13] Kotlin：只读 Map
来源：http://vri.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://owq.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://ytz.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://awg.quarkkingdee.top

[T15] Kotlin：接口
来源：http://yyq.bbcook.cn

interface Shape { fun area(): Double }
来源：http://xvk.jyoumei.cn

[T16] Swift：Hello World
来源：http://eqq.feifeiyinyue.top

print("Hello")
来源：http://yfa.yangfankeji.com

[T17] Swift：变量与常量
来源：http://zpo.aizwys.cn

var a = 1;  let b = 2
来源：http://gjn.sufxvd.cn

[T18] Swift：字符串插值
来源：http://hon.fanxiaobao.xyz

"值: \(b)"
来源：http://zpa.yangfankeji.com

[T19] Swift：可选绑定
来源：http://qlk.shzxlz.cn

if let n = opt { print(n) }
来源：http://row.xinyue.icu

[T20] Swift：数组操作
来源：http://xzh.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://oyn.fktsv.cn

[T21] Swift：遍历
来源：http://sqx.ehwqpu.com

for x in a { print(x) }
来源：http://gvu.jinghuilouyu.cn

[T22] Swift：字典
来源：http://khe.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jvb.haohaochexian.top

[T23] Swift：函数
来源：http://mct.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://reg.tian-w.cn

[T24] Swift：闭包
来源：http://bdk.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ggi.52xcode.cn

[T25] Swift：结构体
来源：http://utv.zhongyouzk.top

struct P { var x: Int }
来源：http://zjx.jinyuanbaomall.cn

[T26] Swift：类与重写
来源：http://wca.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://bmp.wangdashe.top

[T27] Swift：错误处理
来源：http://feq.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://rei.quarkkingdee.top

[T28] Swift：枚举
来源：http://xsg.hcnkem.com

enum Color { case red, green }
来源：http://fys.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://bkt.yj20258888.top

guard let x = opt else { return }
来源：http://uyv.jqgufenzy.top

[T30] Swift：协议
来源：http://wwl.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://out.hfpthk.cn

[T31] Lua：Hello World
来源：http://yat.zycfv.cn

print("Hello")
来源：http://anp.ppjwa.cn

[T32] Lua：局部变量
来源：http://oru.cheryme.top

local a = 1
来源：http://qiz.ppjwa.cn

[T33] Lua：表（数组）
来源：http://flq.hysaishi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sie.0kj1m.cn

[T34] Lua：遍历表
来源：http://vlo.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uyo.jyoumei.cn

[T35] Lua：字典表
来源：http://rvh.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://evk.kuanghao11.cn

[T36] Lua：函数
来源：http://dqv.bbcook.cn

function add(a, b) return a + b end
来源：http://zdv.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://usr.nwbrower.top

"a" .. "b"
来源：http://dcu.quarkkingdee.top

[T38] Lua：条件
来源：http://xvr.ctjpmb.com

if x > 0 then print("正") end
来源：http://pux.tarul.cn

[T39] Lua：模式匹配
来源：http://dua.meibo888.top

string.find(s, "%d+")
来源：http://njn.xziqi.cn

[T40] Lua：元表
来源：http://swl.jianghu66.top

setmetatable({}, { __index = base })
来源：http://ppg.sjlbkw.cn

[T41] Perl：Hello World
来源：http://cgs.chenlongwang.top

print "Hello\n";
来源：http://kbt.yangfankeji.com

[T42] Perl：变量类型
来源：http://els.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bwa.xziqi.cn

[T43] Perl：字符串插值
来源：http://tbs.svipenyu.cn

"值: $a"
来源：http://tof.hammf.cn

[T44] Perl：条件
来源：http://kfy.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://ogm.xylfe.cn

[T45] Perl：数组遍历
来源：http://rgz.cheryme.top

for my $x (@arr) { print $x; }
来源：http://sfl.tanke756.top

[T46] Perl：哈希操作
来源：http://bnl.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ghb.daxiang520.top

[T47] Perl：正则捕获
来源：http://vet.zhengqikj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ukj.ctjpmb.com

[T48] Perl：正则替换
来源：http://hcd.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://ydp.hnqzz.top

[T49] Perl：函数
来源：http://biw.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wcd.hesvh.cn

[T50] Perl：逐行读文件
来源：http://zlr.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vcy.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://ewd.yonumen.top

[T51] Scala：Hello World
来源：http://vab.bjfxy.top

println("Hello")
来源：http://iuk.9152youxi.cn

[T52] Scala：变量
来源：http://qvz.pycfn.com

val a = 1;  var b = 2
来源：http://eix.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://ifp.chenjidiqi.icu

s"值: $b"
来源：http://yqm.zhijiandao.cn

[T54] Scala：集合映射
来源：http://oga.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://est.ybcxt.top

[T55] Scala：集合过滤
来源：http://nph.dashuyun.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oii.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://dcn.aibaodan.cn

case class User(name: String, age: Int)
来源：http://kfv.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://aut.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://htd.yueranfly.top

[T58] Scala：函数定义
来源：http://vop.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://aji.zdbjq.cn

[T59] Scala：循环
来源：http://oei.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://mob.guannengcc.top

[T60] Scala：折叠
来源：http://rkz.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://azz.ehwqpu.com

================================================================================
来源：http://odo.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ygx.jlsjyb.cn

================================================================================
来源：http://spr.havefunace.top

[U01] Py：创建虚拟环境
来源：http://btq.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hup.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://ifo.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vuv.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://xav.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://evo.c1oappe.top

[U04] Py：变量调试打印
来源：http://hfh.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vij.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://drr.vqdsnc.cn

list(dict.fromkeys(arr))
来源：http://qbd.gotoacloud.top

[U06] Py：合并两个字典
来源：http://lzf.sweek.top

{**a, **b}
来源：http://whl.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://idi.xziqi.cn

{v: k for k, v in d.items()}
来源：http://psh.aibaodan.cn

[U08] Py：展平二维列表
来源：http://bun.yj202588.top

[y for x in nested for y in x]
来源：http://orr.yj202588.top

[U09] Py：字典取最大值的键
来源：http://dgm.sysykeji.top

max(d, key=d.get)
来源：http://jcz.cqqwz.cn

[U10] Py：按值排序字典
来源：http://asx.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qel.shanyushiyangkeji.top

[U11] Py：生成器表达式
来源：http://kid.epnwcf.com

(x * 2 for x in arr)
来源：http://xuf.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://oun.shzxlz.cn

Counter(arr).most_common(3)
来源：http://csx.cdnleiting.top

[U13] Py：固定长度队列
来源：http://npf.cqqwz.cn

deque(maxlen=10)
来源：http://ztx.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://xdj.gotoacloud.top

defaultdict(list)
来源：http://dtd.andypj.xyz

[U15] Py：高精度计时
来源：http://dav.ehwqpu.com

t = time.perf_counter()
来源：http://zxo.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://wwe.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ici.meibo888.top

[U17] Py：初始化日志
来源：http://vba.aibaodan.cn

logging.basicConfig(level=logging.INFO)
来源：http://hon.birdmap.top

[U18] Py：预编译正则
来源：http://cmp.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://mfi.tarul.cn

[U19] Py：正则替换带回调
来源：http://bst.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ttx.yfazqb.com

[U20] Py：缓存函数结果
来源：http://cgb.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://llw.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://ozb.hongshengwenyu.top

@contextlib.contextmanager
来源：http://vez.fehbvm.com

[U22] Py：矩阵转置
来源：http://cat.yj20258.top

list(zip(*m))
来源：http://uqg.sxryk.cn

[U23] Py：分块读取大文件
来源：http://rac.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tfl.snrcjt.cn

[U24] Py：路径操作
来源：http://kjq.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pdh.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://awr.yanxiufei.cn

csv.DictReader(f)
来源：http://xyg.fzhhl.top

[U26] Py：并发下载
来源：http://zlk.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fjm.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://kps.guowangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://nxa.yvedp.cn

[U28] Py：类型别名
来源：http://clz.yangfankeji.com

UserId = int
来源：http://bqc.quarkkingdee.top

[U29] Py：属性校验
来源：http://wbt.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://uch.zhiwuduotai.top

[U30] Py：数据类
来源：http://iqm.hnxiangtu.top

@dataclass(slots=True)
来源：http://abz.shzxlz.cn

[U31] Py：单测
来源：http://kyj.kuanghao11.cn

python -m pytest -q
来源：http://hjv.hysaishi.cn

[U32] Py：代码格式化
来源：http://nev.yonumen.top

ruff format . && ruff check --fix .
来源：http://zqu.c1oappe.top

[U33] Py：打包发布
来源：http://bys.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ywz.hysaishi.cn

[U34] Py：判断编码
来源：http://dte.zhongyouzk.top

chardet.detect(raw)
来源：http://rfr.zhongyouzk.top

[U35] Py：发送邮件
来源：http://cne.meibo888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jut.havefunace.top

[U36] Py：定时任务
来源：http://owf.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://rpz.yvedp.cn

[U37] Py：读写 Excel
来源：http://olg.chenjidiqi.icu

pandas.read_excel / DataFrame.to_excel
来源：http://zcm.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://kiq.hcnkem.com

Path(__file__).resolve().parent
来源：http://fwa.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://wbj.shangyingyoupin.top

sys.stdout.isatty()
来源：http://myr.zdbjq.cn

[U40] Py：打印到标准错误
来源：http://oyf.yj20258888.top

print("err", file=sys.stderr)
来源：http://ngu.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://gae.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://dmq.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://lgc.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nlq.havefunace.top

[U43] PHP：声明命名空间
来源：http://atl.vehdjk.com

namespace App\Http;
来源：http://vwp.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://qgv.gotoacloud.top

declare(strict_types=1);
来源：http://fgq.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://vdj.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yhe.yj202588.top

[U46] PHP：可空类型
来源：http://sbm.yueranfly.top

?string $name = null
来源：http://qwk.9152youxi.cn

[U47] PHP：联合类型
来源：http://pkw.gotoacloud.top

int|string $id
来源：http://fai.zdqjudy.top

[U48] PHP：纯枚举
来源：http://jie.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mwq.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://zwj.mhx1999.top

public readonly string $name
来源：http://yta.316326.xyz

[U50] PHP：构造器属性提升
来源：http://mhw.ppjwa.cn

public function __construct(private int $id) {}
来源：http://bmq.yanxiufei.cn

[U51] PHP：数组解构
来源：http://csk.kuanghao11.cn

[$a, $b] = $arr;
来源：http://xfe.ctjpmb.com

[U52] PHP：箭头函数
来源：http://ura.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://ofj.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://aub.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://jdx.havefunace.top

[U54] PHP：空安全调用
来源：http://yml.bbcook.cn

$obj?->method()
来源：http://lzh.zhoulong.xyz

[U55] PHP：match 表达式
来源：http://hse.jlsjyb.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hqt.bjfxy.top

[U56] PHP：命名参数
来源：http://wkq.zdqjudy.top

f(a: 1, b: 2)
来源：http://otw.yanxiufei.cn

[U57] PHP：字符串插值
来源：http://goh.shzxlz.cn

"值: {$a}"
来源：http://xcy.fktsv.cn

[U58] PHP：数组三件套
来源：http://dlx.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://snq.chenzaomai.com

[U59] PHP：自定义排序
来源：http://tbn.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kdn.hcnkem.com

[U60] PHP：JSON 编解码
来源：http://llp.jinqigfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pyq.meibo888.top

[U61] PHP：正则
来源：http://noz.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tnl.52xcode.cn

[U62] PHP：日期对象
来源：http://cnr.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bcz.hnqzz.top

[U63] PHP：文件读写
来源：http://uhp.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ezr.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://hno.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://ekx.cucudq.cn

[U65] PHP：会话
来源：http://yyh.snrcjt.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rhs.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://vgn.cdnleiting.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mmo.zhiwuduotai.top


<!-- 参考信息 -->