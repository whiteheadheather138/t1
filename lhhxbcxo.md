代发 wailian999

[S37] C++：set
来源：http://bnh.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://emr.nanxuanxn.top

[S38] C++：排序
来源：http://dac.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://qpd.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://miy.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xnl.hammf.cn

[S40] C++：查找元素
来源：http://cxj.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nvc.yj20258.top

[S41] C++：类与构造函数
来源：http://jkm.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wmn.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://pyy.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://tqq.zhongyouzk.top

[S43] C++：智能指针
来源：http://qdm.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://cai.zycfv.cn

[S44] C++：引用传参
来源：http://ivd.fzhhl.top

void inc(int &x) { ++x; }
来源：http://wru.pengpengdd.cyou

[S45] C++：lambda
来源：http://juh.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fei.havefunace.top

[S46] C++：函数模板
来源：http://fpt.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sng.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://ufh.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kkj.cqqwz.cn

[S48] C++：逐行读文件
来源：http://uyl.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eht.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://bei.redwolf501.top

[S49] C++：写文件
来源：http://hfb.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jvn.hfpthk.cn

[S50] C++：格式化数字
来源：http://how.fzhhl.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dce.guannengcc.top

[S51] C++：显式类型转换
来源：http://rst.zhoulong.xyz

static_cast<double>(a) / b
来源：http://lai.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://yoi.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://yuv.chenzaomai.com

[S53] C++：移动语义
来源：http://hjo.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://xib.nanxuanxn.top

[S54] C++：异常处理
来源：http://efq.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cjf.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://chp.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yge.ydjk.org.cn

[S56] C++：optional
来源：http://rkc.uphjek.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zaz.haohaochexian.top

[S57] C++：编译期常量
来源：http://xlc.wangdashe.top

constexpr int N = 10;
来源：http://ddn.zhoulong.xyz

[S58] C++：命名空间
来源：http://bed.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://owg.dashuyun.cn

[S59] C++：静态断言
来源：http://rnl.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wyo.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://aem.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sjw.zhiwuduotai.top

================================================================================
来源：http://prx.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://umf.ehwqpu.com

================================================================================
来源：http://aqq.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://oxc.guannengcc.top

println("Hello")
来源：http://tjm.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://pey.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://khc.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://vub.chenzaomai.com

"值: $b"
来源：http://rsi.ppjwa.cn

[T04] Kotlin：空安全
来源：http://kan.ctjpmb.com

val n: String? = null;  n?.length
来源：http://uba.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://brz.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eqd.hfpthk.cn

[T06] Kotlin：集合映射
来源：http://axo.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ygj.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://zzn.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ned.yj202588.top

[T08] Kotlin：数据类
来源：http://mrs.bbcook.cn

data class User(val name: String, val age: Int)
来源：http://wvh.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://eix.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://cgy.xylfe.cn

[T10] Kotlin：默认参数
来源：http://tgh.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kvk.yanxiufei.cn

[T11] Kotlin：协程
来源：http://awm.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://odx.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://txq.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://gap.nanxinkj.top

[T13] Kotlin：只读 Map
来源：http://viu.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://mfs.meibo888.top

[T14] Kotlin：循环
来源：http://oii.epnwcf.com

for (i in 1..10) println(i)
来源：http://wxg.dianchejie.cn

[T15] Kotlin：接口
来源：http://ekq.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://pcq.zdqjudy.top

[T16] Swift：Hello World
来源：http://hkc.zhiwuduotai.top

print("Hello")
来源：http://vge.meibo888.top

[T17] Swift：变量与常量
来源：http://wud.jqgufenzy.top

var a = 1;  let b = 2
来源：http://kkj.chenlongwang.top

[T18] Swift：字符串插值
来源：http://vrc.haohaochexian.top

"值: \(b)"
来源：http://xnb.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://iwy.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://ell.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://vdl.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://jic.dianchejie.cn

[T21] Swift：遍历
来源：http://vxx.zhongyouzk.top

for x in a { print(x) }
来源：http://emx.hnqzz.top

[T22] Swift：字典
来源：http://czu.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hqk.chenzaomai.com

[T23] Swift：函数
来源：http://qde.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wuk.xziqi.cn

[T24] Swift：闭包
来源：http://ieh.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cnl.kuanghao11.cn

[T25] Swift：结构体
来源：http://zva.bjfxy.top

struct P { var x: Int }
来源：http://yep.xinyue.icu

[T26] Swift：类与重写
来源：http://txb.zhixingplan.top

class A: Base { override func f() {} }
来源：http://efk.wangdashe.top

[T27] Swift：错误处理
来源：http://mum.jianghu66.top

do { try f() } catch { print(error) }
来源：http://azk.yanxiufei.cn

[T28] Swift：枚举
来源：http://nkf.yuxming.cn

enum Color { case red, green }
来源：http://wvy.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://jud.bbcook.cn

guard let x = opt else { return }
来源：http://zry.zhixingplan.top

[T30] Swift：协议
来源：http://cau.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://gxm.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://qzy.zdqjudy.top

print("Hello")
来源：http://tmu.svipenyu.cn

[T32] Lua：局部变量
来源：http://hsp.cdnleiting.top

local a = 1
来源：http://cbo.52xcode.cn

[T33] Lua：表（数组）
来源：http://wxz.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://vfo.ydzc1.top

[T34] Lua：遍历表
来源：http://cvv.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jaq.chenzaomai.com

[T35] Lua：字典表
来源：http://msz.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://nom.yuxming.cn

[T36] Lua：函数
来源：http://nvq.52xcode.cn

function add(a, b) return a + b end
来源：http://lan.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://fzz.zhijiandao.cn

"a" .. "b"
来源：http://hvm.uphjek.com

[T38] Lua：条件
来源：http://ywd.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://esk.smart0.xyz

[T39] Lua：模式匹配
来源：http://igz.sufxvd.cn

string.find(s, "%d+")
来源：http://wds.daria6918.cn

[T40] Lua：元表
来源：http://acu.ehwqpu.com

setmetatable({}, { __index = base })
来源：http://zxh.yvedp.cn

[T41] Perl：Hello World
来源：http://ufk.cqqwz.cn

print "Hello\n";
来源：http://lux.cucudq.cn

[T42] Perl：变量类型
来源：http://ixx.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://onv.gotoacloud.top

[T43] Perl：字符串插值
来源：http://jlo.xylfe.cn

"值: $a"
来源：http://zom.andypj.xyz

[T44] Perl：条件
来源：http://eks.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://wxg.guannengcc.top

[T45] Perl：数组遍历
来源：http://aqv.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://jiw.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://vwx.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ldw.jqgfzy.top

[T47] Perl：正则捕获
来源：http://hwu.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hzf.0kj1m.cn

[T48] Perl：正则替换
来源：http://owj.fengsongda.top

$s =~ s/old/new/g;
来源：http://bmf.sxryk.cn

[T49] Perl：函数
来源：http://dxj.uphjek.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zyn.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://sts.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://sms.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://avm.yfazqb.com

[T51] Scala：Hello World
来源：http://rgd.c1oappe.top

println("Hello")
来源：http://ayx.jinyuanbaomall.cn

[T52] Scala：变量
来源：http://chp.zycfv.cn

val a = 1;  var b = 2
来源：http://xph.uphjek.com

[T53] Scala：字符串插值
来源：http://gbi.jqgfzy.top

s"值: $b"
来源：http://veh.yonumen.top

[T54] Scala：集合映射
来源：http://ipt.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://nne.nwbrower.top

[T55] Scala：集合过滤
来源：http://fne.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://erw.epnwcf.com

[T56] Scala：样例类
来源：http://nwc.ivvv.top

case class User(name: String, age: Int)
来源：http://unl.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://ocu.hfpthk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cxu.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://lhp.sysykeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://tjh.zdqjudy.top

[T59] Scala：循环
来源：http://sgn.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://jes.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://psg.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jjw.shanyushiyangtech.top

================================================================================
来源：http://rud.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ngz.nwbrower.top

================================================================================
来源：http://vqh.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://smr.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://vrn.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://xsq.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mdy.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://alg.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://frq.sxryk.cn

[U04] Py：变量调试打印
来源：http://qzc.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hko.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://tse.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://pug.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://gnf.yj20258.top

{**a, **b}
来源：http://kpu.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://yfb.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://rfw.iojbl.cn

[U08] Py：展平二维列表
来源：http://xgn.jinqigfzy.top

[y for x in nested for y in x]
来源：http://mdb.yanxiufei.cn

[U09] Py：字典取最大值的键
来源：http://jya.pycfn.com

max(d, key=d.get)
来源：http://cju.fktsv.cn

[U10] Py：按值排序字典
来源：http://mvl.mhx1999.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yiy.wangshuangyany.cn

[U11] Py：生成器表达式
来源：http://kza.cqqwz.cn

(x * 2 for x in arr)
来源：http://bun.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ssp.hesvh.cn

Counter(arr).most_common(3)
来源：http://ylr.svipenyu.cn

[U13] Py：固定长度队列
来源：http://nqz.cucudq.cn

deque(maxlen=10)
来源：http://pwd.hesvh.cn

[U14] Py：分组收集到列表
来源：http://ufy.aizwys.cn

defaultdict(list)
来源：http://nea.gogol.net.cn

[U15] Py：高精度计时
来源：http://jet.dianchejie.cn

t = time.perf_counter()
来源：http://ecz.shuidangran.top

[U16] Py：命令行参数解析
来源：http://fsq.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://phv.yueranfly.top

[U17] Py：初始化日志
来源：http://bjv.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://yxk.zhijiandao.cn

[U18] Py：预编译正则
来源：http://sty.zycfv.cn

pat = re.compile(r"\d+")
来源：http://ogk.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://pqp.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ele.yueranfly.top

[U20] Py：缓存函数结果
来源：http://njv.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://fub.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://qhg.jinqigufen.top

@contextlib.contextmanager
来源：http://ndr.ehwqpu.com

[U22] Py：矩阵转置
来源：http://zkn.vehdjk.com

list(zip(*m))
来源：http://cdt.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://ksl.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://swt.jianghu66.top

[U24] Py：路径操作
来源：http://tbd.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fon.yj202588.top

[U25] Py：CSV 按字典读
来源：http://oox.xuetiantiany.cn

csv.DictReader(f)
来源：http://twq.iojbl.cn

[U26] Py：并发下载
来源：http://wbp.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pgi.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://leo.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://bkb.cashguo.top

[U28] Py：类型别名
来源：http://jfz.cdnleiting.top

UserId = int
来源：http://ljv.birdmap.top

[U29] Py：属性校验
来源：http://mod.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://scv.daxiang520.top

[U30] Py：数据类
来源：http://ecj.sufxvd.cn

@dataclass(slots=True)
来源：http://ygj.fengsongda.top

[U31] Py：单测
来源：http://csy.zhiwuduotai.top

python -m pytest -q
来源：http://fxg.zhongyouzk.top

[U32] Py：代码格式化
来源：http://vgn.xinyue.icu

ruff format . && ruff check --fix .
来源：http://imp.yj202588.top

[U33] Py：打包发布
来源：http://yao.chenjidiqi.icu

python -m build  （依赖 pyproject.toml）
来源：http://vfw.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://dit.uphjek.com

chardet.detect(raw)
来源：http://gqm.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://wrp.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vmy.chenzaomai.com

[U36] Py：定时任务
来源：http://hbi.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://hqh.yuxming.cn

[U37] Py：读写 Excel
来源：http://zug.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://ado.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://tdd.yj20258888.top

Path(__file__).resolve().parent
来源：http://kza.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://wop.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://xop.xziqi.cn

[U40] Py：打印到标准错误
来源：http://lnw.yangfankeji.com

print("err", file=sys.stderr)
来源：http://swz.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://ntx.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mzf.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://npb.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fyf.sjlbkw.cn

[U43] PHP：声明命名空间
来源：http://mct.zhiwuduotai.top

namespace App\Http;
来源：http://qcw.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://lbx.vehdjk.com

declare(strict_types=1);
来源：http://fsv.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://oyb.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uqs.chenzaomai.com

[U46] PHP：可空类型
来源：http://gyf.hysaishi.cn

?string $name = null
来源：http://ttt.sufxvd.cn

[U47] PHP：联合类型
来源：http://lmz.daxiang520.top

int|string $id
来源：http://oxb.tian-w.cn

[U48] PHP：纯枚举
来源：http://nkn.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sdr.yvedp.cn

[U49] PHP：只读属性
来源：http://djh.zhoulong.xyz

public readonly string $name
来源：http://mfj.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://pnr.meibo888.top

public function __construct(private int $id) {}
来源：http://zqh.smart0.xyz

[U51] PHP：数组解构
来源：http://lka.wangdashe.top

[$a, $b] = $arr;
来源：http://vvk.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://fwa.nwbrower.top

$double = fn($x) => $x * 2;
来源：http://ghp.yfazqb.com

[U53] PHP：空合并运算符
来源：http://pdm.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://dce.c1oappe.top

[U54] PHP：空安全调用
来源：http://ree.ehwqpu.com

$obj?->method()
来源：http://hwm.snrcjt.cn

[U55] PHP：match 表达式
来源：http://nhj.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qgx.cashguo.top

[U56] PHP：命名参数
来源：http://ibn.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://vtt.jlsjyb.cn

[U57] PHP：字符串插值
来源：http://aus.jlsjyb.cn

"值: {$a}"
来源：http://xbn.fktsv.cn

[U58] PHP：数组三件套
来源：http://pej.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ylt.mhx1999.top

[U59] PHP：自定义排序
来源：http://ixj.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cpr.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://guz.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wtg.chenlongwang.top

[U61] PHP：正则
来源：http://rgh.birdmap.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hbd.jqgfzy.top

[U62] PHP：日期对象
来源：http://vug.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qfa.jiagoushi.top


<!-- 参考信息 -->