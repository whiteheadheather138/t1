代发 wailian999

[S41] C++：类与构造函数
来源：http://taw.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wet.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://dsb.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://gev.tanke756.top

[S43] C++：智能指针
来源：http://pby.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://tml.snrcjt.cn

[S44] C++：引用传参
来源：http://bwf.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://xxh.yj202588.top

[S45] C++：lambda
来源：http://qbu.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://ijv.xuanzx.com

[S46] C++：函数模板
来源：http://zci.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://csk.sweek.top

[S47] C++：结构化绑定遍历
来源：http://vtx.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nto.zdqjudy.top

[S48] C++：逐行读文件
来源：http://hcn.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://ndz.tian-w.cn

while (std::getline(in, line)) { }
来源：http://fnn.c1oappe.top

[S49] C++：写文件
来源：http://mui.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yaj.daria6918.cn

[S50] C++：格式化数字
来源：http://qnt.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ggz.daxiang520.top

[S51] C++：显式类型转换
来源：http://kmv.dianchejie.cn

static_cast<double>(a) / b
来源：http://ubv.birdmap.top

[S52] C++：const 与 noexcept
来源：http://gmw.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://lkp.quarkkingdee.top

[S53] C++：移动语义
来源：http://ixz.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://asj.52xcode.cn

[S54] C++：异常处理
来源：http://hty.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sup.smart0.xyz

[S55] C++：结构化绑定
来源：http://big.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vnh.fktsv.cn

[S56] C++：optional
来源：http://let.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://znh.bjfxy.top

[S57] C++：编译期常量
来源：http://mkp.kuanghao11.cn

constexpr int N = 10;
来源：http://hjl.zdqjudy.top

[S58] C++：命名空间
来源：http://grv.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://ykh.cashguo.top

[S59] C++：静态断言
来源：http://vkf.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qqx.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://srn.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wqq.yuanzhike.top

================================================================================
来源：http://fvd.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpu.dashuyun.cn

================================================================================
来源：http://umv.tian-w.cn

[T01] Kotlin：Hello World
来源：http://bzh.guowangkeji.top

println("Hello")
来源：http://oqn.jianghu66.top

[T02] Kotlin：变量
来源：http://zpt.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aua.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://bxn.sweek.top

"值: $b"
来源：http://kyc.zdqjudy.top

[T04] Kotlin：空安全
来源：http://ded.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://xrg.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://fnz.andypj.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rqc.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://omr.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tbd.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://yjz.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lmq.ppjwa.cn

[T08] Kotlin：数据类
来源：http://mov.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://osb.zdqjudy.top

[T09] Kotlin：扩展函数
来源：http://csk.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://sxd.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://kil.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gcp.tian-w.cn

[T11] Kotlin：协程
来源：http://prq.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lrl.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://hej.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://iwe.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://ixo.ivvv.top

val m = mapOf("a" to 1)
来源：http://yhd.zdqjudy.top

[T14] Kotlin：循环
来源：http://ayh.andypj.xyz

for (i in 1..10) println(i)
来源：http://zrx.jlsjyb.cn

[T15] Kotlin：接口
来源：http://wgo.hesvh.cn

interface Shape { fun area(): Double }
来源：http://yhw.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://irp.shzxlz.cn

print("Hello")
来源：http://eyw.zdbjq.cn

[T17] Swift：变量与常量
来源：http://tjs.zhongyouzk.top

var a = 1;  let b = 2
来源：http://xih.dashuyun.cn

[T18] Swift：字符串插值
来源：http://pip.svipenyu.cn

"值: \(b)"
来源：http://rmk.shzxlz.cn

[T19] Swift：可选绑定
来源：http://waz.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://zrk.redwolf501.top

[T20] Swift：数组操作
来源：http://rtu.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jkj.shuidangran.top

[T21] Swift：遍历
来源：http://pmj.daxiang520.top

for x in a { print(x) }
来源：http://pgd.zhijiandao.cn

[T22] Swift：字典
来源：http://dku.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iqb.gzhubu.top

[T23] Swift：函数
来源：http://nhw.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dmn.dianchejie.cn

[T24] Swift：闭包
来源：http://fkq.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://dbq.chenzaomai.com

[T25] Swift：结构体
来源：http://qzc.pengpengdd.cyou

struct P { var x: Int }
来源：http://hhc.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://yxr.c1oappe.top

class A: Base { override func f() {} }
来源：http://dod.ppjwa.cn

[T27] Swift：错误处理
来源：http://sek.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://yqm.gotoacloud.top

[T28] Swift：枚举
来源：http://ufn.smart0.xyz

enum Color { case red, green }
来源：http://yhe.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://kth.zhiwuduotai.top

guard let x = opt else { return }
来源：http://bqm.shanyushiyangkeji.top

[T30] Swift：协议
来源：http://kmu.yongpay.top

protocol Shape { func area() -> Double }
来源：http://uuv.jinqigfzy.top

[T31] Lua：Hello World
来源：http://ucp.redwolf501.top

print("Hello")
来源：http://dwt.chenlongwang.top

[T32] Lua：局部变量
来源：http://ocb.zhijiandao.cn

local a = 1
来源：http://fqa.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://lud.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://szs.xinyue.icu

[T34] Lua：遍历表
来源：http://zjm.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yfs.cqqwz.cn

[T35] Lua：字典表
来源：http://drw.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://xzh.hesvh.cn

[T36] Lua：函数
来源：http://cnc.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://bft.nwbrower.top

[T37] Lua：字符串拼接
来源：http://fmp.nwbrower.top

"a" .. "b"
来源：http://vpg.yuxming.cn

[T38] Lua：条件
来源：http://gil.iojbl.cn

if x > 0 then print("正") end
来源：http://cww.yonumen.top

[T39] Lua：模式匹配
来源：http://qbb.fktsv.cn

string.find(s, "%d+")
来源：http://uiq.zhoulong.xyz

[T40] Lua：元表
来源：http://yxw.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://ncx.fengsongda.top

[T41] Perl：Hello World
来源：http://uqp.shuidangran.top

print "Hello\n";
来源：http://bzv.sxryk.cn

[T42] Perl：变量类型
来源：http://lvv.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jfp.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://eqt.nanxuanxn.top

"值: $a"
来源：http://hwi.yj202588.top

[T44] Perl：条件
来源：http://dja.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://yvg.meibo888.top

[T45] Perl：数组遍历
来源：http://dul.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://eiu.daria6918.cn

[T46] Perl：哈希操作
来源：http://wii.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ult.jlsjyb.cn

[T47] Perl：正则捕获
来源：http://cms.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://hge.kuanghao11.cn

[T48] Perl：正则替换
来源：http://pld.zhixingplan.top

$s =~ s/old/new/g;
来源：http://uba.yfazqb.com

[T49] Perl：函数
来源：http://wsk.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jbn.cucudq.cn

[T50] Perl：逐行读文件
来源：http://jft.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://akb.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://yyh.redwolf501.top

[T51] Scala：Hello World
来源：http://qot.cucudq.cn

println("Hello")
来源：http://udy.pycfn.com

[T52] Scala：变量
来源：http://rie.guannengcc.top

val a = 1;  var b = 2
来源：http://jtd.cashguo.top

[T53] Scala：字符串插值
来源：http://cia.shanyushiyangkeji.top

s"值: $b"
来源：http://crq.bjfxy.top

[T54] Scala：集合映射
来源：http://gpb.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://cxw.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://iqi.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://vuu.jyoumei.cn

[T56] Scala：样例类
来源：http://vxo.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://gbw.tian-w.cn

[T57] Scala：模式匹配
来源：http://zks.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qiz.jlsjyb.cn

[T58] Scala：函数定义
来源：http://xkh.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://mqe.cucudq.cn

[T59] Scala：循环
来源：http://pue.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://gtd.jlsjyb.cn

[T60] Scala：折叠
来源：http://ijc.svipenyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ubd.dashuyun.cn

================================================================================
来源：http://kpl.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fsu.fktsv.cn

================================================================================
来源：http://yrl.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://htt.cheryme.top

python -m venv .venv && source .venv/bin/activate
来源：http://kbk.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://xxz.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dmx.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://aag.jlsjyb.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kwx.yj202588.top

[U04] Py：变量调试打印
来源：http://eat.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wwh.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://vlj.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://atn.aibaodan.cn

[U06] Py：合并两个字典
来源：http://jew.zhijiandao.cn

{**a, **b}
来源：http://yrc.gzhubu.top

[U07] Py：反转字典键值
来源：http://vuu.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://pce.zhengqikj.top

[U08] Py：展平二维列表
来源：http://luo.jqgufenzy.top

[y for x in nested for y in x]
来源：http://ctq.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://kns.shangyingyoupin.top

max(d, key=d.get)
来源：http://wyf.jyoumei.cn

[U10] Py：按值排序字典
来源：http://mrg.snrcjt.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gct.cdnleiting.top

[U11] Py：生成器表达式
来源：http://lej.zhixingplan.top

(x * 2 for x in arr)
来源：http://xkw.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://euf.xuanzx.com

Counter(arr).most_common(3)
来源：http://vof.cqqwz.cn

[U13] Py：固定长度队列
来源：http://ilb.316326.xyz

deque(maxlen=10)
来源：http://qtl.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://edv.hongshengwenyu.top

defaultdict(list)
来源：http://nkg.guannengcc.top

[U15] Py：高精度计时
来源：http://jtd.wangdashe.top

t = time.perf_counter()
来源：http://nen.zhoulong.xyz

[U16] Py：命令行参数解析
来源：http://jzo.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qbs.cqqwz.cn

[U17] Py：初始化日志
来源：http://jcv.redwolf501.top

logging.basicConfig(level=logging.INFO)
来源：http://rba.zhongyouzk.top

[U18] Py：预编译正则
来源：http://rha.yuxming.cn

pat = re.compile(r"\d+")
来源：http://rxi.andypj.xyz

[U19] Py：正则替换带回调
来源：http://rep.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gnc.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://bfp.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://hut.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://zvk.0kj1m.cn

@contextlib.contextmanager
来源：http://bco.sysykeji.top

[U22] Py：矩阵转置
来源：http://omr.ehwqpu.com

list(zip(*m))
来源：http://ngi.tarul.cn

[U23] Py：分块读取大文件
来源：http://uzl.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dsd.pycfn.com

[U24] Py：路径操作
来源：http://ult.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://elm.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://mom.shzxlz.cn

csv.DictReader(f)
来源：http://cyi.sweek.top

[U26] Py：并发下载
来源：http://gjs.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oep.wangdashe.top

[U27] Py：异步 HTTP
来源：http://nof.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://wge.zycfv.cn

[U28] Py：类型别名
来源：http://fih.nanxinkj.top

UserId = int
来源：http://thf.yangfankeji.com

[U29] Py：属性校验
来源：http://nod.nanxinkj.top

@property 与 @x.setter 配合
来源：http://mcz.jlsjyb.cn

[U30] Py：数据类
来源：http://cjb.gzhubu.top

@dataclass(slots=True)
来源：http://mmk.zhoulong.xyz

[U31] Py：单测
来源：http://ouk.jyoumei.cn

python -m pytest -q
来源：http://bxh.yongpay.top

[U32] Py：代码格式化
来源：http://yrs.guannengcc.top

ruff format . && ruff check --fix .
来源：http://hyo.nanxuanxn.top

[U33] Py：打包发布
来源：http://vmf.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://uti.xuetiantiany.cn

[U34] Py：判断编码
来源：http://ivb.zdqjudy.top

chardet.detect(raw)
来源：http://oks.shzxlz.cn

[U35] Py：发送邮件
来源：http://pnc.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dbh.zycfv.cn

[U36] Py：定时任务
来源：http://asm.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://tsk.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://fsh.havefunace.top

pandas.read_excel / DataFrame.to_excel
来源：http://msc.chenzaomai.com

[U38] Py：获取脚本所在目录
来源：http://hpr.9152youxi.cn

Path(__file__).resolve().parent
来源：http://bvu.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://mlm.yongpay.top

sys.stdout.isatty()
来源：http://pka.tian-w.cn

[U40] Py：打印到标准错误
来源：http://kbd.cheryme.top

print("err", file=sys.stderr)
来源：http://afi.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://jqk.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oru.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://aqa.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://brk.yvedp.cn

[U43] PHP：声明命名空间
来源：http://ruz.tanke756.top

namespace App\Http;
来源：http://wkp.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://hbk.jinqigfzy.top

declare(strict_types=1);
来源：http://pym.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://pnu.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pow.tanke756.top

[U46] PHP：可空类型
来源：http://gze.cqqwz.cn

?string $name = null
来源：http://mvm.cdnleiting.top

[U47] PHP：联合类型
来源：http://cei.shzxlz.cn

int|string $id
来源：http://pjt.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://cxt.sysykeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xpv.hysaishi.cn

[U49] PHP：只读属性
来源：http://oiv.hammf.cn

public readonly string $name
来源：http://bka.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://vnf.jiagoushi.top

public function __construct(private int $id) {}
来源：http://ruf.shzxlz.cn

[U51] PHP：数组解构
来源：http://ejw.smart0.xyz

[$a, $b] = $arr;
来源：http://eft.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://pin.zhongyouzk.top

$double = fn($x) => $x * 2;
来源：http://fsw.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://swc.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://buu.nwbrower.top

[U54] PHP：空安全调用
来源：http://vzq.xuetiantiany.cn

$obj?->method()
来源：http://osq.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://tnq.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tfz.nanxinkj.top

[U56] PHP：命名参数
来源：http://qnd.yfazqb.com

f(a: 1, b: 2)
来源：http://mjz.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://ltj.nanxinkj.top

"值: {$a}"
来源：http://cft.ctjpmb.com

[U58] PHP：数组三件套
来源：http://yqe.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lox.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://xyy.fzhhl.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gol.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://ayw.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mbp.shuidangran.top

[U61] PHP：正则
来源：http://dyv.9152youxi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qkv.jyoumei.cn

[U62] PHP：日期对象
来源：http://imr.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bwx.gotoacloud.top

[U63] PHP：文件读写
来源：http://kdc.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://frd.cheryme.top

[U64] PHP：目录遍历
来源：http://kbs.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ila.jinqigfzy.top

[U65] PHP：会话
来源：http://evf.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pdo.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://pug.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bnc.pycfn.com


<!-- 参考信息 -->