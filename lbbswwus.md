代发 wailian999

[S35] C++：map
来源：http://vui.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yna.aizwys.cn

[S36] C++：unordered_map
来源：http://lde.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ktu.feifeiyinyue.top

[S37] C++：set
来源：http://hpa.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vgi.hammf.cn

[S38] C++：排序
来源：http://vbx.havefunace.top

std::sort(v.begin(), v.end());
来源：http://hul.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://pwu.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iyy.cashguo.top

[S40] C++：查找元素
来源：http://zta.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aba.mhx1999.top

[S41] C++：类与构造函数
来源：http://kor.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mju.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://ghj.hywenlv.cn

class B : public Base { public: void f() override {} };
来源：http://jkz.zhiwuduotai.top

[S43] C++：智能指针
来源：http://iiu.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://kkf.guowangkeji.top

[S44] C++：引用传参
来源：http://buq.sysykeji.top

void inc(int &x) { ++x; }
来源：http://vfd.smart0.xyz

[S45] C++：lambda
来源：http://itd.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://ixp.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://bjs.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rbv.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://fkr.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fzq.zhengqikj.top

[S48] C++：逐行读文件
来源：http://hhs.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://day.mhx1999.top

while (std::getline(in, line)) { }
来源：http://ovj.tanke756.top

[S49] C++：写文件
来源：http://ywm.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dru.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://cby.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qve.nanxinkj.top

[S51] C++：显式类型转换
来源：http://gex.xuanzx.com

static_cast<double>(a) / b
来源：http://nrg.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://ehv.yj202588.top

int size() const noexcept { return n_; }
来源：http://dyl.zhoulong.xyz

[S53] C++：移动语义
来源：http://ykf.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://mov.yj202588.top

[S54] C++：异常处理
来源：http://xqw.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nzu.wangdashe.top

[S55] C++：结构化绑定
来源：http://osg.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ntv.jinqigfzy.top

[S56] C++：optional
来源：http://bpo.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ihm.sufxvd.cn

[S57] C++：编译期常量
来源：http://osj.hesvh.cn

constexpr int N = 10;
来源：http://zqt.sysykeji.top

[S58] C++：命名空间
来源：http://kbh.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://wum.sxryk.cn

[S59] C++：静态断言
来源：http://awa.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zub.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://kuf.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://plo.52xcode.cn

================================================================================
来源：http://fxi.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eyx.jqgfzy.top

================================================================================
来源：http://jhy.vehdjk.com

[T01] Kotlin：Hello World
来源：http://zkg.chenlongwang.top

println("Hello")
来源：http://nzr.vqdsnc.cn

[T02] Kotlin：变量
来源：http://tse.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mgm.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://xfl.fanxiaobao.xyz

"值: $b"
来源：http://aze.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://uwx.haohaochexian.top

val n: String? = null;  n?.length
来源：http://ojd.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://nvy.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://emo.gzhubu.top

[T06] Kotlin：集合映射
来源：http://vxw.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mvv.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://btz.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vqd.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://sgh.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://qwx.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://fyp.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://rgn.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://tut.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cre.zhongyouzk.top

[T11] Kotlin：协程
来源：http://iqp.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rxo.fktsv.cn

[T12] Kotlin：解构声明
来源：http://vpc.xuanzx.com

val (a, b) = Pair(1, 2)
来源：http://bji.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://wgs.guannengcc.top

val m = mapOf("a" to 1)
来源：http://ttt.pycfn.com

[T14] Kotlin：循环
来源：http://tip.zycfv.cn

for (i in 1..10) println(i)
来源：http://yqe.aizwys.cn

[T15] Kotlin：接口
来源：http://lde.smart0.xyz

interface Shape { fun area(): Double }
来源：http://cnz.jinqigfzy.top

[T16] Swift：Hello World
来源：http://lte.316326.xyz

print("Hello")
来源：http://kmp.yj20258.top

[T17] Swift：变量与常量
来源：http://zrq.zhengqikj.top

var a = 1;  let b = 2
来源：http://dzu.yueranfly.top

[T18] Swift：字符串插值
来源：http://nhv.fengsongda.top

"值: \(b)"
来源：http://cyk.cqqwz.cn

[T19] Swift：可选绑定
来源：http://dgp.wangdashe.top

if let n = opt { print(n) }
来源：http://efo.hysaishi.cn

[T20] Swift：数组操作
来源：http://hkm.jinqigfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://mqu.guowangkeji.top

[T21] Swift：遍历
来源：http://slo.andypj.xyz

for x in a { print(x) }
来源：http://rxp.redwolf501.top

[T22] Swift：字典
来源：http://adh.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://exu.andypj.xyz

[T23] Swift：函数
来源：http://ywb.c1oappe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ibx.vqdsnc.cn

[T24] Swift：闭包
来源：http://eak.jlsjyb.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://quk.guowangkeji.top

[T25] Swift：结构体
来源：http://foy.pengpengdd.cyou

struct P { var x: Int }
来源：http://okd.zycfv.cn

[T26] Swift：类与重写
来源：http://tpu.xuanzx.com

class A: Base { override func f() {} }
来源：http://cpb.fzhhl.top

[T27] Swift：错误处理
来源：http://otd.xylfe.cn

do { try f() } catch { print(error) }
来源：http://xgc.yfazqb.com

[T28] Swift：枚举
来源：http://zst.jiagoushi.top

enum Color { case red, green }
来源：http://hns.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://lvo.mhx1999.top

guard let x = opt else { return }
来源：http://alw.aibaodan.cn

[T30] Swift：协议
来源：http://yjw.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://ogn.fehbvm.com

[T31] Lua：Hello World
来源：http://zws.bjfxy.top

print("Hello")
来源：http://iey.meibo888.top

[T32] Lua：局部变量
来源：http://sfi.zhoulong.xyz

local a = 1
来源：http://plg.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://pxo.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lzw.yuanzhike.top

[T34] Lua：遍历表
来源：http://xrc.chenlongwang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pts.hcnkem.com

[T35] Lua：字典表
来源：http://zrp.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://pia.zhengqikj.top

[T36] Lua：函数
来源：http://icx.zhoulong.xyz

function add(a, b) return a + b end
来源：http://ret.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://psz.tian-w.cn

"a" .. "b"
来源：http://gzx.vqdsnc.cn

[T38] Lua：条件
来源：http://eze.bjfxy.top

if x > 0 then print("正") end
来源：http://yjy.fehbvm.com

[T39] Lua：模式匹配
来源：http://wty.jinqigufen.top

string.find(s, "%d+")
来源：http://heo.uphjek.com

[T40] Lua：元表
来源：http://dta.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://lud.tarul.cn

[T41] Perl：Hello World
来源：http://moc.nanxinkj.top

print "Hello\n";
来源：http://elc.fengsongda.top

[T42] Perl：变量类型
来源：http://byd.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://byc.nanxinkj.top

[T43] Perl：字符串插值
来源：http://gwz.guowangkeji.top

"值: $a"
来源：http://gce.yj20258888.top

[T44] Perl：条件
来源：http://zot.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://cmn.havefunace.top

[T45] Perl：数组遍历
来源：http://xjg.fzhhl.top

for my $x (@arr) { print $x; }
来源：http://sog.iojbl.cn

[T46] Perl：哈希操作
来源：http://jsw.guannengcc.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lzk.gogol.net.cn

[T47] Perl：正则捕获
来源：http://lwm.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jxw.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://anf.gogol.net.cn

$s =~ s/old/new/g;
来源：http://vsw.quarkkingdee.top

[T49] Perl：函数
来源：http://jof.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bby.hnxiangtu.top

[T50] Perl：逐行读文件
来源：http://ikm.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mtw.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://jnd.cashguo.top

[T51] Scala：Hello World
来源：http://vra.kuanghao11.cn

println("Hello")
来源：http://zvx.chenjidiqi.icu

[T52] Scala：变量
来源：http://hhp.yonumen.top

val a = 1;  var b = 2
来源：http://yhu.fengsongda.top

[T53] Scala：字符串插值
来源：http://dhn.0kj1m.cn

s"值: $b"
来源：http://rbt.vqdsnc.cn

[T54] Scala：集合映射
来源：http://cgu.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://zmb.sysykeji.top

[T55] Scala：集合过滤
来源：http://ozj.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dtq.aibaodan.cn

[T56] Scala：样例类
来源：http://pls.tian-w.cn

case class User(name: String, age: Int)
来源：http://kyp.52xcode.cn

[T57] Scala：模式匹配
来源：http://abv.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lfz.jinqigfzy.top

[T58] Scala：函数定义
来源：http://syp.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://eug.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://fio.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://pup.feifeiyinyue.top

[T60] Scala：折叠
来源：http://psk.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://laj.jyoumei.cn

================================================================================
来源：http://bwk.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vmd.chenlongwang.top

================================================================================
来源：http://vvd.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://hsp.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://gbr.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://gdx.sufxvd.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zwg.sjlbkw.cn

[U03] Py：加载 .env 配置
来源：http://nnz.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jpm.yuxming.cn

[U04] Py：变量调试打印
来源：http://omi.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cft.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://swo.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://niw.zdbjq.cn

[U06] Py：合并两个字典
来源：http://tsz.uphjek.com

{**a, **b}
来源：http://nrw.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://sxn.hnqzz.top

{v: k for k, v in d.items()}
来源：http://jok.feifeiyinyue.top

[U08] Py：展平二维列表
来源：http://xot.jinqigfzy.top

[y for x in nested for y in x]
来源：http://qqg.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://qad.hcnkem.com

max(d, key=d.get)
来源：http://ssp.9152youxi.cn

[U10] Py：按值排序字典
来源：http://lod.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oko.jinyuanbaomall.cn

[U11] Py：生成器表达式
来源：http://uak.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://ajs.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://hde.cdnleiting.top

Counter(arr).most_common(3)
来源：http://hbz.redwolf501.top

[U13] Py：固定长度队列
来源：http://nrf.52xcode.cn

deque(maxlen=10)
来源：http://wkr.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://apr.hesvh.cn

defaultdict(list)
来源：http://bfi.gogol.net.cn

[U15] Py：高精度计时
来源：http://xpa.yanxiufei.cn

t = time.perf_counter()
来源：http://vuq.ppjwa.cn

[U16] Py：命令行参数解析
来源：http://gxk.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sqk.yj20258.top

[U17] Py：初始化日志
来源：http://ouo.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://wqq.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://zqz.xylfe.cn

pat = re.compile(r"\d+")
来源：http://kex.ehwqpu.com

[U19] Py：正则替换带回调
来源：http://avj.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ekm.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://mnx.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://ret.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://zkb.fktsv.cn

@contextlib.contextmanager
来源：http://myp.cucudq.cn

[U22] Py：矩阵转置
来源：http://qhy.zhengqikj.top

list(zip(*m))
来源：http://ien.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://jsw.vehdjk.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hqo.cucudq.cn

[U24] Py：路径操作
来源：http://eqp.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://viy.tanke756.top

[U25] Py：CSV 按字典读
来源：http://wbx.yanxiufei.cn

csv.DictReader(f)
来源：http://glx.yongpay.top

[U26] Py：并发下载
来源：http://ljg.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://thj.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://pwg.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://wnr.316326.xyz

[U28] Py：类型别名
来源：http://zwk.gaohongyu789.top

UserId = int
来源：http://vpe.yj202588.top

[U29] Py：属性校验
来源：http://bhs.yj20258.top

@property 与 @x.setter 配合
来源：http://oxc.gogol.net.cn

[U30] Py：数据类
来源：http://ppm.zhiwuduotai.top

@dataclass(slots=True)
来源：http://lku.smart0.xyz

[U31] Py：单测
来源：http://ebi.vehdjk.com

python -m pytest -q
来源：http://dlv.nwbrower.top

[U32] Py：代码格式化
来源：http://zcq.shuidangran.top

ruff format . && ruff check --fix .
来源：http://vsd.jyoumei.cn

[U33] Py：打包发布
来源：http://hwn.havefunace.top

python -m build  （依赖 pyproject.toml）
来源：http://drf.yj20258888.top

[U34] Py：判断编码
来源：http://ysx.zhoulong.xyz

chardet.detect(raw)
来源：http://apz.ydjk.org.cn

[U35] Py：发送邮件
来源：http://qvj.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mda.snrcjt.cn

[U36] Py：定时任务
来源：http://ipo.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://vvz.havefunace.top

[U37] Py：读写 Excel
来源：http://zep.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://rck.sweek.top

[U38] Py：获取脚本所在目录
来源：http://atq.snrcjt.cn

Path(__file__).resolve().parent
来源：http://uvr.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://faq.dashuyun.cn

sys.stdout.isatty()
来源：http://iaa.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://wcc.yvedp.cn

print("err", file=sys.stderr)
来源：http://yxr.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://ymz.hnqzz.top

composer init;  composer require guzzlehttp/guzzle
来源：http://inv.haohaochexian.top

[U42] PHP：PSR-4 自动加载
来源：http://akg.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zlp.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://inf.jinqigufen.top

namespace App\Http;
来源：http://tel.hcnkem.com

[U44] PHP：开启严格类型
来源：http://wfp.yanxiufei.cn

declare(strict_types=1);
来源：http://zxv.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://sty.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pik.fengsongda.top

[U46] PHP：可空类型
来源：http://qvi.feifeiyinyue.top

?string $name = null
来源：http://rar.hywenlv.cn

[U47] PHP：联合类型
来源：http://ien.ydjk.org.cn

int|string $id
来源：http://thn.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://lgi.daxiang520.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zlh.ivvv.top

[U49] PHP：只读属性
来源：http://axj.c1oappe.top

public readonly string $name
来源：http://trs.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://xaj.tanke756.top

public function __construct(private int $id) {}
来源：http://eqg.shanyushiyangkeji.top

[U51] PHP：数组解构
来源：http://vdq.jiagoushi.top

[$a, $b] = $arr;
来源：http://uif.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://mjq.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://imc.guannengcc.top

[U53] PHP：空合并运算符
来源：http://oyn.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://iur.sjlbkw.cn

[U54] PHP：空安全调用
来源：http://dst.zdqjudy.top

$obj?->method()
来源：http://cjd.yfazqb.com

[U55] PHP：match 表达式
来源：http://guw.ehwqpu.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yui.nwbrower.top

[U56] PHP：命名参数
来源：http://sit.yanxiufei.cn

f(a: 1, b: 2)
来源：http://wkv.9152youxi.cn

[U57] PHP：字符串插值
来源：http://rzq.hnqzz.top

"值: {$a}"
来源：http://dib.birdmap.top

[U58] PHP：数组三件套
来源：http://hcf.9152youxi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kpw.zdbjq.cn

[U59] PHP：自定义排序
来源：http://tgx.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qqg.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://guo.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kfq.haohaochexian.top


<!-- 参考信息 -->