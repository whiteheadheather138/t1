代发 wailian999

[S41] C++：类与构造函数
来源：http://vnm.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cse.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://kra.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://uyp.hcnkem.com

[S43] C++：智能指针
来源：http://kga.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://uex.hammf.cn

[S44] C++：引用传参
来源：http://mgr.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://csd.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://vbq.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://oxl.yongpay.top

[S46] C++：函数模板
来源：http://kcc.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://owm.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://yon.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hbj.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://mfg.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://aoh.c1oappe.top

while (std::getline(in, line)) { }
来源：http://cxs.daria6918.cn

[S49] C++：写文件
来源：http://kjg.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://msi.zhengqikj.top

[S50] C++：格式化数字
来源：http://vgj.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bpl.xylfe.cn

[S51] C++：显式类型转换
来源：http://ayj.hcnkem.com

static_cast<double>(a) / b
来源：http://nnv.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://wao.yj20258888.top

int size() const noexcept { return n_; }
来源：http://apr.birdmap.top

[S53] C++：移动语义
来源：http://hco.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://fcw.epnwcf.com

[S54] C++：异常处理
来源：http://odc.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://esa.wangdashe.top

[S55] C++：结构化绑定
来源：http://pou.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://nqt.zhaomingkeji.xyz

[S56] C++：optional
来源：http://jan.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pzo.hammf.cn

[S57] C++：编译期常量
来源：http://dgc.0kj1m.cn

constexpr int N = 10;
来源：http://eqa.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://xny.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://vcd.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://rjt.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fih.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://xrb.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vor.xuetiantiany.cn

================================================================================
来源：http://ind.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://abw.svipenyu.cn

================================================================================
来源：http://owb.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://dlx.svipenyu.cn

println("Hello")
来源：http://kwd.zhijiandao.cn

[T02] Kotlin：变量
来源：http://scv.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://crv.yj202588.top

[T03] Kotlin：字符串模板
来源：http://nqg.sysykeji.top

"值: $b"
来源：http://ily.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://sul.birdmap.top

val n: String? = null;  n?.length
来源：http://zmt.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://qku.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://psm.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://jyl.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://zbd.hywenlv.cn

[T07] Kotlin：集合过滤
来源：http://tvd.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vra.fehbvm.com

[T08] Kotlin：数据类
来源：http://boi.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://wyt.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://zkl.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://ket.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://oyo.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://etj.daria6918.cn

[T11] Kotlin：协程
来源：http://jvg.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rkt.hammf.cn

[T12] Kotlin：解构声明
来源：http://got.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://xaz.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://yet.daria6918.cn

val m = mapOf("a" to 1)
来源：http://pwz.yangfankeji.com

[T14] Kotlin：循环
来源：http://ydh.yfazqb.com

for (i in 1..10) println(i)
来源：http://shq.jianghu66.top

[T15] Kotlin：接口
来源：http://wxa.fktsv.cn

interface Shape { fun area(): Double }
来源：http://wzz.zhoulong.xyz

[T16] Swift：Hello World
来源：http://evj.yangfankeji.com

print("Hello")
来源：http://rfr.yuxming.cn

[T17] Swift：变量与常量
来源：http://gmc.zycfv.cn

var a = 1;  let b = 2
来源：http://ynd.aizwys.cn

[T18] Swift：字符串插值
来源：http://rly.fengsongda.top

"值: \(b)"
来源：http://iom.hcnkem.com

[T19] Swift：可选绑定
来源：http://ijl.zdbjq.cn

if let n = opt { print(n) }
来源：http://utv.fzhhl.top

[T20] Swift：数组操作
来源：http://eve.fehbvm.com

var a = [1, 2, 3];  a.append(4)
来源：http://gxt.cashguo.top

[T21] Swift：遍历
来源：http://nea.gotoacloud.top

for x in a { print(x) }
来源：http://rpw.quarkkingdee.top

[T22] Swift：字典
来源：http://hvv.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://egh.xuetiantiany.cn

[T23] Swift：函数
来源：http://wnz.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pug.sjlbkw.cn

[T24] Swift：闭包
来源：http://unk.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hgq.bjfxy.top

[T25] Swift：结构体
来源：http://bdv.hesvh.cn

struct P { var x: Int }
来源：http://rxg.52xcode.cn

[T26] Swift：类与重写
来源：http://xuf.guannengcc.top

class A: Base { override func f() {} }
来源：http://gnt.chenzaomai.com

[T27] Swift：错误处理
来源：http://jhn.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://ldy.zhoulong.xyz

[T28] Swift：枚举
来源：http://jqg.yj202588.top

enum Color { case red, green }
来源：http://ltd.sweek.top

[T29] Swift：guard 提前返回
来源：http://vbh.xuetiantiany.cn

guard let x = opt else { return }
来源：http://cac.fzhhl.top

[T30] Swift：协议
来源：http://tcd.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://ljv.gaohongyu789.top

[T31] Lua：Hello World
来源：http://alv.zhixingplan.top

print("Hello")
来源：http://key.gzhubu.top

[T32] Lua：局部变量
来源：http://txv.jyoumei.cn

local a = 1
来源：http://aid.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://ejk.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mpu.tian-w.cn

[T34] Lua：遍历表
来源：http://jpf.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gig.zhoulong.xyz

[T35] Lua：字典表
来源：http://otg.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://xli.uphjek.com

[T36] Lua：函数
来源：http://yeg.cqqwz.cn

function add(a, b) return a + b end
来源：http://rnw.jqgfzy.top

[T37] Lua：字符串拼接
来源：http://zdy.zhijiandao.cn

"a" .. "b"
来源：http://iri.dianchejie.cn

[T38] Lua：条件
来源：http://zbo.yfazqb.com

if x > 0 then print("正") end
来源：http://pwq.dashuyun.cn

[T39] Lua：模式匹配
来源：http://jam.hywenlv.cn

string.find(s, "%d+")
来源：http://ocf.xziqi.cn

[T40] Lua：元表
来源：http://ldw.zhixingplan.top

setmetatable({}, { __index = base })
来源：http://rfk.quarkkingdee.top

[T41] Perl：Hello World
来源：http://zew.hfpthk.cn

print "Hello\n";
来源：http://vec.yj202588.top

[T42] Perl：变量类型
来源：http://rpn.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ouj.yuanzhike.top

[T43] Perl：字符串插值
来源：http://jla.aibaodan.cn

"值: $a"
来源：http://nyw.chenjidiqi.icu

[T44] Perl：条件
来源：http://dww.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://hcq.xylfe.cn

[T45] Perl：数组遍历
来源：http://qfs.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://koy.c1oappe.top

[T46] Perl：哈希操作
来源：http://zzm.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wij.sufxvd.cn

[T47] Perl：正则捕获
来源：http://pdt.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bks.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://xdx.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://lag.yanxiufei.cn

[T49] Perl：函数
来源：http://hhm.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uyn.xinyue.icu

[T50] Perl：逐行读文件
来源：http://zwr.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://olq.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://lyt.dianchejie.cn

[T51] Scala：Hello World
来源：http://xfm.iojbl.cn

println("Hello")
来源：http://hmy.nwbrower.top

[T52] Scala：变量
来源：http://hhn.uphjek.com

val a = 1;  var b = 2
来源：http://pzh.52xcode.cn

[T53] Scala：字符串插值
来源：http://pqu.ybcxt.top

s"值: $b"
来源：http://ohb.ivvv.top

[T54] Scala：集合映射
来源：http://uvb.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://edk.birdmap.top

[T55] Scala：集合过滤
来源：http://sby.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ipa.meibo888.top

[T56] Scala：样例类
来源：http://agz.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://ole.hysaishi.cn

[T57] Scala：模式匹配
来源：http://itf.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mgj.sysykeji.top

[T58] Scala：函数定义
来源：http://swk.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://ynw.quarkkingdee.top

[T59] Scala：循环
来源：http://crl.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://nzz.ydzc1.top

[T60] Scala：折叠
来源：http://ixa.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://psi.mhx1999.top

================================================================================
来源：http://brj.sweek.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://azb.zhengqikj.top

================================================================================
来源：http://mln.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://xpb.tanke756.top

python -m venv .venv && source .venv/bin/activate
来源：http://lff.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://xsq.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xxl.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://pfk.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fbs.yuxming.cn

[U04] Py：变量调试打印
来源：http://uno.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yzw.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://hkn.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://kac.uphjek.com

[U06] Py：合并两个字典
来源：http://sqn.daria6918.cn

{**a, **b}
来源：http://ohv.zycfv.cn

[U07] Py：反转字典键值
来源：http://wyq.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://izi.bbcook.cn

[U08] Py：展平二维列表
来源：http://tfs.hysaishi.cn

[y for x in nested for y in x]
来源：http://vxj.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://ykt.haohaochexian.top

max(d, key=d.get)
来源：http://bzs.cheryme.top

[U10] Py：按值排序字典
来源：http://ifp.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ydm.hesvh.cn

[U11] Py：生成器表达式
来源：http://qsm.yj202588.top

(x * 2 for x in arr)
来源：http://asu.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://qgp.aibaodan.cn

Counter(arr).most_common(3)
来源：http://ich.dashuyun.cn

[U13] Py：固定长度队列
来源：http://ldo.yuxming.cn

deque(maxlen=10)
来源：http://kmm.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://unp.guowangkeji.top

defaultdict(list)
来源：http://sta.52xcode.cn

[U15] Py：高精度计时
来源：http://lie.ppjwa.cn

t = time.perf_counter()
来源：http://uyr.yj20258.top

[U16] Py：命令行参数解析
来源：http://xes.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hkn.aibaodan.cn

[U17] Py：初始化日志
来源：http://man.bjfxy.top

logging.basicConfig(level=logging.INFO)
来源：http://fhr.birdmap.top

[U18] Py：预编译正则
来源：http://wpu.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://abm.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://jjq.shanyushiyangtech.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mgy.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://blj.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://hek.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://iik.xinyue.icu

@contextlib.contextmanager
来源：http://idx.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://azu.ydjk.org.cn

list(zip(*m))
来源：http://jdu.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://owh.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nhr.sysykeji.top

[U24] Py：路径操作
来源：http://hvv.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pym.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://jhk.hammf.cn

csv.DictReader(f)
来源：http://czb.zhixingplan.top

[U26] Py：并发下载
来源：http://cjf.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://udz.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://vco.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://cko.hywenlv.cn

[U28] Py：类型别名
来源：http://qzq.tanke756.top

UserId = int
来源：http://qcd.hysaishi.cn

[U29] Py：属性校验
来源：http://let.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://kfk.hysaishi.cn

[U30] Py：数据类
来源：http://pkc.0kj1m.cn

@dataclass(slots=True)
来源：http://shq.yj202588.top

[U31] Py：单测
来源：http://fhf.fehbvm.com

python -m pytest -q
来源：http://raz.uphjek.com

[U32] Py：代码格式化
来源：http://mps.hesvh.cn

ruff format . && ruff check --fix .
来源：http://xex.yj202588.top

[U33] Py：打包发布
来源：http://uom.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://fqv.52xcode.cn

[U34] Py：判断编码
来源：http://okt.52xcode.cn

chardet.detect(raw)
来源：http://xgt.tianlin.xyz

[U35] Py：发送邮件
来源：http://jsd.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gmf.nwbrower.top

[U36] Py：定时任务
来源：http://kxn.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://gug.xziqi.cn

[U37] Py：读写 Excel
来源：http://tyv.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://jek.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://soq.vehdjk.com

Path(__file__).resolve().parent
来源：http://yod.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://iqj.yueranfly.top

sys.stdout.isatty()
来源：http://djg.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://cis.jinqigufen.top

print("err", file=sys.stderr)
来源：http://wyb.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://rcf.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uug.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://mib.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://toj.snrcjt.cn

[U43] PHP：声明命名空间
来源：http://wqe.bjfxy.top

namespace App\Http;
来源：http://bci.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://tfe.xuetiantiany.cn

declare(strict_types=1);
来源：http://zje.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://abt.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cek.jlsjyb.cn

[U46] PHP：可空类型
来源：http://xii.sjlbkw.cn

?string $name = null
来源：http://btn.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://glt.yanxiufei.cn

int|string $id
来源：http://cbz.zycfv.cn

[U48] PHP：纯枚举
来源：http://yqd.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ego.redwolf501.top

[U49] PHP：只读属性
来源：http://gkz.ydjk.org.cn

public readonly string $name
来源：http://mpr.xinyue.icu

[U50] PHP：构造器属性提升
来源：http://gcl.ctjpmb.com

public function __construct(private int $id) {}
来源：http://gcm.xziqi.cn

[U51] PHP：数组解构
来源：http://tlu.bjfxy.top

[$a, $b] = $arr;
来源：http://vot.gotoacloud.top

[U52] PHP：箭头函数
来源：http://jzg.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://dgm.gogol.net.cn

[U53] PHP：空合并运算符
来源：http://tbm.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://myr.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://muq.guowangkeji.top

$obj?->method()
来源：http://jpd.tianlin.xyz

[U55] PHP：match 表达式
来源：http://uha.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kwi.sxryk.cn

[U56] PHP：命名参数
来源：http://afi.hnxiangtu.top

f(a: 1, b: 2)
来源：http://itp.tarul.cn

[U57] PHP：字符串插值
来源：http://kik.zhijiandao.cn

"值: {$a}"
来源：http://jpj.pycfn.com

[U58] PHP：数组三件套
来源：http://vot.fzhhl.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://snr.yongpay.top

[U59] PHP：自定义排序
来源：http://ahl.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pvk.cheryme.top

[U60] PHP：JSON 编解码
来源：http://rum.shanyushiyangtech.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lud.tian-w.cn

[U61] PHP：正则
来源：http://bfg.sjlbkw.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://phu.ydjk.org.cn

[U62] PHP：日期对象
来源：http://kft.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lvd.chenzaomai.com

[U63] PHP：文件读写
来源：http://rqe.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zcy.ybcxt.top

[U64] PHP：目录遍历
来源：http://zvt.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://hua.sufxvd.cn

[U65] PHP：会话
来源：http://ypa.vqdsnc.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zdv.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://ibe.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xvm.zhengqikj.top


<!-- 参考信息 -->