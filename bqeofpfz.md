代发 wailian999

[S35] C++：map
来源：http://sjj.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ouw.haohaochexian.top

[S36] C++：unordered_map
来源：http://xrf.daxiang520.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mxu.jqgfzy.top

[S37] C++：set
来源：http://wru.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fzq.shuidangran.top

[S38] C++：排序
来源：http://enw.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://brd.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://ntj.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bzg.zhengqikj.top

[S40] C++：查找元素
来源：http://skl.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ssc.yj20258.top

[S41] C++：类与构造函数
来源：http://umm.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lpw.fktsv.cn

[S42] C++：继承与虚函数
来源：http://bup.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://cns.jianghu66.top

[S43] C++：智能指针
来源：http://zxi.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://vqr.yuxming.cn

[S44] C++：引用传参
来源：http://xue.iojbl.cn

void inc(int &x) { ++x; }
来源：http://bun.yanxiufei.cn

[S45] C++：lambda
来源：http://kom.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://wfn.jlsjyb.cn

[S46] C++：函数模板
来源：http://zsw.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ksh.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://bgm.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ldf.hcnkem.com

[S48] C++：逐行读文件
来源：http://bfn.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://acn.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://awf.dianchejie.cn

[S49] C++：写文件
来源：http://brl.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sxz.jiagoushi.top

[S50] C++：格式化数字
来源：http://vjo.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uzb.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://osm.316326.xyz

static_cast<double>(a) / b
来源：http://wzt.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://kff.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://dfu.yj20258888.top

[S53] C++：移动语义
来源：http://xne.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://ygo.ydjk.org.cn

[S54] C++：异常处理
来源：http://unt.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jon.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://ozh.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cpc.nwbrower.top

[S56] C++：optional
来源：http://vwn.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yap.fengsongda.top

[S57] C++：编译期常量
来源：http://ezd.yfazqb.com

constexpr int N = 10;
来源：http://lsp.gogol.net.cn

[S58] C++：命名空间
来源：http://edp.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://iva.feifeiyinyue.top

[S59] C++：静态断言
来源：http://cux.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wei.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://loa.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://unr.sxryk.cn

================================================================================
来源：http://wtw.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dvs.0kj1m.cn

================================================================================
来源：http://pic.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://wtc.zhixingplan.top

println("Hello")
来源：http://nux.nanxuanxn.top

[T02] Kotlin：变量
来源：http://hfh.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zrc.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://ynp.xuetiantiany.cn

"值: $b"
来源：http://bbw.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://xsb.snrcjt.cn

val n: String? = null;  n?.length
来源：http://auf.gaohongyu789.top

[T05] Kotlin：when 表达式
来源：http://mvb.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jsz.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://hue.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://eoi.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://gsn.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iuv.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://rxg.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://zww.yj202588.top

[T09] Kotlin：扩展函数
来源：http://ltn.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://zyv.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://rnt.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vpa.andypj.xyz

[T11] Kotlin：协程
来源：http://see.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jty.bjfxy.top

[T12] Kotlin：解构声明
来源：http://qrs.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://sgg.pycfn.com

[T13] Kotlin：只读 Map
来源：http://rin.hnqzz.top

val m = mapOf("a" to 1)
来源：http://ahg.sjlbkw.cn

[T14] Kotlin：循环
来源：http://ejx.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://rgy.ivvv.top

[T15] Kotlin：接口
来源：http://pjk.redwolf501.top

interface Shape { fun area(): Double }
来源：http://dgv.smart0.xyz

[T16] Swift：Hello World
来源：http://rop.hysaishi.cn

print("Hello")
来源：http://kre.zdbjq.cn

[T17] Swift：变量与常量
来源：http://dhc.shuidangran.top

var a = 1;  let b = 2
来源：http://psm.hnqzz.top

[T18] Swift：字符串插值
来源：http://jqi.xylfe.cn

"值: \(b)"
来源：http://kng.yuxming.cn

[T19] Swift：可选绑定
来源：http://oqc.ybcxt.top

if let n = opt { print(n) }
来源：http://skx.yuanzhike.top

[T20] Swift：数组操作
来源：http://hkl.0kj1m.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oos.cucudq.cn

[T21] Swift：遍历
来源：http://tdv.fehbvm.com

for x in a { print(x) }
来源：http://oul.zhoulong.xyz

[T22] Swift：字典
来源：http://qoh.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://yao.cucudq.cn

[T23] Swift：函数
来源：http://tcp.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ocw.aibaodan.cn

[T24] Swift：闭包
来源：http://fkd.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zlc.hongshengwenyu.top

[T25] Swift：结构体
来源：http://lxq.pengpengdd.cyou

struct P { var x: Int }
来源：http://jof.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://lfl.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://uej.aibaodan.cn

[T27] Swift：错误处理
来源：http://dzz.ydzc1.top

do { try f() } catch { print(error) }
来源：http://dox.fzhhl.top

[T28] Swift：枚举
来源：http://usc.aibaodan.cn

enum Color { case red, green }
来源：http://tsx.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://fnw.hnqzz.top

guard let x = opt else { return }
来源：http://gou.haohaochexian.top

[T30] Swift：协议
来源：http://gpk.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://llv.cheryme.top

[T31] Lua：Hello World
来源：http://jgk.redwolf501.top

print("Hello")
来源：http://eau.pycfn.com

[T32] Lua：局部变量
来源：http://pop.cashguo.top

local a = 1
来源：http://bop.yj202588.top

[T33] Lua：表（数组）
来源：http://gaa.chenzaomai.com

local t = {1, 2, 3};  t[4] = 4
来源：http://hmu.cucudq.cn

[T34] Lua：遍历表
来源：http://fpq.snrcjt.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qbm.cucudq.cn

[T35] Lua：字典表
来源：http://vkz.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://nhj.smart0.xyz

[T36] Lua：函数
来源：http://lnz.nanxuanxn.top

function add(a, b) return a + b end
来源：http://mqb.yongpay.top

[T37] Lua：字符串拼接
来源：http://zfh.redwolf501.top

"a" .. "b"
来源：http://kqo.haohaochexian.top

[T38] Lua：条件
来源：http://njk.tanke756.top

if x > 0 then print("正") end
来源：http://vmw.yvedp.cn

[T39] Lua：模式匹配
来源：http://krw.zhiwuduotai.top

string.find(s, "%d+")
来源：http://pwj.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://xvw.vehdjk.com

setmetatable({}, { __index = base })
来源：http://dtj.yonumen.top

[T41] Perl：Hello World
来源：http://zww.andypj.xyz

print "Hello\n";
来源：http://qwq.yvedp.cn

[T42] Perl：变量类型
来源：http://rsw.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vpv.aizwys.cn

[T43] Perl：字符串插值
来源：http://zcd.yj20258888.top

"值: $a"
来源：http://reo.snrcjt.cn

[T44] Perl：条件
来源：http://mfz.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://yoi.fehbvm.com

[T45] Perl：数组遍历
来源：http://zdd.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://rmg.jinghuilouyu.cn

[T46] Perl：哈希操作
来源：http://mez.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zbr.yj202588.top

[T47] Perl：正则捕获
来源：http://hcy.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pgo.gotoacloud.top

[T48] Perl：正则替换
来源：http://cwm.bbcook.cn

$s =~ s/old/new/g;
来源：http://bkk.jianghu66.top

[T49] Perl：函数
来源：http://ryg.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xna.sxryk.cn

[T50] Perl：逐行读文件
来源：http://qcd.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jux.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://dkv.wangdashe.top

[T51] Scala：Hello World
来源：http://pkw.yj20258.top

println("Hello")
来源：http://aen.chenlongwang.top

[T52] Scala：变量
来源：http://csj.gaohongyu789.top

val a = 1;  var b = 2
来源：http://rzw.zhixingplan.top

[T53] Scala：字符串插值
来源：http://erv.shzxlz.cn

s"值: $b"
来源：http://fsn.jinqigufen.top

[T54] Scala：集合映射
来源：http://lwx.jinyuanbaomall.cn

List(1, 2, 3).map(_ * 2)
来源：http://awf.hnqzz.top

[T55] Scala：集合过滤
来源：http://tps.fehbvm.com

List(1, 2, 3).filter(_ > 1)
来源：http://nge.zycfv.cn

[T56] Scala：样例类
来源：http://gcj.hongshengwenyu.top

case class User(name: String, age: Int)
来源：http://wve.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://suq.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://scj.gogol.net.cn

[T58] Scala：函数定义
来源：http://bmx.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hhk.bjfxy.top

[T59] Scala：循环
来源：http://cnv.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://rev.xylfe.cn

[T60] Scala：折叠
来源：http://ayv.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://twy.tanke756.top

================================================================================
来源：http://mib.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dkw.aibaodan.cn

================================================================================
来源：http://nst.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://vye.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://dsp.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://geh.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gzc.yj20258.top

[U03] Py：加载 .env 配置
来源：http://qff.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hdn.gzhubu.top

[U04] Py：变量调试打印
来源：http://tbs.zhixingplan.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gub.xingfuxueyuan.xyz

[U05] Py：列表去重且保序
来源：http://hao.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://vwn.hnqzz.top

[U06] Py：合并两个字典
来源：http://gcx.hywenlv.cn

{**a, **b}
来源：http://zml.gotoacloud.top

[U07] Py：反转字典键值
来源：http://kdw.daria6918.cn

{v: k for k, v in d.items()}
来源：http://xxg.havefunace.top

[U08] Py：展平二维列表
来源：http://evu.ydzc1.top

[y for x in nested for y in x]
来源：http://dhu.ivvv.top

[U09] Py：字典取最大值的键
来源：http://ixl.yuanzhike.top

max(d, key=d.get)
来源：http://djv.xylfe.cn

[U10] Py：按值排序字典
来源：http://byi.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zqr.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://hkq.jqgufenzy.top

(x * 2 for x in arr)
来源：http://ixj.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wzh.xziqi.cn

Counter(arr).most_common(3)
来源：http://cwb.havefunace.top

[U13] Py：固定长度队列
来源：http://psp.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://wgb.hnqzz.top

[U14] Py：分组收集到列表
来源：http://crf.ppjwa.cn

defaultdict(list)
来源：http://oox.nanxinkj.top

[U15] Py：高精度计时
来源：http://kwh.hnqzz.top

t = time.perf_counter()
来源：http://aec.pycfn.com

[U16] Py：命令行参数解析
来源：http://rha.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nqy.xuanzx.com

[U17] Py：初始化日志
来源：http://xlp.xuetiantiany.cn

logging.basicConfig(level=logging.INFO)
来源：http://caf.bjfxy.top

[U18] Py：预编译正则
来源：http://bxj.yanxiufei.cn

pat = re.compile(r"\d+")
来源：http://bkp.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://rks.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oar.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://buq.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://chq.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://iki.daria6918.cn

@contextlib.contextmanager
来源：http://jbv.yueranfly.top

[U22] Py：矩阵转置
来源：http://yme.aibaodan.cn

list(zip(*m))
来源：http://hxn.aizwys.cn

[U23] Py：分块读取大文件
来源：http://zgh.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://loe.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://xlb.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xyr.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://yhg.fktsv.cn

csv.DictReader(f)
来源：http://tli.sysykeji.top

[U26] Py：并发下载
来源：http://vkw.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jek.epnwcf.com

[U27] Py：异步 HTTP
来源：http://utg.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://pxp.hnxiangtu.top

[U28] Py：类型别名
来源：http://uhu.yanxiufei.cn

UserId = int
来源：http://nbu.fanxiaobao.xyz

[U29] Py：属性校验
来源：http://tkq.jqgfzy.top

@property 与 @x.setter 配合
来源：http://yzo.zhixingplan.top

[U30] Py：数据类
来源：http://die.gotoacloud.top

@dataclass(slots=True)
来源：http://jfc.tarul.cn

[U31] Py：单测
来源：http://ekl.hnqzz.top

python -m pytest -q
来源：http://rhn.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://dyn.mhx1999.top

ruff format . && ruff check --fix .
来源：http://pzc.hammf.cn

[U33] Py：打包发布
来源：http://mdo.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://dyo.fktsv.cn

[U34] Py：判断编码
来源：http://qco.daxiang520.top

chardet.detect(raw)
来源：http://oyj.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://uuv.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://adt.yongpay.top

[U36] Py：定时任务
来源：http://yty.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://qlt.pycfn.com

[U37] Py：读写 Excel
来源：http://byk.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wen.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://nie.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://ltd.gzhubu.top

[U39] Py：判断是否在交互环境
来源：http://uzf.yj20258888.top

sys.stdout.isatty()
来源：http://umr.sweek.top

[U40] Py：打印到标准错误
来源：http://wqr.ehwqpu.com

print("err", file=sys.stderr)
来源：http://mew.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://foj.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://plc.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://uro.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uvg.aizwys.cn

[U43] PHP：声明命名空间
来源：http://xed.hesvh.cn

namespace App\Http;
来源：http://eba.daxiang520.top

[U44] PHP：开启严格类型
来源：http://vhu.zhengqikj.top

declare(strict_types=1);
来源：http://kie.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://uiq.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ens.havefunace.top

[U46] PHP：可空类型
来源：http://peg.52xcode.cn

?string $name = null
来源：http://sni.cheryme.top

[U47] PHP：联合类型
来源：http://qcs.tarul.cn

int|string $id
来源：http://mla.uphjek.com

[U48] PHP：纯枚举
来源：http://jtd.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mgv.c1oappe.top

[U49] PHP：只读属性
来源：http://usm.xuetiantiany.cn

public readonly string $name
来源：http://hpp.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://joo.zdqjudy.top

public function __construct(private int $id) {}
来源：http://wlv.ywan-chungtsiang.top

[U51] PHP：数组解构
来源：http://tcg.vehdjk.com

[$a, $b] = $arr;
来源：http://wdq.xinyue.icu

[U52] PHP：箭头函数
来源：http://oxh.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://odv.tarul.cn

[U53] PHP：空合并运算符
来源：http://ara.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://fnq.aizwys.cn

[U54] PHP：空安全调用
来源：http://xgf.pycfn.com

$obj?->method()
来源：http://kln.cqqwz.cn

[U55] PHP：match 表达式
来源：http://xsa.mhx1999.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fsg.ydzc1.top

[U56] PHP：命名参数
来源：http://qrm.xziqi.cn

f(a: 1, b: 2)
来源：http://zdi.tanke756.top

[U57] PHP：字符串插值
来源：http://oyk.bjfxy.top

"值: {$a}"
来源：http://gaw.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://flf.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zsu.0kj1m.cn

[U59] PHP：自定义排序
来源：http://bfk.birdmap.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ivk.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://mea.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ibb.redwolf501.top


<!-- 参考信息 -->