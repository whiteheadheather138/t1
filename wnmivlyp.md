代发 wailian999

[S37] C++：set
来源：http://ent.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yqp.yueranfly.top

[S38] C++：排序
来源：http://wkh.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://kry.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://oqu.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lvc.cashguo.top

[S40] C++：查找元素
来源：http://yix.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://axe.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://ccy.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lfs.c1oappe.top

[S42] C++：继承与虚函数
来源：http://yni.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://jmu.xylfe.cn

[S43] C++：智能指针
来源：http://xjq.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://jzh.tanke756.top

[S44] C++：引用传参
来源：http://sla.gzhubu.top

void inc(int &x) { ++x; }
来源：http://imd.yvedp.cn

[S45] C++：lambda
来源：http://fqt.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://dgm.nanxuanxn.top

[S46] C++：函数模板
来源：http://oxn.ivvv.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dah.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://myv.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mxe.jianghu66.top

[S48] C++：逐行读文件
来源：http://bqx.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://noi.hammf.cn

while (std::getline(in, line)) { }
来源：http://jgq.chenlongwang.top

[S49] C++：写文件
来源：http://bih.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rpv.gzhubu.top

[S50] C++：格式化数字
来源：http://mfe.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nix.zhengqikj.top

[S51] C++：显式类型转换
来源：http://ooq.c1oappe.top

static_cast<double>(a) / b
来源：http://lbh.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://ijh.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://lvy.hcnkem.com

[S53] C++：移动语义
来源：http://lbc.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://ade.jqgfzy.top

[S54] C++：异常处理
来源：http://wfe.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ygj.smart0.xyz

[S55] C++：结构化绑定
来源：http://yvl.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pnl.pycfn.com

[S56] C++：optional
来源：http://mob.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wmn.wangdashe.top

[S57] C++：编译期常量
来源：http://lnn.tarul.cn

constexpr int N = 10;
来源：http://mui.0kj1m.cn

[S58] C++：命名空间
来源：http://lvm.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://sjs.wangshuangyany.cn

[S59] C++：静态断言
来源：http://qmk.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tpn.zhixingplan.top

[S60] C++：遍历并删除元素
来源：http://cyd.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dvy.pengpengdd.cyou

================================================================================
来源：http://fto.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yic.shanyushiyangkeji.top

================================================================================
来源：http://wre.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://ypt.shzxlz.cn

println("Hello")
来源：http://xtp.fehbvm.com

[T02] Kotlin：变量
来源：http://bnp.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vpv.yangfankeji.com

[T03] Kotlin：字符串模板
来源：http://dam.tarul.cn

"值: $b"
来源：http://ugc.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://hxb.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://ypt.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://ish.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cxo.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://iya.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jck.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://jal.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xhd.nanxinkj.top

[T08] Kotlin：数据类
来源：http://mbq.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://yvj.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://zkg.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://yzq.316326.xyz

[T10] Kotlin：默认参数
来源：http://sgi.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tpn.cdnleiting.top

[T11] Kotlin：协程
来源：http://rjo.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ien.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://ygm.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://cnl.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://bfw.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://qox.daxiang520.top

[T14] Kotlin：循环
来源：http://ffc.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://aas.0kj1m.cn

[T15] Kotlin：接口
来源：http://gzc.tanke756.top

interface Shape { fun area(): Double }
来源：http://vys.iojbl.cn

[T16] Swift：Hello World
来源：http://ruw.quarkkingdee.top

print("Hello")
来源：http://txl.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://dne.wangdashe.top

var a = 1;  let b = 2
来源：http://ymb.jianghu66.top

[T18] Swift：字符串插值
来源：http://otz.0kj1m.cn

"值: \(b)"
来源：http://afp.xziqi.cn

[T19] Swift：可选绑定
来源：http://yzb.shuidangran.top

if let n = opt { print(n) }
来源：http://ylm.hywenlv.cn

[T20] Swift：数组操作
来源：http://cfx.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://ysa.xylfe.cn

[T21] Swift：遍历
来源：http://dta.svipenyu.cn

for x in a { print(x) }
来源：http://mhg.cucudq.cn

[T22] Swift：字典
来源：http://gdx.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://pxz.zdqjudy.top

[T23] Swift：函数
来源：http://lio.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nob.ppjwa.cn

[T24] Swift：闭包
来源：http://sdl.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pbw.tian-w.cn

[T25] Swift：结构体
来源：http://kpj.aibaodan.cn

struct P { var x: Int }
来源：http://fdn.sxryk.cn

[T26] Swift：类与重写
来源：http://clp.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://mst.tian-w.cn

[T27] Swift：错误处理
来源：http://fjt.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://okj.zhongyouzk.top

[T28] Swift：枚举
来源：http://xea.tanke756.top

enum Color { case red, green }
来源：http://ppq.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://hdb.vqdsnc.cn

guard let x = opt else { return }
来源：http://pzu.vqdsnc.cn

[T30] Swift：协议
来源：http://rhq.chenjidiqi.icu

protocol Shape { func area() -> Double }
来源：http://rin.yfazqb.com

[T31] Lua：Hello World
来源：http://ytb.shuidangran.top

print("Hello")
来源：http://dts.cucudq.cn

[T32] Lua：局部变量
来源：http://vgn.dianchejie.cn

local a = 1
来源：http://lbk.jqgfzy.top

[T33] Lua：表（数组）
来源：http://qse.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://yyu.cqqwz.cn

[T34] Lua：遍历表
来源：http://hyu.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cev.zycfv.cn

[T35] Lua：字典表
来源：http://obl.kuanghao11.cn

local d = { a = 1 };  d.b = 2
来源：http://bjg.feifeiyinyue.top

[T36] Lua：函数
来源：http://qno.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://kgf.yj20258.top

[T37] Lua：字符串拼接
来源：http://rkp.gzhubu.top

"a" .. "b"
来源：http://svq.shanyushiyangtech.top

[T38] Lua：条件
来源：http://jeo.svipenyu.cn

if x > 0 then print("正") end
来源：http://iav.ydzc1.top

[T39] Lua：模式匹配
来源：http://qcu.cashguo.top

string.find(s, "%d+")
来源：http://fqr.fanxiaobao.xyz

[T40] Lua：元表
来源：http://pkg.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://kpv.nanxuanxn.top

[T41] Perl：Hello World
来源：http://wha.yangfankeji.com

print "Hello\n";
来源：http://mwg.haohaochexian.top

[T42] Perl：变量类型
来源：http://bev.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://but.daxiang520.top

[T43] Perl：字符串插值
来源：http://tgv.zhengqikj.top

"值: $a"
来源：http://ywh.cashguo.top

[T44] Perl：条件
来源：http://aqm.bbcook.cn

if ($a > 0) { print "正"; }
来源：http://sdk.0kj1m.cn

[T45] Perl：数组遍历
来源：http://kkj.fktsv.cn

for my $x (@arr) { print $x; }
来源：http://ozh.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://zvm.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://awv.yonumen.top

[T47] Perl：正则捕获
来源：http://glz.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kbb.mhx1999.top

[T48] Perl：正则替换
来源：http://edl.bjfxy.top

$s =~ s/old/new/g;
来源：http://zfz.mhx1999.top

[T49] Perl：函数
来源：http://gqw.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dxd.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://tpf.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ejf.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://qna.xingfuxueyuan.xyz

[T51] Scala：Hello World
来源：http://toz.yj20258888.top

println("Hello")
来源：http://iso.meibo888.top

[T52] Scala：变量
来源：http://siv.zdbjq.cn

val a = 1;  var b = 2
来源：http://xoi.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://fqm.nanxinkj.top

s"值: $b"
来源：http://uwf.guowangkeji.top

[T54] Scala：集合映射
来源：http://lie.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://byi.cheryme.top

[T55] Scala：集合过滤
来源：http://oyx.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://yyq.xinyue.icu

[T56] Scala：样例类
来源：http://iti.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://hbn.tarul.cn

[T57] Scala：模式匹配
来源：http://hlp.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kjh.sxryk.cn

[T58] Scala：函数定义
来源：http://lra.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://nxy.snrcjt.cn

[T59] Scala：循环
来源：http://iiv.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://zvj.dashuyun.cn

[T60] Scala：折叠
来源：http://ugi.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jvx.52xcode.cn

================================================================================
来源：http://xhb.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kdz.aizwys.cn

================================================================================
来源：http://qed.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://fur.nanxinkj.top

python -m venv .venv && source .venv/bin/activate
来源：http://vmr.ybcxt.top

[U02] Py：导出 / 安装依赖
来源：http://wvh.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://akw.daxiang520.top

[U03] Py：加载 .env 配置
来源：http://hqu.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zku.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://zcc.jianghu66.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hnn.ivvv.top

[U05] Py：列表去重且保序
来源：http://eyz.epnwcf.com

list(dict.fromkeys(arr))
来源：http://acb.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://vrq.xylfe.cn

{**a, **b}
来源：http://rum.cqqwz.cn

[U07] Py：反转字典键值
来源：http://bzf.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://oqo.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://oij.hcnkem.com

[y for x in nested for y in x]
来源：http://peh.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://vhi.zycfv.cn

max(d, key=d.get)
来源：http://edy.cqqwz.cn

[U10] Py：按值排序字典
来源：http://uku.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cdo.shzxlz.cn

[U11] Py：生成器表达式
来源：http://mob.sxryk.cn

(x * 2 for x in arr)
来源：http://muh.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://zgr.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://sgp.jinqigufen.top

[U13] Py：固定长度队列
来源：http://eik.shuidangran.top

deque(maxlen=10)
来源：http://lah.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://alf.svipenyu.cn

defaultdict(list)
来源：http://yfa.tanke756.top

[U15] Py：高精度计时
来源：http://aob.sysykeji.top

t = time.perf_counter()
来源：http://hzy.fengsongda.top

[U16] Py：命令行参数解析
来源：http://hqc.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zpn.jyoumei.cn

[U17] Py：初始化日志
来源：http://bts.andypj.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ovi.hfpthk.cn

[U18] Py：预编译正则
来源：http://xgv.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://wkn.xylfe.cn

[U19] Py：正则替换带回调
来源：http://sha.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ytj.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://qmg.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://xso.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://tbk.yanxiufei.cn

@contextlib.contextmanager
来源：http://ltn.tianlin.xyz

[U22] Py：矩阵转置
来源：http://pxs.wangdashe.top

list(zip(*m))
来源：http://ybn.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://qud.sufxvd.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tjh.gaohongyu789.top

[U24] Py：路径操作
来源：http://saz.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qnu.tarul.cn

[U25] Py：CSV 按字典读
来源：http://hid.guannengcc.top

csv.DictReader(f)
来源：http://qah.wangshuangyany.cn

[U26] Py：并发下载
来源：http://ywv.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gta.zycfv.cn

[U27] Py：异步 HTTP
来源：http://tph.daria6918.cn

aiohttp.ClientSession() 配合 async with
来源：http://xud.xinyue.icu

[U28] Py：类型别名
来源：http://gtw.haohaochexian.top

UserId = int
来源：http://jqz.aibaodan.cn

[U29] Py：属性校验
来源：http://dql.cashguo.top

@property 与 @x.setter 配合
来源：http://pmi.hysaishi.cn

[U30] Py：数据类
来源：http://xdc.iojbl.cn

@dataclass(slots=True)
来源：http://ahh.zhijiandao.cn

[U31] Py：单测
来源：http://qfj.gogol.net.cn

python -m pytest -q
来源：http://zos.xylfe.cn

[U32] Py：代码格式化
来源：http://wwl.xinyue.icu

ruff format . && ruff check --fix .
来源：http://xly.hnxiangtu.top

[U33] Py：打包发布
来源：http://qpy.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://hcg.guannengcc.top

[U34] Py：判断编码
来源：http://vmb.gogol.net.cn

chardet.detect(raw)
来源：http://bqf.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://zgj.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://joq.hywenlv.cn

[U36] Py：定时任务
来源：http://xub.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://wok.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://yuo.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://ayh.fzhhl.top

[U38] Py：获取脚本所在目录
来源：http://pyg.andypj.xyz

Path(__file__).resolve().parent
来源：http://gwq.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://zrh.xylfe.cn

sys.stdout.isatty()
来源：http://fom.wangdashe.top

[U40] Py：打印到标准错误
来源：http://tnd.epnwcf.com

print("err", file=sys.stderr)
来源：http://vdp.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://qdz.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qgq.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://ezf.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qtq.yueranfly.top

[U43] PHP：声明命名空间
来源：http://uzp.yj20258888.top

namespace App\Http;
来源：http://ihq.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://oln.cucudq.cn

declare(strict_types=1);
来源：http://vmv.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://evr.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yik.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://srf.yfazqb.com

?string $name = null
来源：http://gmx.jianghu66.top

[U47] PHP：联合类型
来源：http://emd.9152youxi.cn

int|string $id
来源：http://sjx.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://yon.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yqk.hywenlv.cn

[U49] PHP：只读属性
来源：http://moq.quarkkingdee.top

public readonly string $name
来源：http://azz.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://skr.aizwys.cn

public function __construct(private int $id) {}
来源：http://sbl.fzhhl.top

[U51] PHP：数组解构
来源：http://kqv.chenlongwang.top

[$a, $b] = $arr;
来源：http://lbo.shzxlz.cn

[U52] PHP：箭头函数
来源：http://hxa.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://zjv.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://ubn.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://aco.yuanzhike.top

[U54] PHP：空安全调用
来源：http://esf.jinyuanbaomall.cn

$obj?->method()
来源：http://lqk.ivvv.top

[U55] PHP：match 表达式
来源：http://iir.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ubj.gogol.net.cn

[U56] PHP：命名参数
来源：http://exh.fehbvm.com

f(a: 1, b: 2)
来源：http://tie.gogol.net.cn

[U57] PHP：字符串插值
来源：http://fau.zhixingplan.top

"值: {$a}"
来源：http://fdy.hnqzz.top

[U58] PHP：数组三件套
来源：http://uxf.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tln.fanxiaobao.xyz

[U59] PHP：自定义排序
来源：http://zyx.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jxy.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://dhb.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dun.hnqzz.top

[U61] PHP：正则
来源：http://htt.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qyc.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://xvg.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tyi.yongpay.top


<!-- 参考信息 -->