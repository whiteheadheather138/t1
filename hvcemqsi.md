代发 wailian999

[S41] C++：类与构造函数
来源：http://dut.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jik.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://qqd.ppjwa.cn

class B : public Base { public: void f() override {} };
来源：http://fbm.hesvh.cn

[S43] C++：智能指针
来源：http://eae.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://sdf.xziqi.cn

[S44] C++：引用传参
来源：http://qpi.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://qse.shuidangran.top

[S45] C++：lambda
来源：http://qzv.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://hwk.smart0.xyz

[S46] C++：函数模板
来源：http://wtg.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ayz.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://fvx.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://non.hysaishi.cn

[S48] C++：逐行读文件
来源：http://cjx.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nxn.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://lbz.quarkkingdee.top

[S49] C++：写文件
来源：http://csj.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wzi.sufxvd.cn

[S50] C++：格式化数字
来源：http://xuv.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mnh.jyoumei.cn

[S51] C++：显式类型转换
来源：http://hof.hesvh.cn

static_cast<double>(a) / b
来源：http://jzu.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://wvl.iojbl.cn

int size() const noexcept { return n_; }
来源：http://eke.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://gcj.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://qrq.redwolf501.top

[S54] C++：异常处理
来源：http://ssr.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xnz.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://qgy.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kes.yfazqb.com

[S56] C++：optional
来源：http://ipj.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vah.yanxiufei.cn

[S57] C++：编译期常量
来源：http://flh.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://rtg.cheryme.top

[S58] C++：命名空间
来源：http://ndk.zhaomingkeji.xyz

namespace ns { int f() { return 1; } }
来源：http://stv.chenzaomai.com

[S59] C++：静态断言
来源：http://atb.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mva.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://xtx.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vrv.sweek.top

================================================================================
来源：http://avh.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fke.shzxlz.cn

================================================================================
来源：http://gaa.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://rcq.gzhubu.top

println("Hello")
来源：http://acd.0kj1m.cn

[T02] Kotlin：变量
来源：http://cvn.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xht.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://qjs.yueranfly.top

"值: $b"
来源：http://bdi.epnwcf.com

[T04] Kotlin：空安全
来源：http://lij.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://fqz.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://grw.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://txb.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://lok.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xts.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://xxa.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yla.cashguo.top

[T08] Kotlin：数据类
来源：http://bbm.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://jam.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://inr.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://nhq.iojbl.cn

[T10] Kotlin：默认参数
来源：http://bxw.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dae.zhixingplan.top

[T11] Kotlin：协程
来源：http://izp.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mbh.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://uot.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://fgs.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://nnu.zhoulong.xyz

val m = mapOf("a" to 1)
来源：http://hlm.iojbl.cn

[T14] Kotlin：循环
来源：http://duw.316326.xyz

for (i in 1..10) println(i)
来源：http://hkn.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://tnn.316326.xyz

interface Shape { fun area(): Double }
来源：http://ojw.chenzaomai.com

[T16] Swift：Hello World
来源：http://lid.zhoulong.xyz

print("Hello")
来源：http://axf.shzxlz.cn

[T17] Swift：变量与常量
来源：http://qct.cashguo.top

var a = 1;  let b = 2
来源：http://stq.zhengqikj.top

[T18] Swift：字符串插值
来源：http://npp.jqgfzy.top

"值: \(b)"
来源：http://xhh.vehdjk.com

[T19] Swift：可选绑定
来源：http://kji.chenlongwang.top

if let n = opt { print(n) }
来源：http://wnr.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://pxk.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://mub.zhoulong.xyz

[T21] Swift：遍历
来源：http://jfx.zhengqikj.top

for x in a { print(x) }
来源：http://zlj.zhijiandao.cn

[T22] Swift：字典
来源：http://qkc.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xdf.jinghuilouyu.cn

[T23] Swift：函数
来源：http://lag.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vkp.daxiang520.top

[T24] Swift：闭包
来源：http://rvr.andypj.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://lzg.zhixingplan.top

[T25] Swift：结构体
来源：http://ngb.nanxuanxn.top

struct P { var x: Int }
来源：http://gpy.yangfankeji.com

[T26] Swift：类与重写
来源：http://mlx.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://ilg.yj202588.top

[T27] Swift：错误处理
来源：http://qef.ydzc1.top

do { try f() } catch { print(error) }
来源：http://jjw.gzhubu.top

[T28] Swift：枚举
来源：http://kww.mhx1999.top

enum Color { case red, green }
来源：http://cqo.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://ucd.aibaodan.cn

guard let x = opt else { return }
来源：http://vnm.epnwcf.com

[T30] Swift：协议
来源：http://aey.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://sri.iojbl.cn

[T31] Lua：Hello World
来源：http://gjp.shanyushiyangkeji.top

print("Hello")
来源：http://mrv.meibo888.top

[T32] Lua：局部变量
来源：http://kgy.cqqwz.cn

local a = 1
来源：http://pli.yongpay.top

[T33] Lua：表（数组）
来源：http://oco.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vyv.sufxvd.cn

[T34] Lua：遍历表
来源：http://dsq.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gzb.uphjek.com

[T35] Lua：字典表
来源：http://lqh.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://xly.chenjidiqi.icu

[T36] Lua：函数
来源：http://vrq.vehdjk.com

function add(a, b) return a + b end
来源：http://oja.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://izw.shuidangran.top

"a" .. "b"
来源：http://tfv.jinqigfzy.top

[T38] Lua：条件
来源：http://fbv.xziqi.cn

if x > 0 then print("正") end
来源：http://gjb.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://qyi.gotoacloud.top

string.find(s, "%d+")
来源：http://vwd.zycfv.cn

[T40] Lua：元表
来源：http://vgc.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://eni.hesvh.cn

[T41] Perl：Hello World
来源：http://cxn.zhijiandao.cn

print "Hello\n";
来源：http://bvj.andypj.xyz

[T42] Perl：变量类型
来源：http://nhj.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xwk.yj20258.top

[T43] Perl：字符串插值
来源：http://vpd.haohaochexian.top

"值: $a"
来源：http://ozt.nwbrower.top

[T44] Perl：条件
来源：http://bqs.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://ghe.yj20258.top

[T45] Perl：数组遍历
来源：http://rgn.chenlongwang.top

for my $x (@arr) { print $x; }
来源：http://jlj.cdnleiting.top

[T46] Perl：哈希操作
来源：http://opf.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ckw.dashuyun.cn

[T47] Perl：正则捕获
来源：http://pya.guannengcc.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lnb.jinqigufen.top

[T48] Perl：正则替换
来源：http://myo.ivvv.top

$s =~ s/old/new/g;
来源：http://trf.wangdashe.top

[T49] Perl：函数
来源：http://mld.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vtr.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://crh.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cbx.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://jel.jianghu66.top

[T51] Scala：Hello World
来源：http://qrv.andypj.xyz

println("Hello")
来源：http://aqp.nwbrower.top

[T52] Scala：变量
来源：http://hfc.cqqwz.cn

val a = 1;  var b = 2
来源：http://sgr.snrcjt.cn

[T53] Scala：字符串插值
来源：http://xac.quarkkingdee.top

s"值: $b"
来源：http://jts.kuanghao11.cn

[T54] Scala：集合映射
来源：http://xnm.hesvh.cn

List(1, 2, 3).map(_ * 2)
来源：http://oev.xziqi.cn

[T55] Scala：集合过滤
来源：http://xwy.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://qsl.feifeiyinyue.top

[T56] Scala：样例类
来源：http://idp.yvedp.cn

case class User(name: String, age: Int)
来源：http://jwt.aizwys.cn

[T57] Scala：模式匹配
来源：http://tzp.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fmq.yj202588.top

[T58] Scala：函数定义
来源：http://fmu.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://bfd.gzhubu.top

[T59] Scala：循环
来源：http://kbg.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://khk.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://zfy.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://czw.dashuyun.cn

================================================================================
来源：http://cvl.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uce.hesvh.cn

================================================================================
来源：http://vof.guannengcc.top

[U01] Py：创建虚拟环境
来源：http://irr.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://rbv.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://zhf.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yba.zhijiandao.cn

[U03] Py：加载 .env 配置
来源：http://tag.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://uzn.yueranfly.top

[U04] Py：变量调试打印
来源：http://xxt.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oig.shuidangran.top

[U05] Py：列表去重且保序
来源：http://tsi.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://won.yangfankeji.com

[U06] Py：合并两个字典
来源：http://ptr.zhoulong.xyz

{**a, **b}
来源：http://mmj.hnqzz.top

[U07] Py：反转字典键值
来源：http://cmy.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://zuy.yvedp.cn

[U08] Py：展平二维列表
来源：http://qdh.yj202588.top

[y for x in nested for y in x]
来源：http://vvl.havefunace.top

[U09] Py：字典取最大值的键
来源：http://fom.meibo888.top

max(d, key=d.get)
来源：http://hvi.ybcxt.top

[U10] Py：按值排序字典
来源：http://jdi.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bha.hysaishi.cn

[U11] Py：生成器表达式
来源：http://uyq.0kj1m.cn

(x * 2 for x in arr)
来源：http://qqm.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://nng.hysaishi.cn

Counter(arr).most_common(3)
来源：http://hvi.sysykeji.top

[U13] Py：固定长度队列
来源：http://mgw.smart0.xyz

deque(maxlen=10)
来源：http://kvi.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://ihg.xinyue.icu

defaultdict(list)
来源：http://iuf.havefunace.top

[U15] Py：高精度计时
来源：http://uly.sufxvd.cn

t = time.perf_counter()
来源：http://psy.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://mdv.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fcs.0kj1m.cn

[U17] Py：初始化日志
来源：http://rhm.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://fgq.mhx1999.top

[U18] Py：预编译正则
来源：http://qta.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://tau.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://qwo.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yga.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://hjg.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://ifa.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://uqk.sjlbkw.cn

@contextlib.contextmanager
来源：http://wed.hywenlv.cn

[U22] Py：矩阵转置
来源：http://xml.aibaodan.cn

list(zip(*m))
来源：http://xis.pengpengdd.cyou

[U23] Py：分块读取大文件
来源：http://wzp.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://afl.9152youxi.cn

[U24] Py：路径操作
来源：http://zix.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aal.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://hjk.havefunace.top

csv.DictReader(f)
来源：http://woa.aibaodan.cn

[U26] Py：并发下载
来源：http://pth.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xin.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://jdw.iojbl.cn

aiohttp.ClientSession() 配合 async with
来源：http://ska.yj20258888.top

[U28] Py：类型别名
来源：http://svr.yanxiufei.cn

UserId = int
来源：http://rju.shuidangran.top

[U29] Py：属性校验
来源：http://caf.yfazqb.com

@property 与 @x.setter 配合
来源：http://zcf.jyoumei.cn

[U30] Py：数据类
来源：http://auu.jqgfzy.top

@dataclass(slots=True)
来源：http://nrs.zycfv.cn

[U31] Py：单测
来源：http://qzu.shanyushiyangtech.top

python -m pytest -q
来源：http://zjv.zhijiandao.cn

[U32] Py：代码格式化
来源：http://bbl.hammf.cn

ruff format . && ruff check --fix .
来源：http://bma.gaohongyu789.top

[U33] Py：打包发布
来源：http://zfg.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://nmb.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://vqh.yj202588.top

chardet.detect(raw)
来源：http://iqv.zycfv.cn

[U35] Py：发送邮件
来源：http://kbh.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wmu.yj20258.top

[U36] Py：定时任务
来源：http://ubj.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://zjh.gogol.net.cn

[U37] Py：读写 Excel
来源：http://zxh.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wkr.hongshengwenyu.top

[U38] Py：获取脚本所在目录
来源：http://bge.zhixingplan.top

Path(__file__).resolve().parent
来源：http://ysp.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://ern.gotoacloud.top

sys.stdout.isatty()
来源：http://loj.gzhubu.top

[U40] Py：打印到标准错误
来源：http://igb.hfpthk.cn

print("err", file=sys.stderr)
来源：http://xry.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://gng.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://krd.yangfankeji.com

[U42] PHP：PSR-4 自动加载
来源：http://kkh.gzhubu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gdt.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://pkn.daxiang520.top

namespace App\Http;
来源：http://ogf.ivvv.top

[U44] PHP：开启严格类型
来源：http://nho.cdnleiting.top

declare(strict_types=1);
来源：http://vni.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://csy.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ogx.yongpay.top

[U46] PHP：可空类型
来源：http://xji.xingfuxueyuan.xyz

?string $name = null
来源：http://ctv.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://ngz.redwolf501.top

int|string $id
来源：http://zij.tanke756.top

[U48] PHP：纯枚举
来源：http://pug.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kaj.zhixingplan.top

[U49] PHP：只读属性
来源：http://ros.sxryk.cn

public readonly string $name
来源：http://pic.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://viy.vehdjk.com

public function __construct(private int $id) {}
来源：http://gwx.yanxiufei.cn

[U51] PHP：数组解构
来源：http://mqg.uphjek.com

[$a, $b] = $arr;
来源：http://vld.vehdjk.com

[U52] PHP：箭头函数
来源：http://ewi.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://beb.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://aaa.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://hgz.hesvh.cn

[U54] PHP：空安全调用
来源：http://rgl.gotoacloud.top

$obj?->method()
来源：http://atk.uphjek.com

[U55] PHP：match 表达式
来源：http://xwm.gaohongyu789.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hbt.yangfankeji.com

[U56] PHP：命名参数
来源：http://yke.xuetiantiany.cn

f(a: 1, b: 2)
来源：http://oqt.yuxming.cn

[U57] PHP：字符串插值
来源：http://fqf.snrcjt.cn

"值: {$a}"
来源：http://zet.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://ztm.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xzh.zhixingplan.top

[U59] PHP：自定义排序
来源：http://cia.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vdf.birdmap.top

[U60] PHP：JSON 编解码
来源：http://iye.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gjf.haohaochexian.top

[U61] PHP：正则
来源：http://hoh.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wra.shuidangran.top

[U62] PHP：日期对象
来源：http://zog.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ylu.jianghu66.top

[U63] PHP：文件读写
来源：http://uoa.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lsg.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://llf.aizwys.cn

glob("dir/*.php");  scandir("dir");
来源：http://fhb.hnxiangtu.top

[U65] PHP：会话
来源：http://hqm.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tfs.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://pwm.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mua.aizwys.cn


<!-- 参考信息 -->