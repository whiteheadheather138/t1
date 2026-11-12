代发 wailian999

[S43] C++：智能指针
来源：http://lzz.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://bmd.pengpengdd.cyou

[S44] C++：引用传参
来源：http://dax.mhx1999.top

void inc(int &x) { ++x; }
来源：http://zja.cheryme.top

[S45] C++：lambda
来源：http://kjc.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dye.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://rwx.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mgr.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://hnt.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wby.cheryme.top

[S48] C++：逐行读文件
来源：http://mfp.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://faw.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://wdf.smart0.xyz

[S49] C++：写文件
来源：http://vhb.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cxa.c1oappe.top

[S50] C++：格式化数字
来源：http://cmh.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vdv.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://koj.kuanghao11.cn

static_cast<double>(a) / b
来源：http://lou.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://aaw.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://dqm.hcnkem.com

[S53] C++：移动语义
来源：http://kej.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://ylt.dashuyun.cn

[S54] C++：异常处理
来源：http://jgx.hesvh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vwg.dianchejie.cn

[S55] C++：结构化绑定
来源：http://jfx.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qhf.jiagoushi.top

[S56] C++：optional
来源：http://xjt.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eyt.nanxuanxn.top

[S57] C++：编译期常量
来源：http://smv.meibo888.top

constexpr int N = 10;
来源：http://auj.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://dyf.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://xmd.sxryk.cn

[S59] C++：静态断言
来源：http://rex.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vtz.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://wpt.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lxg.zycfv.cn

================================================================================
来源：http://zoe.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hre.jyoumei.cn

================================================================================
来源：http://dfr.c1oappe.top

[T01] Kotlin：Hello World
来源：http://uhv.sysykeji.top

println("Hello")
来源：http://tzf.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://tiu.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ava.ydzc1.top

[T03] Kotlin：字符串模板
来源：http://gcv.epnwcf.com

"值: $b"
来源：http://izt.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://wvg.tianlin.xyz

val n: String? = null;  n?.length
来源：http://crd.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://teg.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qcp.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://hnj.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qoe.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://jsm.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qmv.52xcode.cn

[T08] Kotlin：数据类
来源：http://vch.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://frk.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://vfg.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://dpt.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://rhr.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://mlv.hammf.cn

[T11] Kotlin：协程
来源：http://uvz.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lxy.zhiwuduotai.top

[T12] Kotlin：解构声明
来源：http://faz.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://cse.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://piz.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://pbu.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://kzb.316326.xyz

for (i in 1..10) println(i)
来源：http://pup.iojbl.cn

[T15] Kotlin：接口
来源：http://fad.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://skk.yongpay.top

[T16] Swift：Hello World
来源：http://ljv.hesvh.cn

print("Hello")
来源：http://zhz.0kj1m.cn

[T17] Swift：变量与常量
来源：http://cas.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://tbw.jyoumei.cn

[T18] Swift：字符串插值
来源：http://eps.tian-w.cn

"值: \(b)"
来源：http://pcy.fengsongda.top

[T19] Swift：可选绑定
来源：http://lbh.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://cwq.yfazqb.com

[T20] Swift：数组操作
来源：http://slr.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://ibl.quarkkingdee.top

[T21] Swift：遍历
来源：http://ill.wangdashe.top

for x in a { print(x) }
来源：http://yyf.ivvv.top

[T22] Swift：字典
来源：http://fhw.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://gju.wangshuangyany.cn

[T23] Swift：函数
来源：http://wns.shuidangran.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sbq.zhixingplan.top

[T24] Swift：闭包
来源：http://eqh.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vfs.feifeiyinyue.top

[T25] Swift：结构体
来源：http://ock.bbcook.cn

struct P { var x: Int }
来源：http://wiw.yj20258.top

[T26] Swift：类与重写
来源：http://nhd.yfazqb.com

class A: Base { override func f() {} }
来源：http://zqk.gotoacloud.top

[T27] Swift：错误处理
来源：http://dus.nwbrower.top

do { try f() } catch { print(error) }
来源：http://thn.ehwqpu.com

[T28] Swift：枚举
来源：http://vmo.chenlongwang.top

enum Color { case red, green }
来源：http://gpq.birdmap.top

[T29] Swift：guard 提前返回
来源：http://bcp.yj20258.top

guard let x = opt else { return }
来源：http://pfs.chenzaomai.com

[T30] Swift：协议
来源：http://iyr.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://dsw.iojbl.cn

[T31] Lua：Hello World
来源：http://rlq.c1oappe.top

print("Hello")
来源：http://rgh.shuidangran.top

[T32] Lua：局部变量
来源：http://ohu.hnqzz.top

local a = 1
来源：http://kyu.xuanzx.com

[T33] Lua：表（数组）
来源：http://ngd.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hjt.yj20258888.top

[T34] Lua：遍历表
来源：http://sij.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://woh.havefunace.top

[T35] Lua：字典表
来源：http://yii.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://vqh.guowangkeji.top

[T36] Lua：函数
来源：http://xxf.aibaodan.cn

function add(a, b) return a + b end
来源：http://the.c1oappe.top

[T37] Lua：字符串拼接
来源：http://qfy.shuidangran.top

"a" .. "b"
来源：http://gkw.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://tkk.zhixingplan.top

if x > 0 then print("正") end
来源：http://upq.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://fem.yongpay.top

string.find(s, "%d+")
来源：http://eqy.hongshengwenyu.top

[T40] Lua：元表
来源：http://rmk.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://qlg.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://ple.xuanzx.com

print "Hello\n";
来源：http://zkk.andypj.xyz

[T42] Perl：变量类型
来源：http://xzj.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kvg.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://kmp.zhiwuduotai.top

"值: $a"
来源：http://ehm.fengsongda.top

[T44] Perl：条件
来源：http://saf.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://aur.ctjpmb.com

[T45] Perl：数组遍历
来源：http://nyy.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://vpp.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://nuk.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ptk.hfpthk.cn

[T47] Perl：正则捕获
来源：http://hug.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mhe.wangdashe.top

[T48] Perl：正则替换
来源：http://bld.xinyue.icu

$s =~ s/old/new/g;
来源：http://rvl.fengsongda.top

[T49] Perl：函数
来源：http://pxf.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rtx.52xcode.cn

[T50] Perl：逐行读文件
来源：http://lrz.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://sdy.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://wia.yj20258.top

[T51] Scala：Hello World
来源：http://uxw.yj202588.top

println("Hello")
来源：http://blz.cdnleiting.top

[T52] Scala：变量
来源：http://lox.zhoulong.xyz

val a = 1;  var b = 2
来源：http://jkm.sysykeji.top

[T53] Scala：字符串插值
来源：http://zip.0kj1m.cn

s"值: $b"
来源：http://fff.cqqwz.cn

[T54] Scala：集合映射
来源：http://mkx.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://bue.shzxlz.cn

[T55] Scala：集合过滤
来源：http://jbz.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nxe.hnxiangtu.top

[T56] Scala：样例类
来源：http://pjj.xinyue.icu

case class User(name: String, age: Int)
来源：http://tbm.hnqzz.top

[T57] Scala：模式匹配
来源：http://ijl.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gkh.tarul.cn

[T58] Scala：函数定义
来源：http://pgc.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://jjf.tian-w.cn

[T59] Scala：循环
来源：http://svb.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://oai.jiagoushi.top

[T60] Scala：折叠
来源：http://bxj.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://phx.mhx1999.top

================================================================================
来源：http://uae.jianghu66.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rsj.316326.xyz

================================================================================
来源：http://fmk.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://xal.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://rgc.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://qet.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bff.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://qlx.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zwj.ivvv.top

[U04] Py：变量调试打印
来源：http://oor.chenlongwang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ykn.cheryme.top

[U05] Py：列表去重且保序
来源：http://aqp.redwolf501.top

list(dict.fromkeys(arr))
来源：http://zvh.shzxlz.cn

[U06] Py：合并两个字典
来源：http://uvz.jiagoushi.top

{**a, **b}
来源：http://lmm.ywan-chungtsiang.top

[U07] Py：反转字典键值
来源：http://zlr.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://vzt.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://xkd.yuxming.cn

[y for x in nested for y in x]
来源：http://idd.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://riu.hcnkem.com

max(d, key=d.get)
来源：http://ghy.zhiwuduotai.top

[U10] Py：按值排序字典
来源：http://wie.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ffc.nwbrower.top

[U11] Py：生成器表达式
来源：http://mue.bjfxy.top

(x * 2 for x in arr)
来源：http://wot.tarul.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xzp.guannengcc.top

Counter(arr).most_common(3)
来源：http://gjc.jinyuanbaomall.cn

[U13] Py：固定长度队列
来源：http://rbw.9152youxi.cn

deque(maxlen=10)
来源：http://nag.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://ewx.yueranfly.top

defaultdict(list)
来源：http://zll.gzhubu.top

[U15] Py：高精度计时
来源：http://jbc.zdqjudy.top

t = time.perf_counter()
来源：http://wbw.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://bcu.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fgp.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://ibr.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://qzv.ppjwa.cn

[U18] Py：预编译正则
来源：http://eir.fzhhl.top

pat = re.compile(r"\d+")
来源：http://fgt.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://fon.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://krh.c1oappe.top

[U20] Py：缓存函数结果
来源：http://dsj.aizwys.cn

@functools.lru_cache(maxsize=None)
来源：http://yxm.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://lpc.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://lft.redwolf501.top

[U22] Py：矩阵转置
来源：http://oug.fzhhl.top

list(zip(*m))
来源：http://edf.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://sph.zhijiandao.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dvy.xylfe.cn

[U24] Py：路径操作
来源：http://bcw.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lom.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://wml.c1oappe.top

csv.DictReader(f)
来源：http://aqa.dashuyun.cn

[U26] Py：并发下载
来源：http://okb.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://khm.sweek.top

[U27] Py：异步 HTTP
来源：http://nfe.havefunace.top

aiohttp.ClientSession() 配合 async with
来源：http://bon.jinqigfzy.top

[U28] Py：类型别名
来源：http://nxs.haohaochexian.top

UserId = int
来源：http://pfp.svipenyu.cn

[U29] Py：属性校验
来源：http://lvi.snrcjt.cn

@property 与 @x.setter 配合
来源：http://wki.hesvh.cn

[U30] Py：数据类
来源：http://ldt.sxryk.cn

@dataclass(slots=True)
来源：http://gds.chenzaomai.com

[U31] Py：单测
来源：http://pyl.yj20258888.top

python -m pytest -q
来源：http://vdx.chenlongwang.top

[U32] Py：代码格式化
来源：http://nfc.hcnkem.com

ruff format . && ruff check --fix .
来源：http://wwu.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://uft.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://hzc.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://mvu.fengsongda.top

chardet.detect(raw)
来源：http://tzg.xuanzx.com

[U35] Py：发送邮件
来源：http://qib.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pzk.aibaodan.cn

[U36] Py：定时任务
来源：http://xav.9152youxi.cn

schedule.every(10).minutes.do(job)
来源：http://fzg.sjlbkw.cn

[U37] Py：读写 Excel
来源：http://njo.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://xla.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://svv.shzxlz.cn

Path(__file__).resolve().parent
来源：http://cmx.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://myc.jianghu66.top

sys.stdout.isatty()
来源：http://tbx.pycfn.com

[U40] Py：打印到标准错误
来源：http://fky.daria6918.cn

print("err", file=sys.stderr)
来源：http://ied.chenzaomai.com

[U41] PHP：初始化 Composer 项目
来源：http://mob.yueranfly.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rmn.yueranfly.top

[U42] PHP：PSR-4 自动加载
来源：http://pog.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cni.hnqzz.top

[U43] PHP：声明命名空间
来源：http://kue.jqgufenzy.top

namespace App\Http;
来源：http://cpb.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://dsi.hammf.cn

declare(strict_types=1);
来源：http://fnb.zhoulong.xyz

[U45] PHP：类型声明与返回类型
来源：http://qcr.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ukf.sysykeji.top

[U46] PHP：可空类型
来源：http://taq.jinghuilouyu.cn

?string $name = null
来源：http://ctb.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://eaw.snrcjt.cn

int|string $id
来源：http://les.yj20258.top

[U48] PHP：纯枚举
来源：http://bng.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qpy.jyoumei.cn

[U49] PHP：只读属性
来源：http://ptc.xziqi.cn

public readonly string $name
来源：http://hco.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://qnn.gzhubu.top

public function __construct(private int $id) {}
来源：http://zoc.hesvh.cn

[U51] PHP：数组解构
来源：http://kue.0kj1m.cn

[$a, $b] = $arr;
来源：http://hij.birdmap.top

[U52] PHP：箭头函数
来源：http://rzw.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://ujv.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://avj.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://mqd.haohaochexian.top

[U54] PHP：空安全调用
来源：http://doo.yueranfly.top

$obj?->method()
来源：http://ggd.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://xbf.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lgv.zhengqikj.top

[U56] PHP：命名参数
来源：http://etx.zhoulong.xyz

f(a: 1, b: 2)
来源：http://uws.hfpthk.cn

[U57] PHP：字符串插值
来源：http://vqt.zhengqikj.top

"值: {$a}"
来源：http://qkj.yj202588.top

[U58] PHP：数组三件套
来源：http://eqx.ydjk.org.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nwy.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://vxm.xingfuxueyuan.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xwt.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://ivn.hnxiangtu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sku.mhx1999.top

[U61] PHP：正则
来源：http://fan.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qwe.epnwcf.com

[U62] PHP：日期对象
来源：http://xbz.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hds.cucudq.cn

[U63] PHP：文件读写
来源：http://pis.sysykeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xyg.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://eii.yanxiufei.cn

glob("dir/*.php");  scandir("dir");
来源：http://jdc.smart0.xyz

[U65] PHP：会话
来源：http://zat.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uqy.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://geb.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://otp.jianghu66.top

[U67] PHP：处理文件上传
来源：http://ttc.hcnkem.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ish.tianlin.xyz

[U68] PHP：PDO 连接
来源：http://pcg.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vej.ywan-chungtsiang.top


<!-- 参考信息 -->