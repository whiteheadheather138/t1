代发 wailian999

[S35] C++：map
来源：http://syw.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rob.chenlongwang.top

[S36] C++：unordered_map
来源：http://bgd.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pie.iojbl.cn

[S37] C++：set
来源：http://tzm.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ehl.shanyushiyangtech.top

[S38] C++：排序
来源：http://ovv.fanxiaobao.xyz

std::sort(v.begin(), v.end());
来源：http://ihi.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://cqa.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qnp.fehbvm.com

[S40] C++：查找元素
来源：http://ngm.hfpthk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rtl.sufxvd.cn

[S41] C++：类与构造函数
来源：http://rdm.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lxk.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://whb.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://qhg.chenzaomai.com

[S43] C++：智能指针
来源：http://rqw.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://kqk.tian-w.cn

[S44] C++：引用传参
来源：http://iur.uphjek.com

void inc(int &x) { ++x; }
来源：http://edr.svipenyu.cn

[S45] C++：lambda
来源：http://dva.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dpg.guannengcc.top

[S46] C++：函数模板
来源：http://udc.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jzx.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://hvd.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blb.jyoumei.cn

[S48] C++：逐行读文件
来源：http://lfx.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nyu.zycfv.cn

while (std::getline(in, line)) { }
来源：http://lea.yfazqb.com

[S49] C++：写文件
来源：http://snc.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://idm.ydjk.org.cn

[S50] C++：格式化数字
来源：http://jmv.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hpt.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://nak.yj20258888.top

static_cast<double>(a) / b
来源：http://paz.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://jvn.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://hvp.yj20258.top

[S53] C++：移动语义
来源：http://str.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://txj.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://opu.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gyl.epnwcf.com

[S55] C++：结构化绑定
来源：http://pkl.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vci.tanke756.top

[S56] C++：optional
来源：http://cyn.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qrr.hnxiangtu.top

[S57] C++：编译期常量
来源：http://sqc.chenlongwang.top

constexpr int N = 10;
来源：http://vql.fehbvm.com

[S58] C++：命名空间
来源：http://dcz.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://fit.dashuyun.cn

[S59] C++：静态断言
来源：http://quy.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dtn.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://hfm.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://krz.xingfuxueyuan.xyz

================================================================================
来源：http://smz.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cqf.zycfv.cn

================================================================================
来源：http://elw.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://vtx.cdnleiting.top

println("Hello")
来源：http://qat.yanxiufei.cn

[T02] Kotlin：变量
来源：http://duh.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uky.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://hvl.jinqigufen.top

"值: $b"
来源：http://khl.gogol.net.cn

[T04] Kotlin：空安全
来源：http://tid.cucudq.cn

val n: String? = null;  n?.length
来源：http://hgn.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://nex.sufxvd.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ceo.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://dpk.zycfv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://toy.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://hap.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lnf.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://xbr.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://fgi.cashguo.top

[T09] Kotlin：扩展函数
来源：http://vyz.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://jsp.gaohongyu789.top

[T10] Kotlin：默认参数
来源：http://dfe.nanxuanxn.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ujm.gogol.net.cn

[T11] Kotlin：协程
来源：http://rkz.tarul.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jhh.tian-w.cn

[T12] Kotlin：解构声明
来源：http://ttj.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://jiq.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://dei.gzhubu.top

val m = mapOf("a" to 1)
来源：http://zex.quarkkingdee.top

[T14] Kotlin：循环
来源：http://oqk.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://gcs.sjlbkw.cn

[T15] Kotlin：接口
来源：http://xpa.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://lmz.guannengcc.top

[T16] Swift：Hello World
来源：http://rgf.gzhubu.top

print("Hello")
来源：http://tuy.9152youxi.cn

[T17] Swift：变量与常量
来源：http://hll.svipenyu.cn

var a = 1;  let b = 2
来源：http://ggu.yj20258888.top

[T18] Swift：字符串插值
来源：http://ktd.hcnkem.com

"值: \(b)"
来源：http://ngg.ivvv.top

[T19] Swift：可选绑定
来源：http://xoy.aibaodan.cn

if let n = opt { print(n) }
来源：http://tps.52xcode.cn

[T20] Swift：数组操作
来源：http://aqs.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://wbr.bjfxy.top

[T21] Swift：遍历
来源：http://zul.sufxvd.cn

for x in a { print(x) }
来源：http://nve.fzhhl.top

[T22] Swift：字典
来源：http://jjt.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://twb.hcnkem.com

[T23] Swift：函数
来源：http://vga.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kgi.svipenyu.cn

[T24] Swift：闭包
来源：http://rsy.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://obc.uphjek.com

[T25] Swift：结构体
来源：http://ebi.zdbjq.cn

struct P { var x: Int }
来源：http://wny.shuidangran.top

[T26] Swift：类与重写
来源：http://vjd.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://fvl.shzxlz.cn

[T27] Swift：错误处理
来源：http://hgl.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://zjt.c1oappe.top

[T28] Swift：枚举
来源：http://img.ydzc1.top

enum Color { case red, green }
来源：http://rew.tanke756.top

[T29] Swift：guard 提前返回
来源：http://oju.fehbvm.com

guard let x = opt else { return }
来源：http://agx.pycfn.com

[T30] Swift：协议
来源：http://azf.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://rxi.zhoulong.xyz

[T31] Lua：Hello World
来源：http://rja.xylfe.cn

print("Hello")
来源：http://vij.vqdsnc.cn

[T32] Lua：局部变量
来源：http://dto.52xcode.cn

local a = 1
来源：http://vjv.yfazqb.com

[T33] Lua：表（数组）
来源：http://hdm.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tyx.yj20258.top

[T34] Lua：遍历表
来源：http://ray.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zdu.tarul.cn

[T35] Lua：字典表
来源：http://qzf.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://xyu.xuetiantiany.cn

[T36] Lua：函数
来源：http://kcz.sweek.top

function add(a, b) return a + b end
来源：http://eag.sysykeji.top

[T37] Lua：字符串拼接
来源：http://ogf.zhongyouzk.top

"a" .. "b"
来源：http://cgf.jqgufenzy.top

[T38] Lua：条件
来源：http://gux.cdnleiting.top

if x > 0 then print("正") end
来源：http://smt.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://xrg.pengpengdd.cyou

string.find(s, "%d+")
来源：http://uau.tianlin.xyz

[T40] Lua：元表
来源：http://fnz.zhongyouzk.top

setmetatable({}, { __index = base })
来源：http://ecb.aizwys.cn

[T41] Perl：Hello World
来源：http://epm.redwolf501.top

print "Hello\n";
来源：http://tqd.cucudq.cn

[T42] Perl：变量类型
来源：http://fgq.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yvs.yongpay.top

[T43] Perl：字符串插值
来源：http://gxq.9152youxi.cn

"值: $a"
来源：http://cbn.pycfn.com

[T44] Perl：条件
来源：http://twe.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://skl.ehwqpu.com

[T45] Perl：数组遍历
来源：http://ypb.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://rrm.pycfn.com

[T46] Perl：哈希操作
来源：http://pqp.meibo888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tdt.haohaochexian.top

[T47] Perl：正则捕获
来源：http://wwn.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yac.sjlbkw.cn

[T48] Perl：正则替换
来源：http://ztq.yvedp.cn

$s =~ s/old/new/g;
来源：http://kkp.wangshuangyany.cn

[T49] Perl：函数
来源：http://ghb.yonumen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iar.hnqzz.top

[T50] Perl：逐行读文件
来源：http://fpe.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://udr.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://oft.daria6918.cn

[T51] Scala：Hello World
来源：http://phv.meibo888.top

println("Hello")
来源：http://yid.zhoulong.xyz

[T52] Scala：变量
来源：http://pbo.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://wgl.meibo888.top

[T53] Scala：字符串插值
来源：http://qyl.yj20258.top

s"值: $b"
来源：http://fcj.nanxinkj.top

[T54] Scala：集合映射
来源：http://rme.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://hqm.hywenlv.cn

[T55] Scala：集合过滤
来源：http://rch.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://gne.nwbrower.top

[T56] Scala：样例类
来源：http://wlp.jqgfzy.top

case class User(name: String, age: Int)
来源：http://czg.shzxlz.cn

[T57] Scala：模式匹配
来源：http://wxg.nanxuanxn.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lwj.yvedp.cn

[T58] Scala：函数定义
来源：http://fuk.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://xke.zhijiandao.cn

[T59] Scala：循环
来源：http://rwo.haohaochexian.top

for (i <- 1 to 10) println(i)
来源：http://cpb.ehwqpu.com

[T60] Scala：折叠
来源：http://lqk.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hht.cdnleiting.top

================================================================================
来源：http://uft.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xbz.ydjk.org.cn

================================================================================
来源：http://czp.uphjek.com

[U01] Py：创建虚拟环境
来源：http://vei.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rto.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://rqz.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://thi.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://kku.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xzr.cqqwz.cn

[U04] Py：变量调试打印
来源：http://xfw.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xgx.xinyue.icu

[U05] Py：列表去重且保序
来源：http://jva.wangshuangyany.cn

list(dict.fromkeys(arr))
来源：http://foj.yongpay.top

[U06] Py：合并两个字典
来源：http://ido.wangshuangyany.cn

{**a, **b}
来源：http://jap.sweek.top

[U07] Py：反转字典键值
来源：http://fjl.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://oux.yvedp.cn

[U08] Py：展平二维列表
来源：http://uye.zhixingplan.top

[y for x in nested for y in x]
来源：http://oua.uphjek.com

[U09] Py：字典取最大值的键
来源：http://waj.gzhubu.top

max(d, key=d.get)
来源：http://exm.tian-w.cn

[U10] Py：按值排序字典
来源：http://fhh.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ams.tian-w.cn

[U11] Py：生成器表达式
来源：http://mrq.aibaodan.cn

(x * 2 for x in arr)
来源：http://jsq.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://osb.chenzaomai.com

Counter(arr).most_common(3)
来源：http://isq.dashuyun.cn

[U13] Py：固定长度队列
来源：http://qeu.shuidangran.top

deque(maxlen=10)
来源：http://cuv.fengsongda.top

[U14] Py：分组收集到列表
来源：http://jet.gaohongyu789.top

defaultdict(list)
来源：http://orl.chenjidiqi.icu

[U15] Py：高精度计时
来源：http://xrj.smart0.xyz

t = time.perf_counter()
来源：http://rly.bjfxy.top

[U16] Py：命令行参数解析
来源：http://zoh.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yvs.yongpay.top

[U17] Py：初始化日志
来源：http://adq.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://lsd.jlsjyb.cn

[U18] Py：预编译正则
来源：http://lya.yongpay.top

pat = re.compile(r"\d+")
来源：http://dmg.ydzc1.top

[U19] Py：正则替换带回调
来源：http://dsw.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kun.sysykeji.top

[U20] Py：缓存函数结果
来源：http://ejx.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://rut.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://xzb.316326.xyz

@contextlib.contextmanager
来源：http://ljd.fktsv.cn

[U22] Py：矩阵转置
来源：http://jpg.vqdsnc.cn

list(zip(*m))
来源：http://yfu.hammf.cn

[U23] Py：分块读取大文件
来源：http://ata.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://htf.cashguo.top

[U24] Py：路径操作
来源：http://oaa.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vtf.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://vwm.hnqzz.top

csv.DictReader(f)
来源：http://exo.zdqjudy.top

[U26] Py：并发下载
来源：http://xxw.xziqi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dye.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://xqb.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://lur.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://xoe.hywenlv.cn

UserId = int
来源：http://mks.daria6918.cn

[U29] Py：属性校验
来源：http://zzw.nanxinkj.top

@property 与 @x.setter 配合
来源：http://onk.jyoumei.cn

[U30] Py：数据类
来源：http://lmm.nanxuanxn.top

@dataclass(slots=True)
来源：http://amw.jinqigfzy.top

[U31] Py：单测
来源：http://wzo.daxiang520.top

python -m pytest -q
来源：http://gmm.daria6918.cn

[U32] Py：代码格式化
来源：http://jbr.ivvv.top

ruff format . && ruff check --fix .
来源：http://ppz.cashguo.top

[U33] Py：打包发布
来源：http://zei.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://jgr.ctjpmb.com

[U34] Py：判断编码
来源：http://odx.jinqigfzy.top

chardet.detect(raw)
来源：http://esi.haohaochexian.top

[U35] Py：发送邮件
来源：http://ugr.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qpy.hfpthk.cn

[U36] Py：定时任务
来源：http://ysu.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://uvp.yuanzhike.top

[U37] Py：读写 Excel
来源：http://jqf.nwbrower.top

pandas.read_excel / DataFrame.to_excel
来源：http://ebg.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://xjh.ehwqpu.com

Path(__file__).resolve().parent
来源：http://irs.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://nvl.haohaochexian.top

sys.stdout.isatty()
来源：http://xgo.tanke756.top

[U40] Py：打印到标准错误
来源：http://azs.zhengqikj.top

print("err", file=sys.stderr)
来源：http://yth.hesvh.cn

[U41] PHP：初始化 Composer 项目
来源：http://kfk.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pmf.pycfn.com

[U42] PHP：PSR-4 自动加载
来源：http://wkm.gzhubu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ymq.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://xsv.aibaodan.cn

namespace App\Http;
来源：http://hwh.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://xbj.chenjidiqi.icu

declare(strict_types=1);
来源：http://qla.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://xwr.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rbe.tianlin.xyz

[U46] PHP：可空类型
来源：http://vfj.zhaomingkeji.xyz

?string $name = null
来源：http://xia.c1oappe.top

[U47] PHP：联合类型
来源：http://ovm.yanxiufei.cn

int|string $id
来源：http://rsp.316326.xyz

[U48] PHP：纯枚举
来源：http://cft.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://svj.ctjpmb.com

[U49] PHP：只读属性
来源：http://zrc.hammf.cn

public readonly string $name
来源：http://pdw.aibaodan.cn

[U50] PHP：构造器属性提升
来源：http://mad.fzhhl.top

public function __construct(private int $id) {}
来源：http://bbg.epnwcf.com

[U51] PHP：数组解构
来源：http://tsm.hnxiangtu.top

[$a, $b] = $arr;
来源：http://mjz.ctjpmb.com

[U52] PHP：箭头函数
来源：http://ujo.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://msz.yongpay.top

[U53] PHP：空合并运算符
来源：http://qej.xuetiantiany.cn

$v = $a ?? $b ?? "default";
来源：http://ynu.tian-w.cn

[U54] PHP：空安全调用
来源：http://bzh.xziqi.cn

$obj?->method()
来源：http://onp.jiagoushi.top

[U55] PHP：match 表达式
来源：http://gwt.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jck.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://brx.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://ivk.yj20258.top

[U57] PHP：字符串插值
来源：http://tyf.daria6918.cn

"值: {$a}"
来源：http://lxh.dashuyun.cn

[U58] PHP：数组三件套
来源：http://rgi.jqgfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vaf.yfazqb.com

[U59] PHP：自定义排序
来源：http://iyk.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qno.sweek.top

[U60] PHP：JSON 编解码
来源：http://dex.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iyi.xinyue.icu


<!-- 参考信息 -->