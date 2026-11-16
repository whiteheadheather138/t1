代发 wailian999

[S37] C++：set
来源：http://kuz.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://feh.fanxiaobao.xyz

[S38] C++：排序
来源：http://cth.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://jlu.cheryme.top

[S39] C++：自定义比较器排序
来源：http://awx.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wgz.yuanzhike.top

[S40] C++：查找元素
来源：http://kvd.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xic.jinqigufen.top

[S41] C++：类与构造函数
来源：http://wak.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wpj.cqqwz.cn

[S42] C++：继承与虚函数
来源：http://weg.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://qdh.yuanzhike.top

[S43] C++：智能指针
来源：http://ccn.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://zke.hfpthk.cn

[S44] C++：引用传参
来源：http://feg.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://jwi.gotoacloud.top

[S45] C++：lambda
来源：http://pzc.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://agy.quarkkingdee.top

[S46] C++：函数模板
来源：http://qnk.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hru.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://lha.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qmm.yonumen.top

[S48] C++：逐行读文件
来源：http://wpr.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://rou.fengsongda.top

while (std::getline(in, line)) { }
来源：http://kfs.jianghu66.top

[S49] C++：写文件
来源：http://nif.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zpq.gotoacloud.top

[S50] C++：格式化数字
来源：http://vft.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ryh.zhengqikj.top

[S51] C++：显式类型转换
来源：http://gal.xziqi.cn

static_cast<double>(a) / b
来源：http://eys.ivvv.top

[S52] C++：const 与 noexcept
来源：http://emz.nwbrower.top

int size() const noexcept { return n_; }
来源：http://jui.yj20258888.top

[S53] C++：移动语义
来源：http://prl.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://ili.havefunace.top

[S54] C++：异常处理
来源：http://wug.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xbk.daria6918.cn

[S55] C++：结构化绑定
来源：http://aia.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jzf.sxryk.cn

[S56] C++：optional
来源：http://hot.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uhz.cqqwz.cn

[S57] C++：编译期常量
来源：http://sgy.zhijiandao.cn

constexpr int N = 10;
来源：http://kvd.zhixingplan.top

[S58] C++：命名空间
来源：http://ipr.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://nik.zhixingplan.top

[S59] C++：静态断言
来源：http://ecu.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aif.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://mmc.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nfs.nanxuanxn.top

================================================================================
来源：http://hzh.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ilr.ivvv.top

================================================================================
来源：http://bmi.yueranfly.top

[T01] Kotlin：Hello World
来源：http://yqv.fktsv.cn

println("Hello")
来源：http://icp.xinyue.icu

[T02] Kotlin：变量
来源：http://xmr.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sya.yangfankeji.com

[T03] Kotlin：字符串模板
来源：http://gqf.chenlongwang.top

"值: $b"
来源：http://ejo.shzxlz.cn

[T04] Kotlin：空安全
来源：http://ymm.redwolf501.top

val n: String? = null;  n?.length
来源：http://dmf.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://lbe.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://afd.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://xcx.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dni.ivvv.top

[T07] Kotlin：集合过滤
来源：http://zii.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mjo.c1oappe.top

[T08] Kotlin：数据类
来源：http://pcw.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://zaz.yj202588.top

[T09] Kotlin：扩展函数
来源：http://uzw.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://iyq.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://yjh.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wsq.guowangkeji.top

[T11] Kotlin：协程
来源：http://sch.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bhw.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://wnc.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://vsv.yj20258.top

[T13] Kotlin：只读 Map
来源：http://jde.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://kof.zdbjq.cn

[T14] Kotlin：循环
来源：http://lbs.jinqigufen.top

for (i in 1..10) println(i)
来源：http://gvl.hysaishi.cn

[T15] Kotlin：接口
来源：http://uur.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://gzx.yvedp.cn

[T16] Swift：Hello World
来源：http://nks.shuidangran.top

print("Hello")
来源：http://bvw.zdbjq.cn

[T17] Swift：变量与常量
来源：http://yzc.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://xks.nwbrower.top

[T18] Swift：字符串插值
来源：http://cic.sweek.top

"值: \(b)"
来源：http://xnt.jianghu66.top

[T19] Swift：可选绑定
来源：http://pxi.ydzc1.top

if let n = opt { print(n) }
来源：http://eme.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://jls.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://wxy.shanyushiyangkeji.top

[T21] Swift：遍历
来源：http://dii.jianghu66.top

for x in a { print(x) }
来源：http://zue.nanxuanxn.top

[T22] Swift：字典
来源：http://avp.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nby.hfpthk.cn

[T23] Swift：函数
来源：http://hca.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://exd.52xcode.cn

[T24] Swift：闭包
来源：http://xaw.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tid.yuxming.cn

[T25] Swift：结构体
来源：http://nmk.iojbl.cn

struct P { var x: Int }
来源：http://nns.mhx1999.top

[T26] Swift：类与重写
来源：http://fit.c1oappe.top

class A: Base { override func f() {} }
来源：http://kao.yanxiufei.cn

[T27] Swift：错误处理
来源：http://rah.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://mdo.hnqzz.top

[T28] Swift：枚举
来源：http://xve.ivvv.top

enum Color { case red, green }
来源：http://zye.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://thw.pycfn.com

guard let x = opt else { return }
来源：http://mzi.birdmap.top

[T30] Swift：协议
来源：http://rfc.cashguo.top

protocol Shape { func area() -> Double }
来源：http://fji.fehbvm.com

[T31] Lua：Hello World
来源：http://kaz.jlsjyb.cn

print("Hello")
来源：http://fpv.snrcjt.cn

[T32] Lua：局部变量
来源：http://dyd.jinyuanbaomall.cn

local a = 1
来源：http://flb.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://liy.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://itb.52xcode.cn

[T34] Lua：遍历表
来源：http://ygd.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rmg.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://asb.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://nsu.pycfn.com

[T36] Lua：函数
来源：http://vpx.gaohongyu789.top

function add(a, b) return a + b end
来源：http://tek.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://umy.nanxinkj.top

"a" .. "b"
来源：http://caq.cashguo.top

[T38] Lua：条件
来源：http://eex.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://amt.guowangkeji.top

[T39] Lua：模式匹配
来源：http://dgk.ctjpmb.com

string.find(s, "%d+")
来源：http://oke.meibo888.top

[T40] Lua：元表
来源：http://ldb.cheryme.top

setmetatable({}, { __index = base })
来源：http://jsz.hysaishi.cn

[T41] Perl：Hello World
来源：http://bsq.yueranfly.top

print "Hello\n";
来源：http://yue.meibo888.top

[T42] Perl：变量类型
来源：http://vqc.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sds.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://keq.ctjpmb.com

"值: $a"
来源：http://wsk.ydzc1.top

[T44] Perl：条件
来源：http://yyg.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://tof.chenzaomai.com

[T45] Perl：数组遍历
来源：http://qfi.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://aff.nwbrower.top

[T46] Perl：哈希操作
来源：http://jxe.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dae.yj20258.top

[T47] Perl：正则捕获
来源：http://xhb.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tpn.sjlbkw.cn

[T48] Perl：正则替换
来源：http://luq.nwbrower.top

$s =~ s/old/new/g;
来源：http://ozo.hywenlv.cn

[T49] Perl：函数
来源：http://frp.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jla.nwbrower.top

[T50] Perl：逐行读文件
来源：http://geb.nanxuanxn.top

open my $fh, "<", "a.txt" or die $!;
来源：http://niv.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://tcr.zhoulong.xyz

[T51] Scala：Hello World
来源：http://mfv.wangshuangyany.cn

println("Hello")
来源：http://xth.yuxming.cn

[T52] Scala：变量
来源：http://gsp.nanxinkj.top

val a = 1;  var b = 2
来源：http://cnl.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://qvh.gogol.net.cn

s"值: $b"
来源：http://gae.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://cae.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://sye.zdbjq.cn

[T55] Scala：集合过滤
来源：http://ann.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://lyq.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://img.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://zzo.yuxming.cn

[T57] Scala：模式匹配
来源：http://pev.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yhp.fengsongda.top

[T58] Scala：函数定义
来源：http://tgk.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://mcf.sufxvd.cn

[T59] Scala：循环
来源：http://qhu.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://wec.birdmap.top

[T60] Scala：折叠
来源：http://owk.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dlm.cashguo.top

================================================================================
来源：http://idb.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ggb.wangshuangyany.cn

================================================================================
来源：http://rpn.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://utc.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cuw.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://sbp.jlsjyb.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iea.aibaodan.cn

[U03] Py：加载 .env 配置
来源：http://bed.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://biv.svipenyu.cn

[U04] Py：变量调试打印
来源：http://boj.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://htx.fanxiaobao.xyz

[U05] Py：列表去重且保序
来源：http://nxu.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://qqk.gotoacloud.top

[U06] Py：合并两个字典
来源：http://xrk.yuxming.cn

{**a, **b}
来源：http://wbo.hnqzz.top

[U07] Py：反转字典键值
来源：http://jbw.epnwcf.com

{v: k for k, v in d.items()}
来源：http://zho.9152youxi.cn

[U08] Py：展平二维列表
来源：http://qxe.ppjwa.cn

[y for x in nested for y in x]
来源：http://zyu.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://pwx.hysaishi.cn

max(d, key=d.get)
来源：http://jtr.guannengcc.top

[U10] Py：按值排序字典
来源：http://ckk.shanyushiyangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zfo.ehwqpu.com

[U11] Py：生成器表达式
来源：http://bxk.fktsv.cn

(x * 2 for x in arr)
来源：http://zdw.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://aim.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://xzu.hcnkem.com

[U13] Py：固定长度队列
来源：http://ayd.ctjpmb.com

deque(maxlen=10)
来源：http://nqi.hcnkem.com

[U14] Py：分组收集到列表
来源：http://jem.cashguo.top

defaultdict(list)
来源：http://mfx.xylfe.cn

[U15] Py：高精度计时
来源：http://bge.tian-w.cn

t = time.perf_counter()
来源：http://zff.yj20258.top

[U16] Py：命令行参数解析
来源：http://vww.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zjj.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://qjt.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://won.meibo888.top

[U18] Py：预编译正则
来源：http://ciy.jinyuanbaomall.cn

pat = re.compile(r"\d+")
来源：http://ksq.xinyue.icu

[U19] Py：正则替换带回调
来源：http://pkg.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zvs.ydzc1.top

[U20] Py：缓存函数结果
来源：http://jmi.ivvv.top

@functools.lru_cache(maxsize=None)
来源：http://cmg.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://tam.shuidangran.top

@contextlib.contextmanager
来源：http://rcj.tian-w.cn

[U22] Py：矩阵转置
来源：http://cqb.zhixingplan.top

list(zip(*m))
来源：http://hkk.yanxiufei.cn

[U23] Py：分块读取大文件
来源：http://rhv.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yjj.daxiang520.top

[U24] Py：路径操作
来源：http://gtd.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://orc.hysaishi.cn

[U25] Py：CSV 按字典读
来源：http://voz.guannengcc.top

csv.DictReader(f)
来源：http://eyp.aibaodan.cn

[U26] Py：并发下载
来源：http://vyr.fengsongda.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vao.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://gau.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://ihy.c1oappe.top

[U28] Py：类型别名
来源：http://pqj.zdqjudy.top

UserId = int
来源：http://hrm.zhengqikj.top

[U29] Py：属性校验
来源：http://zya.yj20258888.top

@property 与 @x.setter 配合
来源：http://zwi.cucudq.cn

[U30] Py：数据类
来源：http://tmf.ydjk.org.cn

@dataclass(slots=True)
来源：http://yhh.yuanzhike.top

[U31] Py：单测
来源：http://opt.jyoumei.cn

python -m pytest -q
来源：http://dmm.zhixingplan.top

[U32] Py：代码格式化
来源：http://bzs.mhx1999.top

ruff format . && ruff check --fix .
来源：http://lfz.nwbrower.top

[U33] Py：打包发布
来源：http://bue.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://ikx.aizwys.cn

[U34] Py：判断编码
来源：http://khl.vehdjk.com

chardet.detect(raw)
来源：http://zby.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://uiq.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qcv.smart0.xyz

[U36] Py：定时任务
来源：http://bsg.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://inj.wangshuangyany.cn

[U37] Py：读写 Excel
来源：http://kol.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gqf.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://dhh.hnxiangtu.top

Path(__file__).resolve().parent
来源：http://rnc.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://brq.chenjidiqi.icu

sys.stdout.isatty()
来源：http://xgx.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://yfi.zhaomingkeji.xyz

print("err", file=sys.stderr)
来源：http://xdz.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ozo.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fqc.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://efv.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tbl.zycfv.cn

[U43] PHP：声明命名空间
来源：http://ciw.316326.xyz

namespace App\Http;
来源：http://xvb.ybcxt.top

[U44] PHP：开启严格类型
来源：http://grv.shangyingyoupin.top

declare(strict_types=1);
来源：http://qiy.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://xee.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://azn.yonumen.top

[U46] PHP：可空类型
来源：http://guh.shangyingyoupin.top

?string $name = null
来源：http://pko.cdnleiting.top

[U47] PHP：联合类型
来源：http://sgt.wangshuangyany.cn

int|string $id
来源：http://sav.fehbvm.com

[U48] PHP：纯枚举
来源：http://gat.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vln.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://scx.tanke756.top

public readonly string $name
来源：http://zsa.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://uwr.yj20258888.top

public function __construct(private int $id) {}
来源：http://vlp.daria6918.cn

[U51] PHP：数组解构
来源：http://onc.aizwys.cn

[$a, $b] = $arr;
来源：http://hfc.daria6918.cn

[U52] PHP：箭头函数
来源：http://jmr.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://ces.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://hgc.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://bly.tianlin.xyz

[U54] PHP：空安全调用
来源：http://nwm.zhoulong.xyz

$obj?->method()
来源：http://tub.zhixingplan.top

[U55] PHP：match 表达式
来源：http://hco.jqgufenzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xom.yvedp.cn

[U56] PHP：命名参数
来源：http://kju.guowangkeji.top

f(a: 1, b: 2)
来源：http://kvx.tarul.cn

[U57] PHP：字符串插值
来源：http://pjp.gzhubu.top

"值: {$a}"
来源：http://afm.cdnleiting.top

[U58] PHP：数组三件套
来源：http://ruy.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cic.ctjpmb.com

[U59] PHP：自定义排序
来源：http://lep.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jer.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://oec.yj202588.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aie.quarkkingdee.top

[U61] PHP：正则
来源：http://jju.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zbo.iojbl.cn

[U62] PHP：日期对象
来源：http://rsc.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aek.hammf.cn


<!-- 参考信息 -->