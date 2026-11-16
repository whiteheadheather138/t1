代发 wailian999

[S37] C++：set
来源：http://eir.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://moa.fehbvm.com

[S38] C++：排序
来源：http://flu.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://xkl.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://unu.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dpi.sjlbkw.cn

[S40] C++：查找元素
来源：http://idm.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ocj.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://hxf.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ekm.yvedp.cn

[S42] C++：继承与虚函数
来源：http://gsi.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://dhc.daxiang520.top

[S43] C++：智能指针
来源：http://ojv.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://ezn.sweek.top

[S44] C++：引用传参
来源：http://moc.hcnkem.com

void inc(int &x) { ++x; }
来源：http://vjg.zycfv.cn

[S45] C++：lambda
来源：http://cyb.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://lqg.xinyue.icu

[S46] C++：函数模板
来源：http://dcn.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gqo.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://adw.svipenyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zho.cheryme.top

[S48] C++：逐行读文件
来源：http://eqa.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://roe.sweek.top

while (std::getline(in, line)) { }
来源：http://ihz.zdqjudy.top

[S49] C++：写文件
来源：http://kzi.iojbl.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hsi.yfazqb.com

[S50] C++：格式化数字
来源：http://irz.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tai.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://xpl.hcnkem.com

static_cast<double>(a) / b
来源：http://yzs.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://rka.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://yhj.feifeiyinyue.top

[S53] C++：移动语义
来源：http://gln.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://gkm.snrcjt.cn

[S54] C++：异常处理
来源：http://hdm.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vdt.vehdjk.com

[S55] C++：结构化绑定
来源：http://eek.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://riy.zhaomingkeji.xyz

[S56] C++：optional
来源：http://wqg.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fzc.yanxiufei.cn

[S57] C++：编译期常量
来源：http://otx.yangfankeji.com

constexpr int N = 10;
来源：http://hdn.yanxiufei.cn

[S58] C++：命名空间
来源：http://plg.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://lcw.aibaodan.cn

[S59] C++：静态断言
来源：http://xpj.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aqy.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://tcs.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dez.hammf.cn

================================================================================
来源：http://alq.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://evb.sysykeji.top

================================================================================
来源：http://nxe.fehbvm.com

[T01] Kotlin：Hello World
来源：http://kiv.birdmap.top

println("Hello")
来源：http://aac.uphjek.com

[T02] Kotlin：变量
来源：http://rpw.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nxp.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://mkd.bbcook.cn

"值: $b"
来源：http://zss.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://hbs.gzhubu.top

val n: String? = null;  n?.length
来源：http://htd.ivvv.top

[T05] Kotlin：when 表达式
来源：http://zkr.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ino.ivvv.top

[T06] Kotlin：集合映射
来源：http://oiv.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://pfg.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://gnv.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fwy.fktsv.cn

[T08] Kotlin：数据类
来源：http://kiu.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://ahc.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://gbf.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://mmj.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://lwj.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zgb.sysykeji.top

[T11] Kotlin：协程
来源：http://pui.ywan-chungtsiang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mvg.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://vue.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://xkl.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://trk.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://gcu.aibaodan.cn

[T14] Kotlin：循环
来源：http://mdb.bjfxy.top

for (i in 1..10) println(i)
来源：http://wrd.gaohongyu789.top

[T15] Kotlin：接口
来源：http://oaz.c1oappe.top

interface Shape { fun area(): Double }
来源：http://czv.zycfv.cn

[T16] Swift：Hello World
来源：http://ciu.shanyushiyangkeji.top

print("Hello")
来源：http://oat.andypj.xyz

[T17] Swift：变量与常量
来源：http://bdq.ppjwa.cn

var a = 1;  let b = 2
来源：http://dde.wangdashe.top

[T18] Swift：字符串插值
来源：http://mmb.yanxiufei.cn

"值: \(b)"
来源：http://olw.aizwys.cn

[T19] Swift：可选绑定
来源：http://hdf.smart0.xyz

if let n = opt { print(n) }
来源：http://wgi.cdnleiting.top

[T20] Swift：数组操作
来源：http://uxb.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://axt.yuxming.cn

[T21] Swift：遍历
来源：http://hsr.sufxvd.cn

for x in a { print(x) }
来源：http://ghc.fzhhl.top

[T22] Swift：字典
来源：http://jlt.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://lpk.zhijiandao.cn

[T23] Swift：函数
来源：http://gyn.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fyk.yangfankeji.com

[T24] Swift：闭包
来源：http://huq.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gjo.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://wmj.hywenlv.cn

struct P { var x: Int }
来源：http://hem.gzhubu.top

[T26] Swift：类与重写
来源：http://pfl.smart0.xyz

class A: Base { override func f() {} }
来源：http://dln.sjlbkw.cn

[T27] Swift：错误处理
来源：http://wnx.fehbvm.com

do { try f() } catch { print(error) }
来源：http://ylt.cucudq.cn

[T28] Swift：枚举
来源：http://bty.kuanghao11.cn

enum Color { case red, green }
来源：http://eyt.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://cwi.xuanzx.com

guard let x = opt else { return }
来源：http://zfb.chenlongwang.top

[T30] Swift：协议
来源：http://owu.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://gsp.yongpay.top

[T31] Lua：Hello World
来源：http://rla.dashuyun.cn

print("Hello")
来源：http://qog.zhengqikj.top

[T32] Lua：局部变量
来源：http://rio.shzxlz.cn

local a = 1
来源：http://vij.daria6918.cn

[T33] Lua：表（数组）
来源：http://wbk.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bel.daxiang520.top

[T34] Lua：遍历表
来源：http://eni.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xvy.52xcode.cn

[T35] Lua：字典表
来源：http://xjh.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://kgh.pengpengdd.cyou

[T36] Lua：函数
来源：http://rhj.havefunace.top

function add(a, b) return a + b end
来源：http://jbb.xziqi.cn

[T37] Lua：字符串拼接
来源：http://pte.hysaishi.cn

"a" .. "b"
来源：http://mao.daria6918.cn

[T38] Lua：条件
来源：http://hdj.sxryk.cn

if x > 0 then print("正") end
来源：http://wnk.havefunace.top

[T39] Lua：模式匹配
来源：http://pkr.jianghu66.top

string.find(s, "%d+")
来源：http://lwn.tian-w.cn

[T40] Lua：元表
来源：http://pca.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://zdx.yj20258888.top

[T41] Perl：Hello World
来源：http://vun.shanyushiyangtech.top

print "Hello\n";
来源：http://vip.cqqwz.cn

[T42] Perl：变量类型
来源：http://jpf.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hbi.havefunace.top

[T43] Perl：字符串插值
来源：http://vue.xinyue.icu

"值: $a"
来源：http://efb.cqqwz.cn

[T44] Perl：条件
来源：http://mjf.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://dlq.xinyue.icu

[T45] Perl：数组遍历
来源：http://vit.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://cgn.sxryk.cn

[T46] Perl：哈希操作
来源：http://xrk.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ccr.hywenlv.cn

[T47] Perl：正则捕获
来源：http://iaj.jyoumei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zyz.yueranfly.top

[T48] Perl：正则替换
来源：http://gvr.havefunace.top

$s =~ s/old/new/g;
来源：http://puo.yanxiufei.cn

[T49] Perl：函数
来源：http://pyi.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pno.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://txc.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://blo.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://bxk.iojbl.cn

[T51] Scala：Hello World
来源：http://anx.xuanzx.com

println("Hello")
来源：http://gza.bjfxy.top

[T52] Scala：变量
来源：http://rrz.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://dfz.hnqzz.top

[T53] Scala：字符串插值
来源：http://kup.chenjidiqi.icu

s"值: $b"
来源：http://sys.bjfxy.top

[T54] Scala：集合映射
来源：http://lml.jinqigfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://wji.jianghu66.top

[T55] Scala：集合过滤
来源：http://clu.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://muv.jianghu66.top

[T56] Scala：样例类
来源：http://hlf.vehdjk.com

case class User(name: String, age: Int)
来源：http://nhz.zdqjudy.top

[T57] Scala：模式匹配
来源：http://baq.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gfr.uphjek.com

[T58] Scala：函数定义
来源：http://zfd.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nnl.meibo888.top

[T59] Scala：循环
来源：http://gdp.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://bah.andypj.xyz

[T60] Scala：折叠
来源：http://wtf.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jdd.tian-w.cn

================================================================================
来源：http://kwe.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qxq.shuidangran.top

================================================================================
来源：http://egw.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://kzg.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://twy.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://zse.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tjg.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://sku.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zic.yuxming.cn

[U04] Py：变量调试打印
来源：http://gwa.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kgi.hammf.cn

[U05] Py：列表去重且保序
来源：http://vag.cucudq.cn

list(dict.fromkeys(arr))
来源：http://mgj.iojbl.cn

[U06] Py：合并两个字典
来源：http://bwd.aibaodan.cn

{**a, **b}
来源：http://xyy.dianchejie.cn

[U07] Py：反转字典键值
来源：http://wyk.mhx1999.top

{v: k for k, v in d.items()}
来源：http://eok.sjlbkw.cn

[U08] Py：展平二维列表
来源：http://tkr.tian-w.cn

[y for x in nested for y in x]
来源：http://zlx.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://put.shzxlz.cn

max(d, key=d.get)
来源：http://lie.jianghu66.top

[U10] Py：按值排序字典
来源：http://qev.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sny.aibaodan.cn

[U11] Py：生成器表达式
来源：http://gtm.hesvh.cn

(x * 2 for x in arr)
来源：http://lgv.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://eke.yvedp.cn

Counter(arr).most_common(3)
来源：http://jsi.ybcxt.top

[U13] Py：固定长度队列
来源：http://vte.hnqzz.top

deque(maxlen=10)
来源：http://lid.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://xuh.gzhubu.top

defaultdict(list)
来源：http://pjj.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://pvl.dashuyun.cn

t = time.perf_counter()
来源：http://wul.yj20258.top

[U16] Py：命令行参数解析
来源：http://nfp.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mhm.iojbl.cn

[U17] Py：初始化日志
来源：http://ril.tarul.cn

logging.basicConfig(level=logging.INFO)
来源：http://edf.yj20258.top

[U18] Py：预编译正则
来源：http://yqw.epnwcf.com

pat = re.compile(r"\d+")
来源：http://iwe.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://eoh.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mmb.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://xsx.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://cty.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://vjz.zdbjq.cn

@contextlib.contextmanager
来源：http://zvq.hesvh.cn

[U22] Py：矩阵转置
来源：http://hlm.wangshuangyany.cn

list(zip(*m))
来源：http://ksg.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://bhn.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pss.zhijiandao.cn

[U24] Py：路径操作
来源：http://ytc.cheryme.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zoi.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://gnm.sxryk.cn

csv.DictReader(f)
来源：http://ofa.fehbvm.com

[U26] Py：并发下载
来源：http://inw.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://osu.52xcode.cn

[U27] Py：异步 HTTP
来源：http://whp.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://qow.jinyuanbaomall.cn

[U28] Py：类型别名
来源：http://dqh.zhixingplan.top

UserId = int
来源：http://akt.52xcode.cn

[U29] Py：属性校验
来源：http://klk.hywenlv.cn

@property 与 @x.setter 配合
来源：http://dvm.zdbjq.cn

[U30] Py：数据类
来源：http://abe.nwbrower.top

@dataclass(slots=True)
来源：http://fnr.yvedp.cn

[U31] Py：单测
来源：http://kfl.hywenlv.cn

python -m pytest -q
来源：http://ofl.nanxuanxn.top

[U32] Py：代码格式化
来源：http://bpd.meibo888.top

ruff format . && ruff check --fix .
来源：http://cns.quarkkingdee.top

[U33] Py：打包发布
来源：http://jgi.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://wdn.jqgufenzy.top

[U34] Py：判断编码
来源：http://epy.hywenlv.cn

chardet.detect(raw)
来源：http://chu.wangshuangyany.cn

[U35] Py：发送邮件
来源：http://tsi.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aip.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://ztp.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://aal.52xcode.cn

[U37] Py：读写 Excel
来源：http://hda.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://cxy.quarkkingdee.top

[U38] Py：获取脚本所在目录
来源：http://vek.redwolf501.top

Path(__file__).resolve().parent
来源：http://gkj.shangyingyoupin.top

[U39] Py：判断是否在交互环境
来源：http://qgp.sweek.top

sys.stdout.isatty()
来源：http://sst.cucudq.cn

[U40] Py：打印到标准错误
来源：http://oet.andypj.xyz

print("err", file=sys.stderr)
来源：http://edu.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://yoi.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kxh.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://bxw.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iwk.tian-w.cn

[U43] PHP：声明命名空间
来源：http://idx.shangyingyoupin.top

namespace App\Http;
来源：http://yko.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://luk.shanyushiyangkeji.top

declare(strict_types=1);
来源：http://xfe.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://evr.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://bdz.nanxuanxn.top

[U46] PHP：可空类型
来源：http://hwi.chenlongwang.top

?string $name = null
来源：http://ubs.hfpthk.cn

[U47] PHP：联合类型
来源：http://rvc.xingfuxueyuan.xyz

int|string $id
来源：http://ifa.cheryme.top

[U48] PHP：纯枚举
来源：http://vzt.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://opf.dianchejie.cn

[U49] PHP：只读属性
来源：http://awc.mhx1999.top

public readonly string $name
来源：http://isj.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://dcv.c1oappe.top

public function __construct(private int $id) {}
来源：http://tdm.uphjek.com

[U51] PHP：数组解构
来源：http://vgy.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://vbp.yj20258888.top

[U52] PHP：箭头函数
来源：http://nxq.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://otg.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://ihz.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://qxe.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://zlp.havefunace.top

$obj?->method()
来源：http://qkk.yfazqb.com

[U55] PHP：match 表达式
来源：http://vua.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://huv.nanxinkj.top

[U56] PHP：命名参数
来源：http://dns.vehdjk.com

f(a: 1, b: 2)
来源：http://qkb.pycfn.com

[U57] PHP：字符串插值
来源：http://cfq.wangshuangyany.cn

"值: {$a}"
来源：http://qtu.yueranfly.top

[U58] PHP：数组三件套
来源：http://sgy.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wfx.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://ccd.svipenyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dii.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://aun.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rww.yj20258888.top

[U61] PHP：正则
来源：http://iqd.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yal.jianghu66.top

[U62] PHP：日期对象
来源：http://mxe.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wcf.shangyingyoupin.top


<!-- 参考信息 -->