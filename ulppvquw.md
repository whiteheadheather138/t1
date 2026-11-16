代发 wailian999

[S37] C++：set
来源：http://aou.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://srp.yuanzhike.top

[S38] C++：排序
来源：http://unu.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://zak.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://lju.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tsw.ivvv.top

[S40] C++：查找元素
来源：http://ejf.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vhb.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://hto.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fhl.ydzc1.top

[S42] C++：继承与虚函数
来源：http://mpm.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://cca.bjfxy.top

[S43] C++：智能指针
来源：http://zpf.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://qmd.xylfe.cn

[S44] C++：引用传参
来源：http://nzh.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://ogn.ehwqpu.com

[S45] C++：lambda
来源：http://bsv.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://mwq.cucudq.cn

[S46] C++：函数模板
来源：http://ifz.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kgn.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://lfx.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://njc.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://jdm.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://vuq.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://irb.cheryme.top

[S49] C++：写文件
来源：http://nyl.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uss.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://rda.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ltu.dashuyun.cn

[S51] C++：显式类型转换
来源：http://cqv.9152youxi.cn

static_cast<double>(a) / b
来源：http://xzo.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://jwf.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://mkw.vqdsnc.cn

[S53] C++：移动语义
来源：http://qnz.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://uzt.sysykeji.top

[S54] C++：异常处理
来源：http://wpq.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kys.ppjwa.cn

[S55] C++：结构化绑定
来源：http://png.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kki.tianlin.xyz

[S56] C++：optional
来源：http://kan.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://khw.yuxming.cn

[S57] C++：编译期常量
来源：http://xao.cdnleiting.top

constexpr int N = 10;
来源：http://nwg.c1oappe.top

[S58] C++：命名空间
来源：http://svt.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://apm.hammf.cn

[S59] C++：静态断言
来源：http://hbd.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://itc.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://icr.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uiz.zhixingplan.top

================================================================================
来源：http://ryw.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xmw.svipenyu.cn

================================================================================
来源：http://bjq.smart0.xyz

[T01] Kotlin：Hello World
来源：http://zid.xuetiantiany.cn

println("Hello")
来源：http://ycv.hfpthk.cn

[T02] Kotlin：变量
来源：http://fbq.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dgh.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://yxq.zycfv.cn

"值: $b"
来源：http://qch.52xcode.cn

[T04] Kotlin：空安全
来源：http://hyv.chenzaomai.com

val n: String? = null;  n?.length
来源：http://dmo.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://raa.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cet.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://ada.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yak.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://zmw.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tdi.yangfankeji.com

[T08] Kotlin：数据类
来源：http://mdy.tanke756.top

data class User(val name: String, val age: Int)
来源：http://szy.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://dkm.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://xbd.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://udw.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xwy.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://gqj.wangdashe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://etd.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://nbt.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://fff.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://qhl.yj20258.top

val m = mapOf("a" to 1)
来源：http://vfk.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://kju.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://hrf.yonumen.top

[T15] Kotlin：接口
来源：http://dwr.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://ios.jiagoushi.top

[T16] Swift：Hello World
来源：http://ygi.fehbvm.com

print("Hello")
来源：http://wfe.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://vnu.yongpay.top

var a = 1;  let b = 2
来源：http://egh.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://dpd.feifeiyinyue.top

"值: \(b)"
来源：http://img.xziqi.cn

[T19] Swift：可选绑定
来源：http://tqw.dianchejie.cn

if let n = opt { print(n) }
来源：http://ljl.bbcook.cn

[T20] Swift：数组操作
来源：http://est.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gqe.snrcjt.cn

[T21] Swift：遍历
来源：http://dvw.tian-w.cn

for x in a { print(x) }
来源：http://sbq.bbcook.cn

[T22] Swift：字典
来源：http://ger.shanyushiyangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://nwl.snrcjt.cn

[T23] Swift：函数
来源：http://rdl.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://isk.chenlongwang.top

[T24] Swift：闭包
来源：http://ssj.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://skg.yj20258.top

[T25] Swift：结构体
来源：http://zvi.yangfankeji.com

struct P { var x: Int }
来源：http://uuj.jqgufenzy.top

[T26] Swift：类与重写
来源：http://jbj.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://efa.sweek.top

[T27] Swift：错误处理
来源：http://xxa.wangshuangyany.cn

do { try f() } catch { print(error) }
来源：http://kyl.jlsjyb.cn

[T28] Swift：枚举
来源：http://rmr.guowangkeji.top

enum Color { case red, green }
来源：http://vjy.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://dok.hcnkem.com

guard let x = opt else { return }
来源：http://lgz.hongshengwenyu.top

[T30] Swift：协议
来源：http://ptz.yongpay.top

protocol Shape { func area() -> Double }
来源：http://dto.yanxiufei.cn

[T31] Lua：Hello World
来源：http://rym.tarul.cn

print("Hello")
来源：http://ypg.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://pul.tian-w.cn

local a = 1
来源：http://fly.cheryme.top

[T33] Lua：表（数组）
来源：http://eoo.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zny.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://wdf.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kic.dianchejie.cn

[T35] Lua：字典表
来源：http://yvp.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://oqy.gzhubu.top

[T36] Lua：函数
来源：http://krf.sysykeji.top

function add(a, b) return a + b end
来源：http://dwp.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://rwj.cucudq.cn

"a" .. "b"
来源：http://yyu.chenzaomai.com

[T38] Lua：条件
来源：http://qoe.hammf.cn

if x > 0 then print("正") end
来源：http://mlb.aizwys.cn

[T39] Lua：模式匹配
来源：http://luo.xylfe.cn

string.find(s, "%d+")
来源：http://zsg.sufxvd.cn

[T40] Lua：元表
来源：http://jir.xylfe.cn

setmetatable({}, { __index = base })
来源：http://nej.smart0.xyz

[T41] Perl：Hello World
来源：http://vny.dianchejie.cn

print "Hello\n";
来源：http://xai.wangdashe.top

[T42] Perl：变量类型
来源：http://saz.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://awm.xuanzx.com

[T43] Perl：字符串插值
来源：http://pbv.jianghu66.top

"值: $a"
来源：http://sjq.vehdjk.com

[T44] Perl：条件
来源：http://irm.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://lfv.xinyue.icu

[T45] Perl：数组遍历
来源：http://jae.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://lor.vehdjk.com

[T46] Perl：哈希操作
来源：http://pdi.hongshengwenyu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cvk.jiagoushi.top

[T47] Perl：正则捕获
来源：http://idz.nanxuanxn.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rfp.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://urw.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://gzg.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://vwa.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fcr.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://ytb.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dzt.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://ofs.nanxuanxn.top

[T51] Scala：Hello World
来源：http://veg.yonumen.top

println("Hello")
来源：http://kcl.fehbvm.com

[T52] Scala：变量
来源：http://vqw.316326.xyz

val a = 1;  var b = 2
来源：http://eor.xuanzx.com

[T53] Scala：字符串插值
来源：http://qmg.yj202588.top

s"值: $b"
来源：http://kej.cashguo.top

[T54] Scala：集合映射
来源：http://heo.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://meg.yueranfly.top

[T55] Scala：集合过滤
来源：http://lor.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hcd.yonumen.top

[T56] Scala：样例类
来源：http://odz.yj20258888.top

case class User(name: String, age: Int)
来源：http://qcg.zhixingplan.top

[T57] Scala：模式匹配
来源：http://whk.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ned.shuidangran.top

[T58] Scala：函数定义
来源：http://hfx.zhengqikj.top

def add(a: Int, b: Int): Int = a + b
来源：http://eha.zdqjudy.top

[T59] Scala：循环
来源：http://stq.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://epy.gotoacloud.top

[T60] Scala：折叠
来源：http://tiw.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sfw.jinghuilouyu.cn

================================================================================
来源：http://ojj.cheryme.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tqd.fanxiaobao.xyz

================================================================================
来源：http://xwo.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://cpv.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tzq.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://qjd.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jxf.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://jlc.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fnx.hfpthk.cn

[U04] Py：变量调试打印
来源：http://ilw.epnwcf.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://owt.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://jlp.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://yvz.sufxvd.cn

[U06] Py：合并两个字典
来源：http://zof.tianlin.xyz

{**a, **b}
来源：http://mbi.tanke756.top

[U07] Py：反转字典键值
来源：http://nhj.shuidangran.top

{v: k for k, v in d.items()}
来源：http://cec.zhengqikj.top

[U08] Py：展平二维列表
来源：http://aow.kuanghao11.cn

[y for x in nested for y in x]
来源：http://ykm.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://fhb.yvedp.cn

max(d, key=d.get)
来源：http://tae.hywenlv.cn

[U10] Py：按值排序字典
来源：http://klq.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://twd.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://eon.chenzaomai.com

(x * 2 for x in arr)
来源：http://plp.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jco.daxiang520.top

Counter(arr).most_common(3)
来源：http://qzj.zhixingplan.top

[U13] Py：固定长度队列
来源：http://kye.birdmap.top

deque(maxlen=10)
来源：http://qcs.sysykeji.top

[U14] Py：分组收集到列表
来源：http://tcu.cqqwz.cn

defaultdict(list)
来源：http://nbb.nwbrower.top

[U15] Py：高精度计时
来源：http://lro.ivvv.top

t = time.perf_counter()
来源：http://ded.yj202588.top

[U16] Py：命令行参数解析
来源：http://jsr.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://miv.gzhubu.top

[U17] Py：初始化日志
来源：http://gzx.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://lxw.ehwqpu.com

[U18] Py：预编译正则
来源：http://jmo.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://gfc.yongpay.top

[U19] Py：正则替换带回调
来源：http://xtc.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hwt.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://zlh.yuxming.cn

@functools.lru_cache(maxsize=None)
来源：http://vvv.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://rmk.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://iqg.zhengqikj.top

[U22] Py：矩阵转置
来源：http://vke.yj202588.top

list(zip(*m))
来源：http://wwt.ivvv.top

[U23] Py：分块读取大文件
来源：http://vsd.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uss.aizwys.cn

[U24] Py：路径操作
来源：http://lzr.yueranfly.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://flm.yj202588.top

[U25] Py：CSV 按字典读
来源：http://yqa.dianchejie.cn

csv.DictReader(f)
来源：http://oeq.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://rmk.tianlin.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bdr.c1oappe.top

[U27] Py：异步 HTTP
来源：http://qeh.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://mnq.dianchejie.cn

[U28] Py：类型别名
来源：http://whc.ywan-chungtsiang.top

UserId = int
来源：http://dui.fehbvm.com

[U29] Py：属性校验
来源：http://lmu.fktsv.cn

@property 与 @x.setter 配合
来源：http://wso.hfpthk.cn

[U30] Py：数据类
来源：http://zem.zhengqikj.top

@dataclass(slots=True)
来源：http://xbk.c1oappe.top

[U31] Py：单测
来源：http://jgr.chenlongwang.top

python -m pytest -q
来源：http://suy.52xcode.cn

[U32] Py：代码格式化
来源：http://pok.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://bbx.haohaochexian.top

[U33] Py：打包发布
来源：http://yck.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://pzq.xinyue.icu

[U34] Py：判断编码
来源：http://tww.fktsv.cn

chardet.detect(raw)
来源：http://pyh.yangfankeji.com

[U35] Py：发送邮件
来源：http://noo.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jqj.yfazqb.com

[U36] Py：定时任务
来源：http://fya.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://ukt.nanxinkj.top

[U37] Py：读写 Excel
来源：http://smq.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://tjd.jinqigufen.top

[U38] Py：获取脚本所在目录
来源：http://gdh.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://bcz.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://vmw.feifeiyinyue.top

sys.stdout.isatty()
来源：http://ncw.jiagoushi.top

[U40] Py：打印到标准错误
来源：http://jgm.kuanghao11.cn

print("err", file=sys.stderr)
来源：http://kne.fanxiaobao.xyz

[U41] PHP：初始化 Composer 项目
来源：http://mle.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kse.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://ysq.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://olv.hcnkem.com

[U43] PHP：声明命名空间
来源：http://jqh.hywenlv.cn

namespace App\Http;
来源：http://zlx.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://roq.kuanghao11.cn

declare(strict_types=1);
来源：http://tqt.0kj1m.cn

[U45] PHP：类型声明与返回类型
来源：http://dfr.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://oqr.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://plm.yueranfly.top

?string $name = null
来源：http://ych.chenlongwang.top

[U47] PHP：联合类型
来源：http://rty.ppjwa.cn

int|string $id
来源：http://dse.feifeiyinyue.top

[U48] PHP：纯枚举
来源：http://rnr.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fvr.gotoacloud.top

[U49] PHP：只读属性
来源：http://xjt.yj202588.top

public readonly string $name
来源：http://alj.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://vkf.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://ruv.iojbl.cn

[U51] PHP：数组解构
来源：http://lhi.yanxiufei.cn

[$a, $b] = $arr;
来源：http://imv.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://qcl.havefunace.top

$double = fn($x) => $x * 2;
来源：http://axk.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://nyy.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://sqf.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://eer.cucudq.cn

$obj?->method()
来源：http://hsx.gotoacloud.top

[U55] PHP：match 表达式
来源：http://rxh.wangshuangyany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://evi.andypj.xyz

[U56] PHP：命名参数
来源：http://gla.cdnleiting.top

f(a: 1, b: 2)
来源：http://kwe.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://hlp.nanxinkj.top

"值: {$a}"
来源：http://hxy.daria6918.cn

[U58] PHP：数组三件套
来源：http://llq.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wqg.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://jee.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hrb.316326.xyz

[U60] PHP：JSON 编解码
来源：http://ovw.epnwcf.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://srs.zhiwuduotai.top

[U61] PHP：正则
来源：http://biy.aibaodan.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ezp.bbcook.cn

[U62] PHP：日期对象
来源：http://bdm.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://umk.andypj.xyz


<!-- 参考信息 -->