代发 wailian999

[S41] C++：类与构造函数
来源：http://pli.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jpe.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://nrh.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://ytb.quarkkingdee.top

[S43] C++：智能指针
来源：http://fht.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://rtg.wangshuangyany.cn

[S44] C++：引用传参
来源：http://gvu.yj20258.top

void inc(int &x) { ++x; }
来源：http://exq.chenzaomai.com

[S45] C++：lambda
来源：http://xzk.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://rlt.ydjk.org.cn

[S46] C++：函数模板
来源：http://qhz.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jmh.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://blu.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zxm.ivvv.top

[S48] C++：逐行读文件
来源：http://mnz.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ilq.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://axr.meibo888.top

[S49] C++：写文件
来源：http://wru.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://buz.dianchejie.cn

[S50] C++：格式化数字
来源：http://urx.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uda.yuanzhike.top

[S51] C++：显式类型转换
来源：http://ccp.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://lcq.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://kgq.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://mdp.hammf.cn

[S53] C++：移动语义
来源：http://ulb.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://qje.jinqigufen.top

[S54] C++：异常处理
来源：http://cmq.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fah.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://mcn.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wrk.tian-w.cn

[S56] C++：optional
来源：http://cyw.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wtc.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://elt.mhx1999.top

constexpr int N = 10;
来源：http://rhp.ppjwa.cn

[S58] C++：命名空间
来源：http://bau.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://vuc.cdnleiting.top

[S59] C++：静态断言
来源：http://tix.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uzs.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://iuu.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://acu.meibo888.top

================================================================================
来源：http://npe.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nrw.yueranfly.top

================================================================================
来源：http://rxv.yj20258888.top

[T01] Kotlin：Hello World
来源：http://fdy.fengsongda.top

println("Hello")
来源：http://wop.zhengqikj.top

[T02] Kotlin：变量
来源：http://isj.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tmw.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://waa.snrcjt.cn

"值: $b"
来源：http://vsu.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://obv.yangfankeji.com

val n: String? = null;  n?.length
来源：http://fao.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://gmw.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ezu.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://sks.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ccr.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://tpf.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dru.nanxuanxn.top

[T08] Kotlin：数据类
来源：http://sdt.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://tmv.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://ogn.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://kfh.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://msn.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rup.jinqigfzy.top

[T11] Kotlin：协程
来源：http://irr.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ijt.bjfxy.top

[T12] Kotlin：解构声明
来源：http://dpz.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://cdh.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://ezk.fktsv.cn

val m = mapOf("a" to 1)
来源：http://rpd.redwolf501.top

[T14] Kotlin：循环
来源：http://tqv.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://bbg.bjfxy.top

[T15] Kotlin：接口
来源：http://kdk.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://bdu.ctjpmb.com

[T16] Swift：Hello World
来源：http://hso.nanxuanxn.top

print("Hello")
来源：http://pfg.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://aqj.snrcjt.cn

var a = 1;  let b = 2
来源：http://xgd.ehwqpu.com

[T18] Swift：字符串插值
来源：http://bep.jinyuanbaomall.cn

"值: \(b)"
来源：http://dns.smart0.xyz

[T19] Swift：可选绑定
来源：http://jvg.guannengcc.top

if let n = opt { print(n) }
来源：http://ldw.meibo888.top

[T20] Swift：数组操作
来源：http://waf.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fqe.sjlbkw.cn

[T21] Swift：遍历
来源：http://tbf.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://ovf.ehwqpu.com

[T22] Swift：字典
来源：http://wix.nanxinkj.top

var d = ["a": 1];  d["b"] = 2
来源：http://cbh.epnwcf.com

[T23] Swift：函数
来源：http://yum.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nhs.zdbjq.cn

[T24] Swift：闭包
来源：http://tii.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mqk.0kj1m.cn

[T25] Swift：结构体
来源：http://cds.dashuyun.cn

struct P { var x: Int }
来源：http://lmw.yj202588.top

[T26] Swift：类与重写
来源：http://sgf.daria6918.cn

class A: Base { override func f() {} }
来源：http://llv.hammf.cn

[T27] Swift：错误处理
来源：http://rcb.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://giv.gzhubu.top

[T28] Swift：枚举
来源：http://jou.chenzaomai.com

enum Color { case red, green }
来源：http://joh.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://uzz.shzxlz.cn

guard let x = opt else { return }
来源：http://bey.jinqigufen.top

[T30] Swift：协议
来源：http://asg.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://xxu.kuanghao11.cn

[T31] Lua：Hello World
来源：http://oew.iojbl.cn

print("Hello")
来源：http://xbp.pycfn.com

[T32] Lua：局部变量
来源：http://xiq.cheryme.top

local a = 1
来源：http://mjc.xziqi.cn

[T33] Lua：表（数组）
来源：http://pye.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ada.kuanghao11.cn

[T34] Lua：遍历表
来源：http://god.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ciu.svipenyu.cn

[T35] Lua：字典表
来源：http://hly.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://jpd.yangfankeji.com

[T36] Lua：函数
来源：http://zyt.yanxiufei.cn

function add(a, b) return a + b end
来源：http://eiq.ivvv.top

[T37] Lua：字符串拼接
来源：http://rzx.jiagoushi.top

"a" .. "b"
来源：http://sly.xziqi.cn

[T38] Lua：条件
来源：http://qig.ybcxt.top

if x > 0 then print("正") end
来源：http://mbd.ppjwa.cn

[T39] Lua：模式匹配
来源：http://fmj.nwbrower.top

string.find(s, "%d+")
来源：http://nnz.yfazqb.com

[T40] Lua：元表
来源：http://btr.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://enc.havefunace.top

[T41] Perl：Hello World
来源：http://hfs.jinghuilouyu.cn

print "Hello\n";
来源：http://iox.fehbvm.com

[T42] Perl：变量类型
来源：http://erf.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://epj.epnwcf.com

[T43] Perl：字符串插值
来源：http://oud.jinqigufen.top

"值: $a"
来源：http://bvc.52xcode.cn

[T44] Perl：条件
来源：http://skz.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://pad.snrcjt.cn

[T45] Perl：数组遍历
来源：http://zvp.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://lkc.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://evc.52xcode.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ujz.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://rvl.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fch.aibaodan.cn

[T48] Perl：正则替换
来源：http://jbm.hysaishi.cn

$s =~ s/old/new/g;
来源：http://vrn.ppjwa.cn

[T49] Perl：函数
来源：http://hel.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tai.sxryk.cn

[T50] Perl：逐行读文件
来源：http://gkf.yonumen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pxk.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://crf.zhiwuduotai.top

[T51] Scala：Hello World
来源：http://oqi.316326.xyz

println("Hello")
来源：http://cxh.zhiwuduotai.top

[T52] Scala：变量
来源：http://mbd.hnxiangtu.top

val a = 1;  var b = 2
来源：http://yhg.zhoulong.xyz

[T53] Scala：字符串插值
来源：http://sow.fktsv.cn

s"值: $b"
来源：http://wum.yueranfly.top

[T54] Scala：集合映射
来源：http://sjh.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://smj.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://heh.sysykeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://fzx.yj202588.top

[T56] Scala：样例类
来源：http://uye.daria6918.cn

case class User(name: String, age: Int)
来源：http://xle.gotoacloud.top

[T57] Scala：模式匹配
来源：http://tph.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vas.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://gnb.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kxp.daxiang520.top

[T59] Scala：循环
来源：http://zvn.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://zbo.ctjpmb.com

[T60] Scala：折叠
来源：http://tmi.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bsa.andypj.xyz

================================================================================
来源：http://lxx.cqqwz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wkg.zhixingplan.top

================================================================================
来源：http://wjx.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://axp.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://tzz.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://xjr.yonumen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dwm.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://ugj.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://gxm.chenlongwang.top

[U04] Py：变量调试打印
来源：http://pgu.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://llj.pycfn.com

[U05] Py：列表去重且保序
来源：http://atm.gzhubu.top

list(dict.fromkeys(arr))
来源：http://txc.snrcjt.cn

[U06] Py：合并两个字典
来源：http://xpk.yueranfly.top

{**a, **b}
来源：http://nrx.ehwqpu.com

[U07] Py：反转字典键值
来源：http://lro.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://iml.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://wjx.cashguo.top

[y for x in nested for y in x]
来源：http://fiv.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://yve.cqqwz.cn

max(d, key=d.get)
来源：http://nju.cucudq.cn

[U10] Py：按值排序字典
来源：http://aig.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://syc.yfazqb.com

[U11] Py：生成器表达式
来源：http://osj.zhixingplan.top

(x * 2 for x in arr)
来源：http://vkd.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://shf.epnwcf.com

Counter(arr).most_common(3)
来源：http://eby.redwolf501.top

[U13] Py：固定长度队列
来源：http://pvo.meibo888.top

deque(maxlen=10)
来源：http://ngk.fzhhl.top

[U14] Py：分组收集到列表
来源：http://fra.cucudq.cn

defaultdict(list)
来源：http://zin.shzxlz.cn

[U15] Py：高精度计时
来源：http://tao.yangfankeji.com

t = time.perf_counter()
来源：http://rdu.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://nhn.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vfv.vqdsnc.cn

[U17] Py：初始化日志
来源：http://cpr.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://xfm.uphjek.com

[U18] Py：预编译正则
来源：http://bph.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://qte.gotoacloud.top

[U19] Py：正则替换带回调
来源：http://fue.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://elz.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://dys.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://qot.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://vzg.zdqjudy.top

@contextlib.contextmanager
来源：http://wxk.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://wwr.xingfuxueyuan.xyz

list(zip(*m))
来源：http://blj.yj202588.top

[U23] Py：分块读取大文件
来源：http://ijf.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hwe.daxiang520.top

[U24] Py：路径操作
来源：http://cuq.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tdt.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://pvm.jiagoushi.top

csv.DictReader(f)
来源：http://ryj.ydjk.org.cn

[U26] Py：并发下载
来源：http://lvv.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yvr.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://poo.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://dmd.ydjk.org.cn

[U28] Py：类型别名
来源：http://tik.meibo888.top

UserId = int
来源：http://wqv.bbcook.cn

[U29] Py：属性校验
来源：http://iwr.dashuyun.cn

@property 与 @x.setter 配合
来源：http://fwn.iojbl.cn

[U30] Py：数据类
来源：http://gaj.cashguo.top

@dataclass(slots=True)
来源：http://abu.epnwcf.com

[U31] Py：单测
来源：http://frx.smart0.xyz

python -m pytest -q
来源：http://kps.nwbrower.top

[U32] Py：代码格式化
来源：http://axy.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://xcu.yanxiufei.cn

[U33] Py：打包发布
来源：http://jcj.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://rwl.jqgfzy.top

[U34] Py：判断编码
来源：http://ruk.shangyingyoupin.top

chardet.detect(raw)
来源：http://gci.yueranfly.top

[U35] Py：发送邮件
来源：http://kgi.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dmz.uphjek.com

[U36] Py：定时任务
来源：http://lbh.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://xvi.jinqigufen.top

[U37] Py：读写 Excel
来源：http://wpv.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zbg.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://gkk.jianghu66.top

Path(__file__).resolve().parent
来源：http://kmp.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://snl.jyoumei.cn

sys.stdout.isatty()
来源：http://jzd.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://ytv.aibaodan.cn

print("err", file=sys.stderr)
来源：http://ymz.hnxiangtu.top

[U41] PHP：初始化 Composer 项目
来源：http://tgp.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kks.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://hhw.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ngv.tian-w.cn

[U43] PHP：声明命名空间
来源：http://ita.sxryk.cn

namespace App\Http;
来源：http://crx.jqgufenzy.top

[U44] PHP：开启严格类型
来源：http://hew.hammf.cn

declare(strict_types=1);
来源：http://pzm.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://kwu.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tdz.fzhhl.top

[U46] PHP：可空类型
来源：http://ewk.fengsongda.top

?string $name = null
来源：http://ejo.yongpay.top

[U47] PHP：联合类型
来源：http://dln.ybcxt.top

int|string $id
来源：http://deu.guowangkeji.top

[U48] PHP：纯枚举
来源：http://iij.hesvh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cvc.jqgfzy.top

[U49] PHP：只读属性
来源：http://izo.aibaodan.cn

public readonly string $name
来源：http://fii.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://vsh.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://kmp.redwolf501.top

[U51] PHP：数组解构
来源：http://iwr.yj20258888.top

[$a, $b] = $arr;
来源：http://cyz.zdqjudy.top

[U52] PHP：箭头函数
来源：http://xge.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://nbb.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://pnt.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://rsv.9152youxi.cn

[U54] PHP：空安全调用
来源：http://sqj.cdnleiting.top

$obj?->method()
来源：http://qxr.ydjk.org.cn

[U55] PHP：match 表达式
来源：http://sgn.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vcl.cheryme.top

[U56] PHP：命名参数
来源：http://ekf.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://ayc.dashuyun.cn

[U57] PHP：字符串插值
来源：http://rjz.xuetiantiany.cn

"值: {$a}"
来源：http://qwg.uphjek.com

[U58] PHP：数组三件套
来源：http://kga.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wfy.yj20258.top

[U59] PHP：自定义排序
来源：http://gkl.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kni.cashguo.top

[U60] PHP：JSON 编解码
来源：http://sly.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rih.vehdjk.com

[U61] PHP：正则
来源：http://xhw.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wii.jyoumei.cn

[U62] PHP：日期对象
来源：http://eeq.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lke.redwolf501.top

[U63] PHP：文件读写
来源：http://knb.kuanghao11.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://num.tanke756.top

[U64] PHP：目录遍历
来源：http://wmw.cashguo.top

glob("dir/*.php");  scandir("dir");
来源：http://hlw.ppjwa.cn

[U65] PHP：会话
来源：http://uun.yj20258888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dgy.xingfuxueyuan.xyz

[U66] PHP：设置 Cookie
来源：http://tjs.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wfp.hnqzz.top


<!-- 参考信息 -->