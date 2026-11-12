代发 wailian999

[S39] C++：自定义比较器排序
来源：http://ktq.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://niw.jyoumei.cn

[S40] C++：查找元素
来源：http://msg.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hzp.hammf.cn

[S41] C++：类与构造函数
来源：http://qkl.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://klz.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://qwb.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://leg.hywenlv.cn

[S43] C++：智能指针
来源：http://rqr.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://egp.smart0.xyz

[S44] C++：引用传参
来源：http://wiq.yfazqb.com

void inc(int &x) { ++x; }
来源：http://ttn.zdqjudy.top

[S45] C++：lambda
来源：http://ffs.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://qjl.jianghu66.top

[S46] C++：函数模板
来源：http://zju.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dun.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://psz.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://boc.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://ofi.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ajs.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://ybw.dianchejie.cn

[S49] C++：写文件
来源：http://yva.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lwy.fengsongda.top

[S50] C++：格式化数字
来源：http://zqr.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gdf.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://kln.hammf.cn

static_cast<double>(a) / b
来源：http://wio.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://viu.yj20258.top

int size() const noexcept { return n_; }
来源：http://sno.zdbjq.cn

[S53] C++：移动语义
来源：http://tby.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://goc.chenjidiqi.icu

[S54] C++：异常处理
来源：http://arp.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rtw.dashuyun.cn

[S55] C++：结构化绑定
来源：http://vfk.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://twy.ybcxt.top

[S56] C++：optional
来源：http://xat.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kiw.gogol.net.cn

[S57] C++：编译期常量
来源：http://pmm.jinghuilouyu.cn

constexpr int N = 10;
来源：http://vul.daxiang520.top

[S58] C++：命名空间
来源：http://ggw.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://jzn.yfazqb.com

[S59] C++：静态断言
来源：http://vav.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oav.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://rqe.hcnkem.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wbz.tanke756.top

================================================================================
来源：http://yqz.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uij.hongshengwenyu.top

================================================================================
来源：http://sgv.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://byg.nwbrower.top

println("Hello")
来源：http://vtt.zhijiandao.cn

[T02] Kotlin：变量
来源：http://sth.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oxh.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://tqp.ybcxt.top

"值: $b"
来源：http://kas.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://ynj.jianghu66.top

val n: String? = null;  n?.length
来源：http://ujx.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://mqc.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rhg.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://tmx.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hal.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://yeu.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://whn.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://pgb.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://bry.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://fjh.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://wzf.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://jyb.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vqn.guannengcc.top

[T11] Kotlin：协程
来源：http://xow.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rcn.nanxuanxn.top

[T12] Kotlin：解构声明
来源：http://ura.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://dod.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://xje.cheryme.top

val m = mapOf("a" to 1)
来源：http://ikx.zhixingplan.top

[T14] Kotlin：循环
来源：http://uqf.fengsongda.top

for (i in 1..10) println(i)
来源：http://cvs.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://qdv.hnqzz.top

interface Shape { fun area(): Double }
来源：http://hks.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://kyf.fzhhl.top

print("Hello")
来源：http://kjy.9152youxi.cn

[T17] Swift：变量与常量
来源：http://hrk.nanxinkj.top

var a = 1;  let b = 2
来源：http://uos.iojbl.cn

[T18] Swift：字符串插值
来源：http://mve.meibo888.top

"值: \(b)"
来源：http://vqc.aizwys.cn

[T19] Swift：可选绑定
来源：http://llr.hysaishi.cn

if let n = opt { print(n) }
来源：http://gfe.316326.xyz

[T20] Swift：数组操作
来源：http://wdg.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://txa.sxryk.cn

[T21] Swift：遍历
来源：http://jqh.pycfn.com

for x in a { print(x) }
来源：http://wwu.yuxming.cn

[T22] Swift：字典
来源：http://tod.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://bot.xziqi.cn

[T23] Swift：函数
来源：http://dyk.zhaomingkeji.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://icq.gaohongyu789.top

[T24] Swift：闭包
来源：http://hbe.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kze.guowangkeji.top

[T25] Swift：结构体
来源：http://lbx.sysykeji.top

struct P { var x: Int }
来源：http://qmd.shuidangran.top

[T26] Swift：类与重写
来源：http://sbt.snrcjt.cn

class A: Base { override func f() {} }
来源：http://abu.jlsjyb.cn

[T27] Swift：错误处理
来源：http://pdc.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://zly.shangyingyoupin.top

[T28] Swift：枚举
来源：http://mkd.redwolf501.top

enum Color { case red, green }
来源：http://omu.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://gsg.daria6918.cn

guard let x = opt else { return }
来源：http://ivd.jiagoushi.top

[T30] Swift：协议
来源：http://hyu.yj20258888.top

protocol Shape { func area() -> Double }
来源：http://uez.tanke756.top

[T31] Lua：Hello World
来源：http://ano.wangdashe.top

print("Hello")
来源：http://nzr.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://exw.cashguo.top

local a = 1
来源：http://duc.fzhhl.top

[T33] Lua：表（数组）
来源：http://tmf.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kio.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://byu.jinqigfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kgz.quarkkingdee.top

[T35] Lua：字典表
来源：http://hux.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://jrj.zhoulong.xyz

[T36] Lua：函数
来源：http://qez.52xcode.cn

function add(a, b) return a + b end
来源：http://hua.cqqwz.cn

[T37] Lua：字符串拼接
来源：http://sui.hfpthk.cn

"a" .. "b"
来源：http://mcj.0kj1m.cn

[T38] Lua：条件
来源：http://epf.ybcxt.top

if x > 0 then print("正") end
来源：http://eui.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://cge.yuanzhike.top

string.find(s, "%d+")
来源：http://cae.fanxiaobao.xyz

[T40] Lua：元表
来源：http://aub.sysykeji.top

setmetatable({}, { __index = base })
来源：http://vud.fktsv.cn

[T41] Perl：Hello World
来源：http://ano.meibo888.top

print "Hello\n";
来源：http://gmw.sweek.top

[T42] Perl：变量类型
来源：http://amz.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://axn.yueranfly.top

[T43] Perl：字符串插值
来源：http://fgf.ydjk.org.cn

"值: $a"
来源：http://hrm.fanxiaobao.xyz

[T44] Perl：条件
来源：http://brs.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://csr.gotoacloud.top

[T45] Perl：数组遍历
来源：http://ird.ywan-chungtsiang.top

for my $x (@arr) { print $x; }
来源：http://ddz.tanke756.top

[T46] Perl：哈希操作
来源：http://caj.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aih.c1oappe.top

[T47] Perl：正则捕获
来源：http://gaz.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vjf.zycfv.cn

[T48] Perl：正则替换
来源：http://bhr.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://wtv.yfazqb.com

[T49] Perl：函数
来源：http://izi.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wpk.yj202588.top

[T50] Perl：逐行读文件
来源：http://vsm.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jnx.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://xei.sufxvd.cn

[T51] Scala：Hello World
来源：http://qmg.fengsongda.top

println("Hello")
来源：http://bvl.iojbl.cn

[T52] Scala：变量
来源：http://lpe.ydzc1.top

val a = 1;  var b = 2
来源：http://zdb.fzhhl.top

[T53] Scala：字符串插值
来源：http://iea.hcnkem.com

s"值: $b"
来源：http://bwn.fktsv.cn

[T54] Scala：集合映射
来源：http://rsm.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://lds.yueranfly.top

[T55] Scala：集合过滤
来源：http://zkr.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eym.fehbvm.com

[T56] Scala：样例类
来源：http://euu.ybcxt.top

case class User(name: String, age: Int)
来源：http://fea.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://ael.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kga.cucudq.cn

[T58] Scala：函数定义
来源：http://khz.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wcz.zhixingplan.top

[T59] Scala：循环
来源：http://rpu.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://hhf.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://xqz.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vlx.yuanzhike.top

================================================================================
来源：http://fjc.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kjo.uphjek.com

================================================================================
来源：http://tvv.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://tsq.chenzaomai.com

python -m venv .venv && source .venv/bin/activate
来源：http://wik.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://bjl.hysaishi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sha.daria6918.cn

[U03] Py：加载 .env 配置
来源：http://lpo.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://clt.sufxvd.cn

[U04] Py：变量调试打印
来源：http://cwl.tarul.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://amd.hammf.cn

[U05] Py：列表去重且保序
来源：http://wzg.ehwqpu.com

list(dict.fromkeys(arr))
来源：http://xuz.yangfankeji.com

[U06] Py：合并两个字典
来源：http://mua.cqqwz.cn

{**a, **b}
来源：http://vyb.yvedp.cn

[U07] Py：反转字典键值
来源：http://bfp.yuanzhike.top

{v: k for k, v in d.items()}
来源：http://fwq.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://zrd.zdqjudy.top

[y for x in nested for y in x]
来源：http://fjx.ydzc1.top

[U09] Py：字典取最大值的键
来源：http://uvq.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://qpo.sufxvd.cn

[U10] Py：按值排序字典
来源：http://bar.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hiy.gotoacloud.top

[U11] Py：生成器表达式
来源：http://eze.yj20258.top

(x * 2 for x in arr)
来源：http://ygt.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ipz.wangdashe.top

Counter(arr).most_common(3)
来源：http://sbu.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://isa.fanxiaobao.xyz

deque(maxlen=10)
来源：http://jqr.zycfv.cn

[U14] Py：分组收集到列表
来源：http://ulo.sysykeji.top

defaultdict(list)
来源：http://iwa.wangdashe.top

[U15] Py：高精度计时
来源：http://hzm.jinghuilouyu.cn

t = time.perf_counter()
来源：http://cvu.vehdjk.com

[U16] Py：命令行参数解析
来源：http://oup.meibo888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oxd.jinghuilouyu.cn

[U17] Py：初始化日志
来源：http://lqc.daxiang520.top

logging.basicConfig(level=logging.INFO)
来源：http://rci.cqqwz.cn

[U18] Py：预编译正则
来源：http://voc.xuetiantiany.cn

pat = re.compile(r"\d+")
来源：http://fro.yj20258888.top

[U19] Py：正则替换带回调
来源：http://mrq.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jkt.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://aqn.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://rcb.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://fld.vehdjk.com

@contextlib.contextmanager
来源：http://gcz.zdbjq.cn

[U22] Py：矩阵转置
来源：http://xzq.haohaochexian.top

list(zip(*m))
来源：http://zoq.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://uyn.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://krq.chenjidiqi.icu

[U24] Py：路径操作
来源：http://yxv.feifeiyinyue.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qot.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://gde.yfazqb.com

csv.DictReader(f)
来源：http://pfa.sweek.top

[U26] Py：并发下载
来源：http://jzm.hnxiangtu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tbd.redwolf501.top

[U27] Py：异步 HTTP
来源：http://hrz.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://yfe.shangyingyoupin.top

[U28] Py：类型别名
来源：http://usz.sxryk.cn

UserId = int
来源：http://pqa.zdbjq.cn

[U29] Py：属性校验
来源：http://pqn.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://lyf.yuxming.cn

[U30] Py：数据类
来源：http://ihl.yfazqb.com

@dataclass(slots=True)
来源：http://may.jinyuanbaomall.cn

[U31] Py：单测
来源：http://ixh.fehbvm.com

python -m pytest -q
来源：http://lvu.gaohongyu789.top

[U32] Py：代码格式化
来源：http://pmb.yongpay.top

ruff format . && ruff check --fix .
来源：http://ocd.yueranfly.top

[U33] Py：打包发布
来源：http://kdc.gzhubu.top

python -m build  （依赖 pyproject.toml）
来源：http://irj.yuxming.cn

[U34] Py：判断编码
来源：http://ejz.tianlin.xyz

chardet.detect(raw)
来源：http://nis.yj202588.top

[U35] Py：发送邮件
来源：http://vgu.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vwi.andypj.xyz

[U36] Py：定时任务
来源：http://sfr.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://agm.sufxvd.cn

[U37] Py：读写 Excel
来源：http://lla.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qfv.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://jwr.jqgfzy.top

Path(__file__).resolve().parent
来源：http://wqt.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://nrc.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://knm.316326.xyz

[U40] Py：打印到标准错误
来源：http://rtr.nanxuanxn.top

print("err", file=sys.stderr)
来源：http://dgu.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://fyr.epnwcf.com

composer init;  composer require guzzlehttp/guzzle
来源：http://myb.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://rnj.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ivz.jqgfzy.top

[U43] PHP：声明命名空间
来源：http://jkt.ehwqpu.com

namespace App\Http;
来源：http://djh.316326.xyz

[U44] PHP：开启严格类型
来源：http://ynr.52xcode.cn

declare(strict_types=1);
来源：http://ahr.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://ocv.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hmb.uphjek.com

[U46] PHP：可空类型
来源：http://iog.c1oappe.top

?string $name = null
来源：http://tor.chenlongwang.top

[U47] PHP：联合类型
来源：http://hhr.smart0.xyz

int|string $id
来源：http://eul.gotoacloud.top

[U48] PHP：纯枚举
来源：http://cps.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dqp.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://bhn.hongshengwenyu.top

public readonly string $name
来源：http://hrs.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://rfk.daxiang520.top

public function __construct(private int $id) {}
来源：http://snw.ppjwa.cn

[U51] PHP：数组解构
来源：http://kiw.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://yir.yueranfly.top

[U52] PHP：箭头函数
来源：http://okm.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://vel.yonumen.top

[U53] PHP：空合并运算符
来源：http://vwb.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://lxg.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://fmx.ctjpmb.com

$obj?->method()
来源：http://svf.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://jki.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://llp.sufxvd.cn

[U56] PHP：命名参数
来源：http://nzl.yueranfly.top

f(a: 1, b: 2)
来源：http://qhm.yonumen.top

[U57] PHP：字符串插值
来源：http://ueh.xuanzx.com

"值: {$a}"
来源：http://pff.zdbjq.cn

[U58] PHP：数组三件套
来源：http://dqc.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hum.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://sba.jinghuilouyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://skg.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://wnc.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fgk.pengpengdd.cyou

[U61] PHP：正则
来源：http://hkx.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ati.gzhubu.top

[U62] PHP：日期对象
来源：http://yzz.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mnh.yuxming.cn

[U63] PHP：文件读写
来源：http://bjy.cqqwz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hsb.meibo888.top

[U64] PHP：目录遍历
来源：http://nxz.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://vtq.ybcxt.top


<!-- 参考信息 -->