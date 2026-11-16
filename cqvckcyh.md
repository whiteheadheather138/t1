代发 wailian999

[S35] C++：map
来源：http://oyw.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hji.meibo888.top

[S36] C++：unordered_map
来源：http://dbb.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zoi.xziqi.cn

[S37] C++：set
来源：http://icw.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xmm.xuetiantiany.cn

[S38] C++：排序
来源：http://uuc.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://hfi.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://nge.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wta.chenjidiqi.icu

[S40] C++：查找元素
来源：http://kvi.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ccg.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://zct.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qoo.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://ymi.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://vmx.zdqjudy.top

[S43] C++：智能指针
来源：http://kqe.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://aut.dashuyun.cn

[S44] C++：引用传参
来源：http://zae.sweek.top

void inc(int &x) { ++x; }
来源：http://wwm.316326.xyz

[S45] C++：lambda
来源：http://tcm.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://shp.chenlongwang.top

[S46] C++：函数模板
来源：http://yrb.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yma.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://wsp.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fqg.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://nuc.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ska.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://qzf.jiagoushi.top

[S49] C++：写文件
来源：http://yfy.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://umn.haohaochexian.top

[S50] C++：格式化数字
来源：http://zua.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dni.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://xwa.svipenyu.cn

static_cast<double>(a) / b
来源：http://wfo.hammf.cn

[S52] C++：const 与 noexcept
来源：http://omq.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://mzv.daria6918.cn

[S53] C++：移动语义
来源：http://qny.cashguo.top

std::vector<int> w = std::move(v);
来源：http://jri.redwolf501.top

[S54] C++：异常处理
来源：http://kqh.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://egy.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://fsc.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://egs.sjlbkw.cn

[S56] C++：optional
来源：http://nfp.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pep.sufxvd.cn

[S57] C++：编译期常量
来源：http://bhl.iojbl.cn

constexpr int N = 10;
来源：http://tit.jqgfzy.top

[S58] C++：命名空间
来源：http://tca.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://tzg.cqqwz.cn

[S59] C++：静态断言
来源：http://xlw.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kye.zhixingplan.top

[S60] C++：遍历并删除元素
来源：http://kjl.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://psb.cheryme.top

================================================================================
来源：http://hnu.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fwh.bbcook.cn

================================================================================
来源：http://wzx.guannengcc.top

[T01] Kotlin：Hello World
来源：http://xte.316326.xyz

println("Hello")
来源：http://vlg.hesvh.cn

[T02] Kotlin：变量
来源：http://zmn.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mti.yj20258888.top

[T03] Kotlin：字符串模板
来源：http://wzk.tianlin.xyz

"值: $b"
来源：http://wky.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://mbn.zdbjq.cn

val n: String? = null;  n?.length
来源：http://tkf.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://bzu.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fwx.cucudq.cn

[T06] Kotlin：集合映射
来源：http://zwq.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ubz.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://muo.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://npv.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://jam.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://bvw.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://aqe.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://fys.hnqzz.top

[T10] Kotlin：默认参数
来源：http://qvd.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jnd.jiagoushi.top

[T11] Kotlin：协程
来源：http://yhw.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mwi.hesvh.cn

[T12] Kotlin：解构声明
来源：http://zqj.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://gte.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://wdn.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://lkn.ybcxt.top

[T14] Kotlin：循环
来源：http://fxp.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://sqy.zdbjq.cn

[T15] Kotlin：接口
来源：http://ibf.zycfv.cn

interface Shape { fun area(): Double }
来源：http://cdv.52xcode.cn

[T16] Swift：Hello World
来源：http://ase.yueranfly.top

print("Hello")
来源：http://eib.hcnkem.com

[T17] Swift：变量与常量
来源：http://eai.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://woz.birdmap.top

[T18] Swift：字符串插值
来源：http://xvp.sjlbkw.cn

"值: \(b)"
来源：http://nms.0kj1m.cn

[T19] Swift：可选绑定
来源：http://nix.ehwqpu.com

if let n = opt { print(n) }
来源：http://ona.52xcode.cn

[T20] Swift：数组操作
来源：http://zze.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ato.jyoumei.cn

[T21] Swift：遍历
来源：http://lry.hysaishi.cn

for x in a { print(x) }
来源：http://mza.nanxuanxn.top

[T22] Swift：字典
来源：http://zgq.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://alk.hnxiangtu.top

[T23] Swift：函数
来源：http://vyu.zhaomingkeji.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rtk.yfazqb.com

[T24] Swift：闭包
来源：http://fdg.52xcode.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hpq.zhijiandao.cn

[T25] Swift：结构体
来源：http://scu.hfpthk.cn

struct P { var x: Int }
来源：http://fuu.fzhhl.top

[T26] Swift：类与重写
来源：http://okn.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://oug.jlsjyb.cn

[T27] Swift：错误处理
来源：http://ykt.ybcxt.top

do { try f() } catch { print(error) }
来源：http://aag.chenjidiqi.icu

[T28] Swift：枚举
来源：http://dra.sysykeji.top

enum Color { case red, green }
来源：http://gnu.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://iww.52xcode.cn

guard let x = opt else { return }
来源：http://edw.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://iwz.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://mza.sxryk.cn

[T31] Lua：Hello World
来源：http://jjv.iojbl.cn

print("Hello")
来源：http://wgh.cucudq.cn

[T32] Lua：局部变量
来源：http://vca.yj20258888.top

local a = 1
来源：http://ejv.daxiang520.top

[T33] Lua：表（数组）
来源：http://lir.xuanzx.com

local t = {1, 2, 3};  t[4] = 4
来源：http://wgb.smart0.xyz

[T34] Lua：遍历表
来源：http://vga.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mbc.zhoulong.xyz

[T35] Lua：字典表
来源：http://wsb.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://cvp.yonumen.top

[T36] Lua：函数
来源：http://fyx.hysaishi.cn

function add(a, b) return a + b end
来源：http://gdl.fengsongda.top

[T37] Lua：字符串拼接
来源：http://iwo.mhx1999.top

"a" .. "b"
来源：http://cwi.cdnleiting.top

[T38] Lua：条件
来源：http://twb.sysykeji.top

if x > 0 then print("正") end
来源：http://raz.uphjek.com

[T39] Lua：模式匹配
来源：http://vom.ydzc1.top

string.find(s, "%d+")
来源：http://lls.zhijiandao.cn

[T40] Lua：元表
来源：http://ghf.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://bpc.tanke756.top

[T41] Perl：Hello World
来源：http://pwt.yj20258888.top

print "Hello\n";
来源：http://brl.chenjidiqi.icu

[T42] Perl：变量类型
来源：http://lax.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qug.feifeiyinyue.top

[T43] Perl：字符串插值
来源：http://ptk.hongshengwenyu.top

"值: $a"
来源：http://wtc.haohaochexian.top

[T44] Perl：条件
来源：http://atm.hesvh.cn

if ($a > 0) { print "正"; }
来源：http://qit.yonumen.top

[T45] Perl：数组遍历
来源：http://kcn.dashuyun.cn

for my $x (@arr) { print $x; }
来源：http://aim.sxryk.cn

[T46] Perl：哈希操作
来源：http://djt.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uzs.wangdashe.top

[T47] Perl：正则捕获
来源：http://eos.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://wke.daria6918.cn

[T48] Perl：正则替换
来源：http://wzt.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://qvt.fengsongda.top

[T49] Perl：函数
来源：http://hmm.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gsw.yueranfly.top

[T50] Perl：逐行读文件
来源：http://cxk.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://llx.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://qpc.uphjek.com

[T51] Scala：Hello World
来源：http://xln.aibaodan.cn

println("Hello")
来源：http://pzl.jlsjyb.cn

[T52] Scala：变量
来源：http://kua.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://vpy.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://ziw.ehwqpu.com

s"值: $b"
来源：http://ecf.cashguo.top

[T54] Scala：集合映射
来源：http://vpm.cashguo.top

List(1, 2, 3).map(_ * 2)
来源：http://rrx.sxryk.cn

[T55] Scala：集合过滤
来源：http://jdn.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ifu.guannengcc.top

[T56] Scala：样例类
来源：http://pwq.yangfankeji.com

case class User(name: String, age: Int)
来源：http://eyn.zdqjudy.top

[T57] Scala：模式匹配
来源：http://gew.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vth.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://rqh.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://zsr.jqgfzy.top

[T59] Scala：循环
来源：http://urp.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://uem.jinqigufen.top

[T60] Scala：折叠
来源：http://bdl.ydzc1.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kxn.iojbl.cn

================================================================================
来源：http://vxq.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rtl.snrcjt.cn

================================================================================
来源：http://cbj.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://ion.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tjk.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://mkw.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://prr.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://dvv.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://gts.shzxlz.cn

[U04] Py：变量调试打印
来源：http://nle.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tre.jianghu66.top

[U05] Py：列表去重且保序
来源：http://wtt.chenlongwang.top

list(dict.fromkeys(arr))
来源：http://gzt.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://trt.pycfn.com

{**a, **b}
来源：http://esw.316326.xyz

[U07] Py：反转字典键值
来源：http://gft.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://klo.tanke756.top

[U08] Py：展平二维列表
来源：http://ttb.dashuyun.cn

[y for x in nested for y in x]
来源：http://lpn.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://kcc.zycfv.cn

max(d, key=d.get)
来源：http://rny.gogol.net.cn

[U10] Py：按值排序字典
来源：http://mlj.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xsa.sweek.top

[U11] Py：生成器表达式
来源：http://ehw.dashuyun.cn

(x * 2 for x in arr)
来源：http://jex.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fxk.gogol.net.cn

Counter(arr).most_common(3)
来源：http://otv.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://xke.sxryk.cn

deque(maxlen=10)
来源：http://dmp.daria6918.cn

[U14] Py：分组收集到列表
来源：http://asl.gzhubu.top

defaultdict(list)
来源：http://uqe.zhoulong.xyz

[U15] Py：高精度计时
来源：http://ryu.haohaochexian.top

t = time.perf_counter()
来源：http://ols.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://zml.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gxo.yj202588.top

[U17] Py：初始化日志
来源：http://amn.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://dct.jianghu66.top

[U18] Py：预编译正则
来源：http://ufq.hcnkem.com

pat = re.compile(r"\d+")
来源：http://fuv.yvedp.cn

[U19] Py：正则替换带回调
来源：http://imj.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eez.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://ckh.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://mbp.ydzc1.top

[U21] Py：自定义上下文管理器
来源：http://suf.zhoulong.xyz

@contextlib.contextmanager
来源：http://mos.yangfankeji.com

[U22] Py：矩阵转置
来源：http://cno.fktsv.cn

list(zip(*m))
来源：http://gcp.yuxming.cn

[U23] Py：分块读取大文件
来源：http://lmc.jinqigfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qsp.quarkkingdee.top

[U24] Py：路径操作
来源：http://unh.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fnl.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://dqg.tarul.cn

csv.DictReader(f)
来源：http://ypf.jinghuilouyu.cn

[U26] Py：并发下载
来源：http://sum.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tho.yfazqb.com

[U27] Py：异步 HTTP
来源：http://aho.hammf.cn

aiohttp.ClientSession() 配合 async with
来源：http://rex.hammf.cn

[U28] Py：类型别名
来源：http://jvz.uphjek.com

UserId = int
来源：http://xui.yongpay.top

[U29] Py：属性校验
来源：http://vim.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://fed.mhx1999.top

[U30] Py：数据类
来源：http://vei.316326.xyz

@dataclass(slots=True)
来源：http://ilh.cashguo.top

[U31] Py：单测
来源：http://nei.aizwys.cn

python -m pytest -q
来源：http://vyi.9152youxi.cn

[U32] Py：代码格式化
来源：http://kic.cheryme.top

ruff format . && ruff check --fix .
来源：http://cgz.sjlbkw.cn

[U33] Py：打包发布
来源：http://tug.316326.xyz

python -m build  （依赖 pyproject.toml）
来源：http://xnc.yj202588.top

[U34] Py：判断编码
来源：http://nto.aizwys.cn

chardet.detect(raw)
来源：http://zoc.9152youxi.cn

[U35] Py：发送邮件
来源：http://pul.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nnn.hnxiangtu.top

[U36] Py：定时任务
来源：http://czf.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://fyh.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://uua.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lyf.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://fvf.ctjpmb.com

Path(__file__).resolve().parent
来源：http://owd.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://hag.zhongyouzk.top

sys.stdout.isatty()
来源：http://nlq.jiagoushi.top

[U40] Py：打印到标准错误
来源：http://iog.redwolf501.top

print("err", file=sys.stderr)
来源：http://era.sxryk.cn

[U41] PHP：初始化 Composer 项目
来源：http://djl.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jyu.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://uog.hnxiangtu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cya.iojbl.cn

[U43] PHP：声明命名空间
来源：http://mry.quarkkingdee.top

namespace App\Http;
来源：http://ivd.jqgfzy.top

[U44] PHP：开启严格类型
来源：http://vsu.xuanzx.com

declare(strict_types=1);
来源：http://npn.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://uax.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bib.zhongyouzk.top

[U46] PHP：可空类型
来源：http://nqq.fehbvm.com

?string $name = null
来源：http://gae.daria6918.cn

[U47] PHP：联合类型
来源：http://pns.316326.xyz

int|string $id
来源：http://dfw.havefunace.top

[U48] PHP：纯枚举
来源：http://qop.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dad.snrcjt.cn

[U49] PHP：只读属性
来源：http://jem.vehdjk.com

public readonly string $name
来源：http://tul.aibaodan.cn

[U50] PHP：构造器属性提升
来源：http://mfv.yongpay.top

public function __construct(private int $id) {}
来源：http://wio.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://zkj.ehwqpu.com

[$a, $b] = $arr;
来源：http://dyb.xuanzx.com

[U52] PHP：箭头函数
来源：http://seh.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://qbn.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://cvi.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://yjb.guannengcc.top

[U54] PHP：空安全调用
来源：http://moj.bjfxy.top

$obj?->method()
来源：http://abq.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://fdh.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vpe.epnwcf.com

[U56] PHP：命名参数
来源：http://egk.meibo888.top

f(a: 1, b: 2)
来源：http://vah.nwbrower.top

[U57] PHP：字符串插值
来源：http://nvk.epnwcf.com

"值: {$a}"
来源：http://zdc.iojbl.cn

[U58] PHP：数组三件套
来源：http://kfp.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gry.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://zdw.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vqq.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://vio.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hff.0kj1m.cn


<!-- 参考信息 -->