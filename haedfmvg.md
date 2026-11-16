代发 wailian999

[S43] C++：智能指针
来源：http://hfp.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://xbh.chenjidiqi.icu

[S44] C++：引用传参
来源：http://dij.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://fwd.pengpengdd.cyou

[S45] C++：lambda
来源：http://ksv.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hrg.guowangkeji.top

[S46] C++：函数模板
来源：http://lhn.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rbe.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://qwc.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uch.meibo888.top

[S48] C++：逐行读文件
来源：http://fjn.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://pcy.redwolf501.top

while (std::getline(in, line)) { }
来源：http://grl.jinghuilouyu.cn

[S49] C++：写文件
来源：http://hlj.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xtj.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://swa.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gru.tian-w.cn

[S51] C++：显式类型转换
来源：http://ifl.ivvv.top

static_cast<double>(a) / b
来源：http://cji.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://zpy.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://ovr.yongpay.top

[S53] C++：移动语义
来源：http://ewk.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://ouu.jinqigfzy.top

[S54] C++：异常处理
来源：http://jhc.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gro.wangdashe.top

[S55] C++：结构化绑定
来源：http://laz.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ymz.jianghu66.top

[S56] C++：optional
来源：http://mxo.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rrr.zhengqikj.top

[S57] C++：编译期常量
来源：http://bsf.shuidangran.top

constexpr int N = 10;
来源：http://ubk.jinqigfzy.top

[S58] C++：命名空间
来源：http://sla.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://zhd.sysykeji.top

[S59] C++：静态断言
来源：http://njv.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ccw.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://kgl.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rnr.yanxiufei.cn

================================================================================
来源：http://wie.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bsl.yanxiufei.cn

================================================================================
来源：http://lzy.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://obo.yuanzhike.top

println("Hello")
来源：http://alh.mhx1999.top

[T02] Kotlin：变量
来源：http://vgl.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yaw.yongpay.top

[T03] Kotlin：字符串模板
来源：http://lep.nanxuanxn.top

"值: $b"
来源：http://ufb.havefunace.top

[T04] Kotlin：空安全
来源：http://hbj.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://hcr.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://lad.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://maf.hfpthk.cn

[T06] Kotlin：集合映射
来源：http://ees.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dsg.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://iyu.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fpf.mhx1999.top

[T08] Kotlin：数据类
来源：http://gbx.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://eaw.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://tpa.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://eio.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://ebx.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hos.kuanghao11.cn

[T11] Kotlin：协程
来源：http://mcf.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hni.yuxming.cn

[T12] Kotlin：解构声明
来源：http://nxu.gogol.net.cn

val (a, b) = Pair(1, 2)
来源：http://zeg.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://zwy.sweek.top

val m = mapOf("a" to 1)
来源：http://kcc.fengsongda.top

[T14] Kotlin：循环
来源：http://puh.fengsongda.top

for (i in 1..10) println(i)
来源：http://qjx.gogol.net.cn

[T15] Kotlin：接口
来源：http://ufo.ydzc1.top

interface Shape { fun area(): Double }
来源：http://tom.jinqigfzy.top

[T16] Swift：Hello World
来源：http://xdf.yj202588.top

print("Hello")
来源：http://oeh.dashuyun.cn

[T17] Swift：变量与常量
来源：http://nhn.hnxiangtu.top

var a = 1;  let b = 2
来源：http://mun.zhengqikj.top

[T18] Swift：字符串插值
来源：http://ffx.zhoulong.xyz

"值: \(b)"
来源：http://yqj.fktsv.cn

[T19] Swift：可选绑定
来源：http://jzq.wangdashe.top

if let n = opt { print(n) }
来源：http://tha.hammf.cn

[T20] Swift：数组操作
来源：http://dqi.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://qkl.zhixingplan.top

[T21] Swift：遍历
来源：http://pdo.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://oco.shzxlz.cn

[T22] Swift：字典
来源：http://twx.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://toc.hnqzz.top

[T23] Swift：函数
来源：http://tzn.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nit.yonumen.top

[T24] Swift：闭包
来源：http://yzs.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ufd.tianlin.xyz

[T25] Swift：结构体
来源：http://azg.guannengcc.top

struct P { var x: Int }
来源：http://zuh.jqgufenzy.top

[T26] Swift：类与重写
来源：http://zmr.smart0.xyz

class A: Base { override func f() {} }
来源：http://avr.chenjidiqi.icu

[T27] Swift：错误处理
来源：http://ymv.52xcode.cn

do { try f() } catch { print(error) }
来源：http://ytj.yanxiufei.cn

[T28] Swift：枚举
来源：http://wxs.vehdjk.com

enum Color { case red, green }
来源：http://ugl.cashguo.top

[T29] Swift：guard 提前返回
来源：http://lez.sweek.top

guard let x = opt else { return }
来源：http://wjg.yj20258.top

[T30] Swift：协议
来源：http://ipr.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://rlu.zdqjudy.top

[T31] Lua：Hello World
来源：http://hyq.yj20258.top

print("Hello")
来源：http://hft.gogol.net.cn

[T32] Lua：局部变量
来源：http://bgo.jinghuilouyu.cn

local a = 1
来源：http://fhf.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://kjw.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dzi.zhijiandao.cn

[T34] Lua：遍历表
来源：http://now.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rsn.chenzaomai.com

[T35] Lua：字典表
来源：http://lee.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://scg.jqgfzy.top

[T36] Lua：函数
来源：http://yru.c1oappe.top

function add(a, b) return a + b end
来源：http://qsw.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://vxn.meibo888.top

"a" .. "b"
来源：http://scy.andypj.xyz

[T38] Lua：条件
来源：http://aun.yongpay.top

if x > 0 then print("正") end
来源：http://pnd.ivvv.top

[T39] Lua：模式匹配
来源：http://uxq.yangfankeji.com

string.find(s, "%d+")
来源：http://xwj.ywan-chungtsiang.top

[T40] Lua：元表
来源：http://rol.vehdjk.com

setmetatable({}, { __index = base })
来源：http://dwq.hesvh.cn

[T41] Perl：Hello World
来源：http://poz.hnqzz.top

print "Hello\n";
来源：http://thu.redwolf501.top

[T42] Perl：变量类型
来源：http://cia.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://udb.9152youxi.cn

[T43] Perl：字符串插值
来源：http://drw.xuanzx.com

"值: $a"
来源：http://tyl.zhengqikj.top

[T44] Perl：条件
来源：http://dcg.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://jdt.pengpengdd.cyou

[T45] Perl：数组遍历
来源：http://jqo.meibo888.top

for my $x (@arr) { print $x; }
来源：http://frc.yj20258.top

[T46] Perl：哈希操作
来源：http://bzu.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zux.chenzaomai.com

[T47] Perl：正则捕获
来源：http://ujb.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://duz.nanxinkj.top

[T48] Perl：正则替换
来源：http://agr.sxryk.cn

$s =~ s/old/new/g;
来源：http://txl.cashguo.top

[T49] Perl：函数
来源：http://zve.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rzi.yj20258.top

[T50] Perl：逐行读文件
来源：http://fwv.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rif.dianchejie.cn

while (my $line = <$fh>) { print $line; }
来源：http://qbb.epnwcf.com

[T51] Scala：Hello World
来源：http://pmz.zhengqikj.top

println("Hello")
来源：http://osg.jqgufenzy.top

[T52] Scala：变量
来源：http://yml.andypj.xyz

val a = 1;  var b = 2
来源：http://uxo.jiagoushi.top

[T53] Scala：字符串插值
来源：http://sbq.tian-w.cn

s"值: $b"
来源：http://dtm.yueranfly.top

[T54] Scala：集合映射
来源：http://unh.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://met.sweek.top

[T55] Scala：集合过滤
来源：http://nnv.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uhc.yj202588.top

[T56] Scala：样例类
来源：http://jwc.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://wct.tianlin.xyz

[T57] Scala：模式匹配
来源：http://srs.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://evp.hywenlv.cn

[T58] Scala：函数定义
来源：http://xcs.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://ykx.hnqzz.top

[T59] Scala：循环
来源：http://fzc.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://ljz.ehwqpu.com

[T60] Scala：折叠
来源：http://bms.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bgx.ivvv.top

================================================================================
来源：http://mch.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kbd.aibaodan.cn

================================================================================
来源：http://zdy.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://gzy.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://yco.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://yze.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://crg.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://fcc.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://iul.sweek.top

[U04] Py：变量调试打印
来源：http://bue.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yvk.meibo888.top

[U05] Py：列表去重且保序
来源：http://kyp.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://wno.hesvh.cn

[U06] Py：合并两个字典
来源：http://ylj.yonumen.top

{**a, **b}
来源：http://ytx.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://gdr.yueranfly.top

{v: k for k, v in d.items()}
来源：http://phy.svipenyu.cn

[U08] Py：展平二维列表
来源：http://blx.svipenyu.cn

[y for x in nested for y in x]
来源：http://gjb.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://ltl.ydzc1.top

max(d, key=d.get)
来源：http://fil.hywenlv.cn

[U10] Py：按值排序字典
来源：http://mqv.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cwn.hesvh.cn

[U11] Py：生成器表达式
来源：http://iiz.gaohongyu789.top

(x * 2 for x in arr)
来源：http://epr.yanxiufei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rlq.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://nog.epnwcf.com

[U13] Py：固定长度队列
来源：http://xas.zhoulong.xyz

deque(maxlen=10)
来源：http://vnb.zhaomingkeji.xyz

[U14] Py：分组收集到列表
来源：http://qib.guowangkeji.top

defaultdict(list)
来源：http://jdd.jyoumei.cn

[U15] Py：高精度计时
来源：http://tfl.dashuyun.cn

t = time.perf_counter()
来源：http://cgx.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://lke.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ldy.fengsongda.top

[U17] Py：初始化日志
来源：http://gwg.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://qdf.nanxinkj.top

[U18] Py：预编译正则
来源：http://npp.c1oappe.top

pat = re.compile(r"\d+")
来源：http://cmw.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://ugl.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jbz.jinghuilouyu.cn

[U20] Py：缓存函数结果
来源：http://qne.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://pal.ywan-chungtsiang.top

[U21] Py：自定义上下文管理器
来源：http://fqd.ydjk.org.cn

@contextlib.contextmanager
来源：http://oxh.316326.xyz

[U22] Py：矩阵转置
来源：http://rwd.jqgufenzy.top

list(zip(*m))
来源：http://bhw.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://ooo.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oof.havefunace.top

[U24] Py：路径操作
来源：http://kty.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dbq.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://hij.9152youxi.cn

csv.DictReader(f)
来源：http://yyg.ivvv.top

[U26] Py：并发下载
来源：http://lqt.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ykg.birdmap.top

[U27] Py：异步 HTTP
来源：http://kzn.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://djw.jianghu66.top

[U28] Py：类型别名
来源：http://rru.nwbrower.top

UserId = int
来源：http://hma.ppjwa.cn

[U29] Py：属性校验
来源：http://ixq.hfpthk.cn

@property 与 @x.setter 配合
来源：http://pdc.pycfn.com

[U30] Py：数据类
来源：http://fwn.jianghu66.top

@dataclass(slots=True)
来源：http://pcd.hammf.cn

[U31] Py：单测
来源：http://dwb.uphjek.com

python -m pytest -q
来源：http://nlm.zdbjq.cn

[U32] Py：代码格式化
来源：http://tid.birdmap.top

ruff format . && ruff check --fix .
来源：http://xup.sweek.top

[U33] Py：打包发布
来源：http://nuc.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://pnb.zhoulong.xyz

[U34] Py：判断编码
来源：http://kxm.yj20258.top

chardet.detect(raw)
来源：http://vza.zhixingplan.top

[U35] Py：发送邮件
来源：http://qtu.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wkx.yj20258888.top

[U36] Py：定时任务
来源：http://mjn.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://kdz.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://rxq.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://hxa.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://wsj.gogol.net.cn

Path(__file__).resolve().parent
来源：http://cep.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://swq.zycfv.cn

sys.stdout.isatty()
来源：http://hgm.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://wmr.yonumen.top

print("err", file=sys.stderr)
来源：http://jth.vehdjk.com

[U41] PHP：初始化 Composer 项目
来源：http://ekf.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cwy.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://hcd.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ljn.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://xlj.sxryk.cn

namespace App\Http;
来源：http://ctw.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://ydk.ehwqpu.com

declare(strict_types=1);
来源：http://akv.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://lhr.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dqc.jqgfzy.top

[U46] PHP：可空类型
来源：http://tlx.ydjk.org.cn

?string $name = null
来源：http://slj.zhoulong.xyz

[U47] PHP：联合类型
来源：http://pmn.chenzaomai.com

int|string $id
来源：http://stc.yvedp.cn

[U48] PHP：纯枚举
来源：http://yms.dashuyun.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://brt.shzxlz.cn

[U49] PHP：只读属性
来源：http://avm.fzhhl.top

public readonly string $name
来源：http://inl.redwolf501.top

[U50] PHP：构造器属性提升
来源：http://hwb.yueranfly.top

public function __construct(private int $id) {}
来源：http://kbz.yj20258.top

[U51] PHP：数组解构
来源：http://gkv.uphjek.com

[$a, $b] = $arr;
来源：http://qkc.cheryme.top

[U52] PHP：箭头函数
来源：http://fue.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://usd.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://crs.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://rwe.hnxiangtu.top

[U54] PHP：空安全调用
来源：http://yat.aibaodan.cn

$obj?->method()
来源：http://eii.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://jvp.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ejq.jiagoushi.top

[U56] PHP：命名参数
来源：http://hhb.vqdsnc.cn

f(a: 1, b: 2)
来源：http://dcg.jinghuilouyu.cn

[U57] PHP：字符串插值
来源：http://koq.meibo888.top

"值: {$a}"
来源：http://dab.316326.xyz

[U58] PHP：数组三件套
来源：http://voy.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zvi.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://pxj.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bki.gogol.net.cn

[U60] PHP：JSON 编解码
来源：http://lik.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wbx.andypj.xyz

[U61] PHP：正则
来源：http://fux.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ynm.zhixingplan.top

[U62] PHP：日期对象
来源：http://tge.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://psm.gzhubu.top

[U63] PHP：文件读写
来源：http://akd.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://euj.c1oappe.top

[U64] PHP：目录遍历
来源：http://xnx.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://lix.andypj.xyz

[U65] PHP：会话
来源：http://jak.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://upz.fengsongda.top

[U66] PHP：设置 Cookie
来源：http://zoa.yongpay.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hox.tanke756.top

[U67] PHP：处理文件上传
来源：http://jxe.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://axp.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://qgz.chenlongwang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vhw.zhongyouzk.top


<!-- 参考信息 -->