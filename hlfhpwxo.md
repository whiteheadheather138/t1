代发 wailian999

[S41] C++：类与构造函数
来源：http://shk.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jaq.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://zoz.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://ezo.mhx1999.top

[S43] C++：智能指针
来源：http://sgl.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://xmp.hesvh.cn

[S44] C++：引用传参
来源：http://nbt.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://dey.tian-w.cn

[S45] C++：lambda
来源：http://myk.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://egj.dashuyun.cn

[S46] C++：函数模板
来源：http://jma.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uuc.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://iwh.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nvt.chenlongwang.top

[S48] C++：逐行读文件
来源：http://ofr.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://hek.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://izj.yfazqb.com

[S49] C++：写文件
来源：http://drz.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xan.snrcjt.cn

[S50] C++：格式化数字
来源：http://dwn.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wsq.zhixingplan.top

[S51] C++：显式类型转换
来源：http://tin.hnqzz.top

static_cast<double>(a) / b
来源：http://xjf.yongpay.top

[S52] C++：const 与 noexcept
来源：http://qtv.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://bgr.cdnleiting.top

[S53] C++：移动语义
来源：http://dao.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://xfo.cashguo.top

[S54] C++：异常处理
来源：http://jnx.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mlc.jqgfzy.top

[S55] C++：结构化绑定
来源：http://vgt.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iaz.ppjwa.cn

[S56] C++：optional
来源：http://csp.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ufr.sysykeji.top

[S57] C++：编译期常量
来源：http://njt.zycfv.cn

constexpr int N = 10;
来源：http://ajp.ehwqpu.com

[S58] C++：命名空间
来源：http://idk.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://nvy.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://vud.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zxz.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://wet.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://owj.ctjpmb.com

================================================================================
来源：http://qbp.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://urj.yfazqb.com

================================================================================
来源：http://ffr.birdmap.top

[T01] Kotlin：Hello World
来源：http://qiw.shanyushiyangkeji.top

println("Hello")
来源：http://otb.birdmap.top

[T02] Kotlin：变量
来源：http://mou.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://djf.pengpengdd.cyou

[T03] Kotlin：字符串模板
来源：http://zwm.jinyuanbaomall.cn

"值: $b"
来源：http://eet.tanke756.top

[T04] Kotlin：空安全
来源：http://ezh.epnwcf.com

val n: String? = null;  n?.length
来源：http://svx.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://rrt.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nsn.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://ybp.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cly.pycfn.com

[T07] Kotlin：集合过滤
来源：http://fgb.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qkv.chenlongwang.top

[T08] Kotlin：数据类
来源：http://lsz.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://rtz.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://lfw.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://csc.shuidangran.top

[T10] Kotlin：默认参数
来源：http://nbh.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ylq.yfazqb.com

[T11] Kotlin：协程
来源：http://gyp.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zln.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://prh.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://jzz.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://hfo.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://zlj.iojbl.cn

[T14] Kotlin：循环
来源：http://pin.tanke756.top

for (i in 1..10) println(i)
来源：http://thf.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://jjx.uphjek.com

interface Shape { fun area(): Double }
来源：http://zle.yonumen.top

[T16] Swift：Hello World
来源：http://exw.nwbrower.top

print("Hello")
来源：http://bxn.cdnleiting.top

[T17] Swift：变量与常量
来源：http://vmy.cucudq.cn

var a = 1;  let b = 2
来源：http://eyf.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://qkz.fktsv.cn

"值: \(b)"
来源：http://weo.birdmap.top

[T19] Swift：可选绑定
来源：http://tqp.ydzc1.top

if let n = opt { print(n) }
来源：http://pph.jiagoushi.top

[T20] Swift：数组操作
来源：http://wry.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://mll.cashguo.top

[T21] Swift：遍历
来源：http://fcw.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://btb.nanxuanxn.top

[T22] Swift：字典
来源：http://aou.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://xow.tian-w.cn

[T23] Swift：函数
来源：http://gwr.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nfr.xylfe.cn

[T24] Swift：闭包
来源：http://mdv.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kbc.nanxuanxn.top

[T25] Swift：结构体
来源：http://eko.nanxinkj.top

struct P { var x: Int }
来源：http://buu.hnxiangtu.top

[T26] Swift：类与重写
来源：http://oec.cucudq.cn

class A: Base { override func f() {} }
来源：http://ddy.xziqi.cn

[T27] Swift：错误处理
来源：http://izu.fzhhl.top

do { try f() } catch { print(error) }
来源：http://dbs.wangshuangyany.cn

[T28] Swift：枚举
来源：http://oui.jyoumei.cn

enum Color { case red, green }
来源：http://run.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://ymn.meibo888.top

guard let x = opt else { return }
来源：http://bcw.zycfv.cn

[T30] Swift：协议
来源：http://tdb.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://hez.316326.xyz

[T31] Lua：Hello World
来源：http://zsf.ydzc1.top

print("Hello")
来源：http://uiu.fehbvm.com

[T32] Lua：局部变量
来源：http://lve.kuanghao11.cn

local a = 1
来源：http://vdd.hcnkem.com

[T33] Lua：表（数组）
来源：http://bdf.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cmo.jinqigufen.top

[T34] Lua：遍历表
来源：http://fxe.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://abw.zdbjq.cn

[T35] Lua：字典表
来源：http://pxd.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://zlc.yj202588.top

[T36] Lua：函数
来源：http://bjj.ctjpmb.com

function add(a, b) return a + b end
来源：http://zlh.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://lwn.havefunace.top

"a" .. "b"
来源：http://bci.ydjk.org.cn

[T38] Lua：条件
来源：http://ajw.uphjek.com

if x > 0 then print("正") end
来源：http://gmm.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://iwk.jinqigfzy.top

string.find(s, "%d+")
来源：http://uck.shzxlz.cn

[T40] Lua：元表
来源：http://ino.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://fot.daxiang520.top

[T41] Perl：Hello World
来源：http://vfq.jqgfzy.top

print "Hello\n";
来源：http://gzr.yj202588.top

[T42] Perl：变量类型
来源：http://git.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cft.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://jpw.bjfxy.top

"值: $a"
来源：http://dxh.meibo888.top

[T44] Perl：条件
来源：http://hcp.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://xbn.chenlongwang.top

[T45] Perl：数组遍历
来源：http://mdg.pycfn.com

for my $x (@arr) { print $x; }
来源：http://xhf.mhx1999.top

[T46] Perl：哈希操作
来源：http://not.jiagoushi.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mpa.sufxvd.cn

[T47] Perl：正则捕获
来源：http://gdr.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kzd.nanxuanxn.top

[T48] Perl：正则替换
来源：http://rdu.pycfn.com

$s =~ s/old/new/g;
来源：http://lea.ybcxt.top

[T49] Perl：函数
来源：http://tqp.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ezp.sufxvd.cn

[T50] Perl：逐行读文件
来源：http://wbq.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fqu.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://zqd.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://bae.hysaishi.cn

println("Hello")
来源：http://hgp.daria6918.cn

[T52] Scala：变量
来源：http://bti.hysaishi.cn

val a = 1;  var b = 2
来源：http://tdv.zdbjq.cn

[T53] Scala：字符串插值
来源：http://onf.zhiwuduotai.top

s"值: $b"
来源：http://mnl.pycfn.com

[T54] Scala：集合映射
来源：http://tly.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://cxw.fengsongda.top

[T55] Scala：集合过滤
来源：http://fgr.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://iet.hammf.cn

[T56] Scala：样例类
来源：http://hre.daxiang520.top

case class User(name: String, age: Int)
来源：http://jfr.dianchejie.cn

[T57] Scala：模式匹配
来源：http://dvb.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://hct.nanxuanxn.top

[T58] Scala：函数定义
来源：http://hxi.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://xnc.sufxvd.cn

[T59] Scala：循环
来源：http://hhm.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://mti.ydzc1.top

[T60] Scala：折叠
来源：http://ggj.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mbd.shuidangran.top

================================================================================
来源：http://qko.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fhp.52xcode.cn

================================================================================
来源：http://jor.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://nye.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://mfu.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://xxp.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ita.sweek.top

[U03] Py：加载 .env 配置
来源：http://ejj.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jxa.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://nui.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eae.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://arv.yj20258.top

list(dict.fromkeys(arr))
来源：http://pla.dashuyun.cn

[U06] Py：合并两个字典
来源：http://ttc.fehbvm.com

{**a, **b}
来源：http://ymr.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://peq.hammf.cn

{v: k for k, v in d.items()}
来源：http://pdz.316326.xyz

[U08] Py：展平二维列表
来源：http://hug.fktsv.cn

[y for x in nested for y in x]
来源：http://onr.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://ibn.hnqzz.top

max(d, key=d.get)
来源：http://xxl.ctjpmb.com

[U10] Py：按值排序字典
来源：http://sft.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jnx.andypj.xyz

[U11] Py：生成器表达式
来源：http://ojs.redwolf501.top

(x * 2 for x in arr)
来源：http://mkh.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://bdg.andypj.xyz

Counter(arr).most_common(3)
来源：http://kyd.xylfe.cn

[U13] Py：固定长度队列
来源：http://nma.smart0.xyz

deque(maxlen=10)
来源：http://rvm.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://ira.bjfxy.top

defaultdict(list)
来源：http://maz.nanxinkj.top

[U15] Py：高精度计时
来源：http://npe.fengsongda.top

t = time.perf_counter()
来源：http://nuw.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://frp.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cqt.0kj1m.cn

[U17] Py：初始化日志
来源：http://gpp.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://qml.redwolf501.top

[U18] Py：预编译正则
来源：http://lri.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://rtp.c1oappe.top

[U19] Py：正则替换带回调
来源：http://cgc.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://frb.cucudq.cn

[U20] Py：缓存函数结果
来源：http://dwm.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://zxc.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://gjl.zdbjq.cn

@contextlib.contextmanager
来源：http://fxh.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://rgz.zdqjudy.top

list(zip(*m))
来源：http://jou.fengsongda.top

[U23] Py：分块读取大文件
来源：http://qyi.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gbj.zhongyouzk.top

[U24] Py：路径操作
来源：http://abe.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xjx.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://gek.nwbrower.top

csv.DictReader(f)
来源：http://huf.quarkkingdee.top

[U26] Py：并发下载
来源：http://jvz.hnqzz.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bjq.feifeiyinyue.top

[U27] Py：异步 HTTP
来源：http://hfc.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://bcw.gotoacloud.top

[U28] Py：类型别名
来源：http://nhr.mhx1999.top

UserId = int
来源：http://sfg.shzxlz.cn

[U29] Py：属性校验
来源：http://xdf.zhengqikj.top

@property 与 @x.setter 配合
来源：http://qqq.jyoumei.cn

[U30] Py：数据类
来源：http://jxt.aizwys.cn

@dataclass(slots=True)
来源：http://vuv.bbcook.cn

[U31] Py：单测
来源：http://ftq.yj20258888.top

python -m pytest -q
来源：http://mzx.hesvh.cn

[U32] Py：代码格式化
来源：http://sdw.havefunace.top

ruff format . && ruff check --fix .
来源：http://rhh.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://idh.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://ifw.ppjwa.cn

[U34] Py：判断编码
来源：http://yid.hywenlv.cn

chardet.detect(raw)
来源：http://bqy.bbcook.cn

[U35] Py：发送邮件
来源：http://puk.zdqjudy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kja.cheryme.top

[U36] Py：定时任务
来源：http://sjh.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://vyu.yuanzhike.top

[U37] Py：读写 Excel
来源：http://qjg.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://vvo.xingfuxueyuan.xyz

[U38] Py：获取脚本所在目录
来源：http://heu.pycfn.com

Path(__file__).resolve().parent
来源：http://hzv.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://bpr.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://oyq.jianghu66.top

[U40] Py：打印到标准错误
来源：http://stp.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://sjw.hfpthk.cn

[U41] PHP：初始化 Composer 项目
来源：http://gqi.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uur.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://via.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ims.ydzc1.top

[U43] PHP：声明命名空间
来源：http://vfd.andypj.xyz

namespace App\Http;
来源：http://xjr.fanxiaobao.xyz

[U44] PHP：开启严格类型
来源：http://ino.fanxiaobao.xyz

declare(strict_types=1);
来源：http://hcm.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://svr.c1oappe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vmc.gaohongyu789.top

[U46] PHP：可空类型
来源：http://ldn.feifeiyinyue.top

?string $name = null
来源：http://xiq.xylfe.cn

[U47] PHP：联合类型
来源：http://kct.epnwcf.com

int|string $id
来源：http://bmd.ctjpmb.com

[U48] PHP：纯枚举
来源：http://lxx.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eit.snrcjt.cn

[U49] PHP：只读属性
来源：http://ruh.chenjidiqi.icu

public readonly string $name
来源：http://azk.epnwcf.com

[U50] PHP：构造器属性提升
来源：http://wlw.0kj1m.cn

public function __construct(private int $id) {}
来源：http://hwa.ehwqpu.com

[U51] PHP：数组解构
来源：http://kxt.uphjek.com

[$a, $b] = $arr;
来源：http://dnp.chenlongwang.top

[U52] PHP：箭头函数
来源：http://oei.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://hcl.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://noa.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://ouc.uphjek.com

[U54] PHP：空安全调用
来源：http://bkr.guowangkeji.top

$obj?->method()
来源：http://kzm.dianchejie.cn

[U55] PHP：match 表达式
来源：http://esp.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kpn.316326.xyz

[U56] PHP：命名参数
来源：http://qyc.nwbrower.top

f(a: 1, b: 2)
来源：http://zts.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://mnu.xziqi.cn

"值: {$a}"
来源：http://fan.yuanzhike.top

[U58] PHP：数组三件套
来源：http://tvt.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tid.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://kmt.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cvh.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://hhp.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jxo.hesvh.cn

[U61] PHP：正则
来源：http://mgf.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ayc.fengsongda.top

[U62] PHP：日期对象
来源：http://zad.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pyl.yvedp.cn

[U63] PHP：文件读写
来源：http://ami.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://alq.yfazqb.com

[U64] PHP：目录遍历
来源：http://tst.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://ekf.sysykeji.top

[U65] PHP：会话
来源：http://ihr.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uom.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://snb.sysykeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yap.shangyingyoupin.top


<!-- 参考信息 -->