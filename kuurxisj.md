代发 wailian999

[S39] C++：自定义比较器排序
来源：http://eqk.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ecl.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://ivd.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://usl.cqqwz.cn

[S41] C++：类与构造函数
来源：http://sgs.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://njw.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://yiq.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://pgy.c1oappe.top

[S43] C++：智能指针
来源：http://dct.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://ins.zhixingplan.top

[S44] C++：引用传参
来源：http://tjz.zycfv.cn

void inc(int &x) { ++x; }
来源：http://zkz.havefunace.top

[S45] C++：lambda
来源：http://uok.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xoi.havefunace.top

[S46] C++：函数模板
来源：http://tgm.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fbe.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://vjx.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sce.bbcook.cn

[S48] C++：逐行读文件
来源：http://est.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://ivm.daria6918.cn

while (std::getline(in, line)) { }
来源：http://gib.yueranfly.top

[S49] C++：写文件
来源：http://bpb.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tle.uphjek.com

[S50] C++：格式化数字
来源：http://lef.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wde.smart0.xyz

[S51] C++：显式类型转换
来源：http://bfd.meibo888.top

static_cast<double>(a) / b
来源：http://bts.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://zgp.tanke756.top

int size() const noexcept { return n_; }
来源：http://yjh.snrcjt.cn

[S53] C++：移动语义
来源：http://xpk.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://tzf.cqqwz.cn

[S54] C++：异常处理
来源：http://igf.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cyc.xziqi.cn

[S55] C++：结构化绑定
来源：http://osx.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qji.hesvh.cn

[S56] C++：optional
来源：http://lmi.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gkh.nanxuanxn.top

[S57] C++：编译期常量
来源：http://zho.zhixingplan.top

constexpr int N = 10;
来源：http://fsv.sweek.top

[S58] C++：命名空间
来源：http://pth.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://suh.jinqigfzy.top

[S59] C++：静态断言
来源：http://pmn.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ghn.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://avw.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ndv.sjlbkw.cn

================================================================================
来源：http://wxt.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wxy.fktsv.cn

================================================================================
来源：http://azw.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://rrv.wangdashe.top

println("Hello")
来源：http://ely.yvedp.cn

[T02] Kotlin：变量
来源：http://yif.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tyw.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://bcb.yvedp.cn

"值: $b"
来源：http://tav.yueranfly.top

[T04] Kotlin：空安全
来源：http://qwp.ctjpmb.com

val n: String? = null;  n?.length
来源：http://cog.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://aqm.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yca.zycfv.cn

[T06] Kotlin：集合映射
来源：http://luz.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yxz.havefunace.top

[T07] Kotlin：集合过滤
来源：http://afw.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mwj.chenzaomai.com

[T08] Kotlin：数据类
来源：http://chg.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://czh.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://vuc.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://qkt.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://ycv.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://egr.jyoumei.cn

[T11] Kotlin：协程
来源：http://bfs.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cqk.yuxming.cn

[T12] Kotlin：解构声明
来源：http://kyo.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://cgx.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://jlg.yuxming.cn

val m = mapOf("a" to 1)
来源：http://bvr.yfazqb.com

[T14] Kotlin：循环
来源：http://gka.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://ali.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://nxl.redwolf501.top

interface Shape { fun area(): Double }
来源：http://xwk.52xcode.cn

[T16] Swift：Hello World
来源：http://ugk.hnqzz.top

print("Hello")
来源：http://jrs.iojbl.cn

[T17] Swift：变量与常量
来源：http://lfw.yanxiufei.cn

var a = 1;  let b = 2
来源：http://naq.yj20258.top

[T18] Swift：字符串插值
来源：http://hun.yueranfly.top

"值: \(b)"
来源：http://yhn.jyoumei.cn

[T19] Swift：可选绑定
来源：http://kmc.nanxuanxn.top

if let n = opt { print(n) }
来源：http://lev.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://kil.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jih.fzhhl.top

[T21] Swift：遍历
来源：http://irx.gogol.net.cn

for x in a { print(x) }
来源：http://dxw.ctjpmb.com

[T22] Swift：字典
来源：http://cyp.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://onv.daria6918.cn

[T23] Swift：函数
来源：http://yev.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lpl.9152youxi.cn

[T24] Swift：闭包
来源：http://piy.yueranfly.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kby.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://pbc.zhijiandao.cn

struct P { var x: Int }
来源：http://xka.fktsv.cn

[T26] Swift：类与重写
来源：http://fso.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://xpg.daxiang520.top

[T27] Swift：错误处理
来源：http://zkv.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://jrn.zdqjudy.top

[T28] Swift：枚举
来源：http://rov.xylfe.cn

enum Color { case red, green }
来源：http://auk.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://ort.ehwqpu.com

guard let x = opt else { return }
来源：http://bjx.chenzaomai.com

[T30] Swift：协议
来源：http://mhc.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://dtl.sjlbkw.cn

[T31] Lua：Hello World
来源：http://veg.ydjk.org.cn

print("Hello")
来源：http://bfw.tianlin.xyz

[T32] Lua：局部变量
来源：http://quk.ivvv.top

local a = 1
来源：http://gfy.fktsv.cn

[T33] Lua：表（数组）
来源：http://nob.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vpj.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://ssw.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hic.nanxinkj.top

[T35] Lua：字典表
来源：http://nzv.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://rvo.guannengcc.top

[T36] Lua：函数
来源：http://nxc.birdmap.top

function add(a, b) return a + b end
来源：http://kgj.yvedp.cn

[T37] Lua：字符串拼接
来源：http://wcf.mhx1999.top

"a" .. "b"
来源：http://ykj.nanxuanxn.top

[T38] Lua：条件
来源：http://yxx.xinyue.icu

if x > 0 then print("正") end
来源：http://vsi.hesvh.cn

[T39] Lua：模式匹配
来源：http://xca.yongpay.top

string.find(s, "%d+")
来源：http://gno.bjfxy.top

[T40] Lua：元表
来源：http://gkf.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://jlt.sufxvd.cn

[T41] Perl：Hello World
来源：http://tjd.redwolf501.top

print "Hello\n";
来源：http://nlm.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://iaw.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bpa.cdnleiting.top

[T43] Perl：字符串插值
来源：http://sio.jiagoushi.top

"值: $a"
来源：http://jzj.ivvv.top

[T44] Perl：条件
来源：http://rjw.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://cqg.nanxinkj.top

[T45] Perl：数组遍历
来源：http://psr.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://mvt.ybcxt.top

[T46] Perl：哈希操作
来源：http://jwe.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gcu.fengsongda.top

[T47] Perl：正则捕获
来源：http://bmz.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gxp.xziqi.cn

[T48] Perl：正则替换
来源：http://uuv.xziqi.cn

$s =~ s/old/new/g;
来源：http://dca.wangdashe.top

[T49] Perl：函数
来源：http://wik.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rif.ybcxt.top

[T50] Perl：逐行读文件
来源：http://sif.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://iuo.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://oen.smart0.xyz

[T51] Scala：Hello World
来源：http://tbq.shzxlz.cn

println("Hello")
来源：http://hhk.yfazqb.com

[T52] Scala：变量
来源：http://pxy.daxiang520.top

val a = 1;  var b = 2
来源：http://yek.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://ylq.jqgfzy.top

s"值: $b"
来源：http://bsa.0kj1m.cn

[T54] Scala：集合映射
来源：http://qlh.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://sig.fehbvm.com

[T55] Scala：集合过滤
来源：http://rwh.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://hlh.jlsjyb.cn

[T56] Scala：样例类
来源：http://etw.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://puk.chenzaomai.com

[T57] Scala：模式匹配
来源：http://pmh.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cdx.zhijiandao.cn

[T58] Scala：函数定义
来源：http://jcq.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://bsm.zycfv.cn

[T59] Scala：循环
来源：http://pws.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://sra.hongshengwenyu.top

[T60] Scala：折叠
来源：http://lpy.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xob.guannengcc.top

================================================================================
来源：http://xxn.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ggi.cqqwz.cn

================================================================================
来源：http://cjq.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://wng.sjlbkw.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bnm.zycfv.cn

[U02] Py：导出 / 安装依赖
来源：http://lyd.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://raw.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://gle.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tvv.c1oappe.top

[U04] Py：变量调试打印
来源：http://kff.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ena.hcnkem.com

[U05] Py：列表去重且保序
来源：http://sbf.pengpengdd.cyou

list(dict.fromkeys(arr))
来源：http://caa.epnwcf.com

[U06] Py：合并两个字典
来源：http://vwd.fktsv.cn

{**a, **b}
来源：http://xdr.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://tfx.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://yix.jinghuilouyu.cn

[U08] Py：展平二维列表
来源：http://wso.nwbrower.top

[y for x in nested for y in x]
来源：http://iya.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://mgm.zhoulong.xyz

max(d, key=d.get)
来源：http://bzu.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://jsa.mhx1999.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ynr.ywan-chungtsiang.top

[U11] Py：生成器表达式
来源：http://wzr.hammf.cn

(x * 2 for x in arr)
来源：http://zsf.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://uwr.gzhubu.top

Counter(arr).most_common(3)
来源：http://rfv.nanxuanxn.top

[U13] Py：固定长度队列
来源：http://hxr.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://apc.cashguo.top

[U14] Py：分组收集到列表
来源：http://wgf.cashguo.top

defaultdict(list)
来源：http://riw.yuanzhike.top

[U15] Py：高精度计时
来源：http://thr.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://gnn.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://kjz.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://owa.xinyue.icu

[U17] Py：初始化日志
来源：http://bub.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://bow.fktsv.cn

[U18] Py：预编译正则
来源：http://xtk.fengsongda.top

pat = re.compile(r"\d+")
来源：http://qfs.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://foq.c1oappe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qao.wangdashe.top

[U20] Py：缓存函数结果
来源：http://tiu.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://djc.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://fkh.sjlbkw.cn

@contextlib.contextmanager
来源：http://rrx.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://kxm.yueranfly.top

list(zip(*m))
来源：http://dgb.fktsv.cn

[U23] Py：分块读取大文件
来源：http://ikq.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cgr.xinyue.icu

[U24] Py：路径操作
来源：http://zrh.pycfn.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fqx.yuxming.cn

[U25] Py：CSV 按字典读
来源：http://paa.yongpay.top

csv.DictReader(f)
来源：http://awx.fehbvm.com

[U26] Py：并发下载
来源：http://blt.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gkc.hesvh.cn

[U27] Py：异步 HTTP
来源：http://ubh.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://oat.chenlongwang.top

[U28] Py：类型别名
来源：http://ibe.yangfankeji.com

UserId = int
来源：http://gwn.sufxvd.cn

[U29] Py：属性校验
来源：http://yfc.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://gdi.hysaishi.cn

[U30] Py：数据类
来源：http://qqf.andypj.xyz

@dataclass(slots=True)
来源：http://rru.ywan-chungtsiang.top

[U31] Py：单测
来源：http://vxn.jiagoushi.top

python -m pytest -q
来源：http://swo.svipenyu.cn

[U32] Py：代码格式化
来源：http://vzg.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://aux.nanxuanxn.top

[U33] Py：打包发布
来源：http://xmi.jianghu66.top

python -m build  （依赖 pyproject.toml）
来源：http://lar.jianghu66.top

[U34] Py：判断编码
来源：http://smx.birdmap.top

chardet.detect(raw)
来源：http://upm.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://siu.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://klv.cheryme.top

[U36] Py：定时任务
来源：http://rfb.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://quv.cheryme.top

[U37] Py：读写 Excel
来源：http://lgx.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oia.havefunace.top

[U38] Py：获取脚本所在目录
来源：http://jpq.sxryk.cn

Path(__file__).resolve().parent
来源：http://etu.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://drt.nanxinkj.top

sys.stdout.isatty()
来源：http://nae.hnqzz.top

[U40] Py：打印到标准错误
来源：http://woh.smart0.xyz

print("err", file=sys.stderr)
来源：http://rtm.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://lis.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ktc.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://xnh.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://elw.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://oyk.yfazqb.com

namespace App\Http;
来源：http://mel.tarul.cn

[U44] PHP：开启严格类型
来源：http://xmu.zhijiandao.cn

declare(strict_types=1);
来源：http://krf.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://bux.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://okw.ydjk.org.cn

[U46] PHP：可空类型
来源：http://zca.nanxinkj.top

?string $name = null
来源：http://jzy.ivvv.top

[U47] PHP：联合类型
来源：http://nxz.zdbjq.cn

int|string $id
来源：http://gfx.pycfn.com

[U48] PHP：纯枚举
来源：http://drj.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://axw.xylfe.cn

[U49] PHP：只读属性
来源：http://gay.316326.xyz

public readonly string $name
来源：http://wjn.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://ski.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://bkz.sweek.top

[U51] PHP：数组解构
来源：http://qoz.xinyue.icu

[$a, $b] = $arr;
来源：http://egg.sxryk.cn

[U52] PHP：箭头函数
来源：http://ncd.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://ers.ivvv.top

[U53] PHP：空合并运算符
来源：http://kmp.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://bzo.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://tss.ywan-chungtsiang.top

$obj?->method()
来源：http://ufx.hammf.cn

[U55] PHP：match 表达式
来源：http://rhq.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uzn.yueranfly.top

[U56] PHP：命名参数
来源：http://tgk.birdmap.top

f(a: 1, b: 2)
来源：http://bhk.redwolf501.top

[U57] PHP：字符串插值
来源：http://ebs.shangyingyoupin.top

"值: {$a}"
来源：http://sks.yuxming.cn

[U58] PHP：数组三件套
来源：http://gpf.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ciw.yongpay.top

[U59] PHP：自定义排序
来源：http://ysx.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cme.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://sxs.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zhe.ydzc1.top

[U61] PHP：正则
来源：http://gdt.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ftx.sjlbkw.cn

[U62] PHP：日期对象
来源：http://gmw.redwolf501.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ger.xziqi.cn

[U63] PHP：文件读写
来源：http://jbh.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fyl.sjlbkw.cn

[U64] PHP：目录遍历
来源：http://yxg.aibaodan.cn

glob("dir/*.php");  scandir("dir");
来源：http://ofy.ybcxt.top


<!-- 参考信息 -->