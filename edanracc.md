代发 wailian999

[S39] C++：自定义比较器排序
来源：http://gjx.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xfz.gaohongyu789.top

[S40] C++：查找元素
来源：http://juj.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kmq.ppjwa.cn

[S41] C++：类与构造函数
来源：http://kkc.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pcp.birdmap.top

[S42] C++：继承与虚函数
来源：http://pdf.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://bzk.uphjek.com

[S43] C++：智能指针
来源：http://iqj.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://jov.zdqjudy.top

[S44] C++：引用传参
来源：http://rgm.gzhubu.top

void inc(int &x) { ++x; }
来源：http://uss.c1oappe.top

[S45] C++：lambda
来源：http://gfq.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://qgv.chenjidiqi.icu

[S46] C++：函数模板
来源：http://anz.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bfp.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://ari.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ugr.fktsv.cn

[S48] C++：逐行读文件
来源：http://ibf.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://zks.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://bqg.chenzaomai.com

[S49] C++：写文件
来源：http://kus.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uon.nanxuanxn.top

[S50] C++：格式化数字
来源：http://lzn.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qtg.ppjwa.cn

[S51] C++：显式类型转换
来源：http://qgk.redwolf501.top

static_cast<double>(a) / b
来源：http://pkh.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://vax.birdmap.top

int size() const noexcept { return n_; }
来源：http://mcc.shanyushiyangkeji.top

[S53] C++：移动语义
来源：http://mth.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://ylg.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://ugd.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hnd.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://bol.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yvc.aizwys.cn

[S56] C++：optional
来源：http://jyk.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://czv.yanxiufei.cn

[S57] C++：编译期常量
来源：http://iyo.jqgufenzy.top

constexpr int N = 10;
来源：http://uod.gogol.net.cn

[S58] C++：命名空间
来源：http://qna.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://eoo.shangyingyoupin.top

[S59] C++：静态断言
来源：http://ehd.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iwk.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://fwm.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dlr.uphjek.com

================================================================================
来源：http://mgn.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nog.jinghuilouyu.cn

================================================================================
来源：http://eyz.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://oii.vqdsnc.cn

println("Hello")
来源：http://wfp.hywenlv.cn

[T02] Kotlin：变量
来源：http://tya.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eyg.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://olx.mhx1999.top

"值: $b"
来源：http://gbr.fengsongda.top

[T04] Kotlin：空安全
来源：http://yyc.gotoacloud.top

val n: String? = null;  n?.length
来源：http://ubm.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://ybk.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nqi.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://guh.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ydl.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://vgm.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pqb.zycfv.cn

[T08] Kotlin：数据类
来源：http://jyi.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://gtg.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://dlc.birdmap.top

fun String.exclaim() = this + "!"
来源：http://fsh.jianghu66.top

[T10] Kotlin：默认参数
来源：http://ida.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lyi.gogol.net.cn

[T11] Kotlin：协程
来源：http://ziz.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://ycq.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://vca.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://kzp.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://kkc.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://ooh.xuanzx.com

[T14] Kotlin：循环
来源：http://zsv.tian-w.cn

for (i in 1..10) println(i)
来源：http://tai.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://jan.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://clr.fktsv.cn

[T16] Swift：Hello World
来源：http://orm.chenjidiqi.icu

print("Hello")
来源：http://feh.fktsv.cn

[T17] Swift：变量与常量
来源：http://dfi.tarul.cn

var a = 1;  let b = 2
来源：http://rqz.andypj.xyz

[T18] Swift：字符串插值
来源：http://ukn.gzhubu.top

"值: \(b)"
来源：http://gsx.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://ign.0kj1m.cn

if let n = opt { print(n) }
来源：http://max.yuxming.cn

[T20] Swift：数组操作
来源：http://xcx.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://rnx.zhijiandao.cn

[T21] Swift：遍历
来源：http://cjj.hnqzz.top

for x in a { print(x) }
来源：http://ksc.fengsongda.top

[T22] Swift：字典
来源：http://yop.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://adf.jiagoushi.top

[T23] Swift：函数
来源：http://xfm.jlsjyb.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yko.nanxuanxn.top

[T24] Swift：闭包
来源：http://wlm.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dmz.vehdjk.com

[T25] Swift：结构体
来源：http://prj.nanxuanxn.top

struct P { var x: Int }
来源：http://trz.zdbjq.cn

[T26] Swift：类与重写
来源：http://qid.fehbvm.com

class A: Base { override func f() {} }
来源：http://nwa.yfazqb.com

[T27] Swift：错误处理
来源：http://zaq.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://xie.sxryk.cn

[T28] Swift：枚举
来源：http://fvv.havefunace.top

enum Color { case red, green }
来源：http://zjp.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://hhj.cqqwz.cn

guard let x = opt else { return }
来源：http://ops.yuanzhike.top

[T30] Swift：协议
来源：http://oth.xylfe.cn

protocol Shape { func area() -> Double }
来源：http://zbx.gzhubu.top

[T31] Lua：Hello World
来源：http://haa.yueranfly.top

print("Hello")
来源：http://fqm.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://mdf.jinghuilouyu.cn

local a = 1
来源：http://nau.xuanzx.com

[T33] Lua：表（数组）
来源：http://epi.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://kwf.cashguo.top

[T34] Lua：遍历表
来源：http://hjo.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://rxx.iojbl.cn

[T35] Lua：字典表
来源：http://joz.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://kba.shangyingyoupin.top

[T36] Lua：函数
来源：http://ufn.yuanzhike.top

function add(a, b) return a + b end
来源：http://ykx.smart0.xyz

[T37] Lua：字符串拼接
来源：http://uci.gotoacloud.top

"a" .. "b"
来源：http://nta.wangdashe.top

[T38] Lua：条件
来源：http://ktj.hammf.cn

if x > 0 then print("正") end
来源：http://tav.jyoumei.cn

[T39] Lua：模式匹配
来源：http://fwd.dashuyun.cn

string.find(s, "%d+")
来源：http://ern.fzhhl.top

[T40] Lua：元表
来源：http://slx.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://ust.cashguo.top

[T41] Perl：Hello World
来源：http://gja.jianghu66.top

print "Hello\n";
来源：http://onm.tarul.cn

[T42] Perl：变量类型
来源：http://gio.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vkk.zycfv.cn

[T43] Perl：字符串插值
来源：http://wnl.zhiwuduotai.top

"值: $a"
来源：http://ebc.kuanghao11.cn

[T44] Perl：条件
来源：http://wvz.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://ntn.snrcjt.cn

[T45] Perl：数组遍历
来源：http://wbd.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://qxo.shzxlz.cn

[T46] Perl：哈希操作
来源：http://ite.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xki.tianlin.xyz

[T47] Perl：正则捕获
来源：http://ksv.jinqigfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mwd.fehbvm.com

[T48] Perl：正则替换
来源：http://lef.tarul.cn

$s =~ s/old/new/g;
来源：http://oar.nanxinkj.top

[T49] Perl：函数
来源：http://fin.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qyu.redwolf501.top

[T50] Perl：逐行读文件
来源：http://rvd.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jqx.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://jgr.hywenlv.cn

[T51] Scala：Hello World
来源：http://nhd.zhaomingkeji.xyz

println("Hello")
来源：http://fqt.nanxinkj.top

[T52] Scala：变量
来源：http://wln.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://eew.yfazqb.com

[T53] Scala：字符串插值
来源：http://nzs.ybcxt.top

s"值: $b"
来源：http://csw.cashguo.top

[T54] Scala：集合映射
来源：http://ziv.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://emk.yj20258888.top

[T55] Scala：集合过滤
来源：http://qwz.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hdf.uphjek.com

[T56] Scala：样例类
来源：http://yuv.aibaodan.cn

case class User(name: String, age: Int)
来源：http://ick.yj20258888.top

[T57] Scala：模式匹配
来源：http://hjs.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qsl.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://zsa.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://plr.yangfankeji.com

[T59] Scala：循环
来源：http://rhh.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://lih.ydzc1.top

[T60] Scala：折叠
来源：http://rkt.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ioc.hammf.cn

================================================================================
来源：http://rwn.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://abp.hammf.cn

================================================================================
来源：http://pcb.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://lwq.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://fjk.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://zrz.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xbw.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://poj.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dqn.vehdjk.com

[U04] Py：变量调试打印
来源：http://bhu.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://skr.sufxvd.cn

[U05] Py：列表去重且保序
来源：http://sey.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://gye.c1oappe.top

[U06] Py：合并两个字典
来源：http://kul.shanyushiyangkeji.top

{**a, **b}
来源：http://abu.haohaochexian.top

[U07] Py：反转字典键值
来源：http://fbr.daria6918.cn

{v: k for k, v in d.items()}
来源：http://pdw.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://rff.bjfxy.top

[y for x in nested for y in x]
来源：http://lti.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://trk.bbcook.cn

max(d, key=d.get)
来源：http://ggn.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://oop.shanyushiyangtech.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://clo.9152youxi.cn

[U11] Py：生成器表达式
来源：http://bkb.iojbl.cn

(x * 2 for x in arr)
来源：http://jyg.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zbl.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://fqs.yangfankeji.com

[U13] Py：固定长度队列
来源：http://vsr.yueranfly.top

deque(maxlen=10)
来源：http://itt.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://yep.hnxiangtu.top

defaultdict(list)
来源：http://ohx.jlsjyb.cn

[U15] Py：高精度计时
来源：http://yep.chenzaomai.com

t = time.perf_counter()
来源：http://ddd.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://cac.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jaa.tian-w.cn

[U17] Py：初始化日志
来源：http://ayv.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://hin.jianghu66.top

[U18] Py：预编译正则
来源：http://vfp.aibaodan.cn

pat = re.compile(r"\d+")
来源：http://fcs.xinyue.icu

[U19] Py：正则替换带回调
来源：http://jia.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nrc.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://elo.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://fxq.sweek.top

[U21] Py：自定义上下文管理器
来源：http://wkt.0kj1m.cn

@contextlib.contextmanager
来源：http://bur.uphjek.com

[U22] Py：矩阵转置
来源：http://jft.meibo888.top

list(zip(*m))
来源：http://bii.yongpay.top

[U23] Py：分块读取大文件
来源：http://hzb.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yop.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://cww.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://atk.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://dmj.cheryme.top

csv.DictReader(f)
来源：http://pdc.hysaishi.cn

[U26] Py：并发下载
来源：http://hnk.hcnkem.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oem.gzhubu.top

[U27] Py：异步 HTTP
来源：http://xyh.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://weh.yvedp.cn

[U28] Py：类型别名
来源：http://edp.gogol.net.cn

UserId = int
来源：http://ltk.gaohongyu789.top

[U29] Py：属性校验
来源：http://kvt.zdqjudy.top

@property 与 @x.setter 配合
来源：http://uek.dianchejie.cn

[U30] Py：数据类
来源：http://stu.smart0.xyz

@dataclass(slots=True)
来源：http://eno.daxiang520.top

[U31] Py：单测
来源：http://gfi.yuanzhike.top

python -m pytest -q
来源：http://dsu.guannengcc.top

[U32] Py：代码格式化
来源：http://ino.svipenyu.cn

ruff format . && ruff check --fix .
来源：http://hsn.hongshengwenyu.top

[U33] Py：打包发布
来源：http://lmb.zhiwuduotai.top

python -m build  （依赖 pyproject.toml）
来源：http://yha.hfpthk.cn

[U34] Py：判断编码
来源：http://wag.vehdjk.com

chardet.detect(raw)
来源：http://oir.dianchejie.cn

[U35] Py：发送邮件
来源：http://kgh.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bbd.c1oappe.top

[U36] Py：定时任务
来源：http://tsi.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://czm.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://ozq.gotoacloud.top

pandas.read_excel / DataFrame.to_excel
来源：http://asc.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://kjb.daria6918.cn

Path(__file__).resolve().parent
来源：http://slz.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://ori.tarul.cn

sys.stdout.isatty()
来源：http://gcf.birdmap.top

[U40] Py：打印到标准错误
来源：http://tpf.yj20258.top

print("err", file=sys.stderr)
来源：http://vfw.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://bie.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://bpy.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://rsa.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wni.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://ntj.jqgfzy.top

namespace App\Http;
来源：http://qqz.yvedp.cn

[U44] PHP：开启严格类型
来源：http://avn.cqqwz.cn

declare(strict_types=1);
来源：http://tvr.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://gol.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://apa.yueranfly.top

[U46] PHP：可空类型
来源：http://usr.fktsv.cn

?string $name = null
来源：http://oah.andypj.xyz

[U47] PHP：联合类型
来源：http://yel.zhoulong.xyz

int|string $id
来源：http://knw.sxryk.cn

[U48] PHP：纯枚举
来源：http://etk.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kbi.dashuyun.cn

[U49] PHP：只读属性
来源：http://qli.jiagoushi.top

public readonly string $name
来源：http://fsk.dashuyun.cn

[U50] PHP：构造器属性提升
来源：http://ejg.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://vae.bjfxy.top

[U51] PHP：数组解构
来源：http://tea.xuanzx.com

[$a, $b] = $arr;
来源：http://jlw.hnxiangtu.top

[U52] PHP：箭头函数
来源：http://iwf.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://kqh.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://ybx.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://kjg.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://njm.yanxiufei.cn

$obj?->method()
来源：http://ofu.smart0.xyz

[U55] PHP：match 表达式
来源：http://xgd.cucudq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qzu.dashuyun.cn

[U56] PHP：命名参数
来源：http://wbk.nanxinkj.top

f(a: 1, b: 2)
来源：http://qqt.svipenyu.cn

[U57] PHP：字符串插值
来源：http://nbb.zhijiandao.cn

"值: {$a}"
来源：http://czi.tianlin.xyz

[U58] PHP：数组三件套
来源：http://krc.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bab.sufxvd.cn

[U59] PHP：自定义排序
来源：http://jxu.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ihp.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://dcj.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ics.nanxinkj.top

[U61] PHP：正则
来源：http://ofm.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zmk.hcnkem.com

[U62] PHP：日期对象
来源：http://bfu.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://woj.nanxinkj.top

[U63] PHP：文件读写
来源：http://app.kuanghao11.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zjs.yvedp.cn

[U64] PHP：目录遍历
来源：http://qgg.cashguo.top

glob("dir/*.php");  scandir("dir");
来源：http://gsg.fzhhl.top


<!-- 参考信息 -->