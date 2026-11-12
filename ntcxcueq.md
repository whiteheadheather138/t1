代发 wailian999

[S43] C++：智能指针
来源：http://nzn.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://isx.0kj1m.cn

[S44] C++：引用传参
来源：http://fmu.vehdjk.com

void inc(int &x) { ++x; }
来源：http://bpz.yangfankeji.com

[S45] C++：lambda
来源：http://fvp.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vxr.dianchejie.cn

[S46] C++：函数模板
来源：http://gym.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kru.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://vzy.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fsg.hnxiangtu.top

[S48] C++：逐行读文件
来源：http://dsj.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://lcd.sysykeji.top

while (std::getline(in, line)) { }
来源：http://enn.aibaodan.cn

[S49] C++：写文件
来源：http://fkb.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zvm.316326.xyz

[S50] C++：格式化数字
来源：http://dzp.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vgg.zdbjq.cn

[S51] C++：显式类型转换
来源：http://gom.tian-w.cn

static_cast<double>(a) / b
来源：http://wei.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://ksr.guannengcc.top

int size() const noexcept { return n_; }
来源：http://zoy.yj20258.top

[S53] C++：移动语义
来源：http://tew.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://kaz.vehdjk.com

[S54] C++：异常处理
来源：http://tqh.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://owh.yongpay.top

[S55] C++：结构化绑定
来源：http://sxe.daxiang520.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gui.zdqjudy.top

[S56] C++：optional
来源：http://ugq.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bgs.zhiwuduotai.top

[S57] C++：编译期常量
来源：http://sqg.cdnleiting.top

constexpr int N = 10;
来源：http://qlm.sxryk.cn

[S58] C++：命名空间
来源：http://pzm.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://nyv.jqgufenzy.top

[S59] C++：静态断言
来源：http://idk.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ead.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://grb.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yad.yuxming.cn

================================================================================
来源：http://cgc.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gpe.daria6918.cn

================================================================================
来源：http://zqk.9152youxi.cn

[T01] Kotlin：Hello World
来源：http://cxw.xuetiantiany.cn

println("Hello")
来源：http://lpj.zhijiandao.cn

[T02] Kotlin：变量
来源：http://vir.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nct.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://fuz.haohaochexian.top

"值: $b"
来源：http://pdu.havefunace.top

[T04] Kotlin：空安全
来源：http://yaq.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://amb.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://hjo.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sna.xziqi.cn

[T06] Kotlin：集合映射
来源：http://xbb.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cji.pycfn.com

[T07] Kotlin：集合过滤
来源：http://muy.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wsn.yj20258888.top

[T08] Kotlin：数据类
来源：http://rtn.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://tlm.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://uom.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://kiv.hesvh.cn

[T10] Kotlin：默认参数
来源：http://lxx.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rkk.cucudq.cn

[T11] Kotlin：协程
来源：http://jww.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ens.sysykeji.top

[T12] Kotlin：解构声明
来源：http://ndp.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://xpy.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://dqh.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://hrg.zhongyouzk.top

[T14] Kotlin：循环
来源：http://hfa.aibaodan.cn

for (i in 1..10) println(i)
来源：http://bzg.daxiang520.top

[T15] Kotlin：接口
来源：http://acl.guannengcc.top

interface Shape { fun area(): Double }
来源：http://qov.sweek.top

[T16] Swift：Hello World
来源：http://xwn.gotoacloud.top

print("Hello")
来源：http://zsb.yj20258.top

[T17] Swift：变量与常量
来源：http://laf.vqdsnc.cn

var a = 1;  let b = 2
来源：http://cmw.yj20258.top

[T18] Swift：字符串插值
来源：http://lvp.hnqzz.top

"值: \(b)"
来源：http://nud.xziqi.cn

[T19] Swift：可选绑定
来源：http://dfz.haohaochexian.top

if let n = opt { print(n) }
来源：http://sjk.fehbvm.com

[T20] Swift：数组操作
来源：http://cea.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pjy.dashuyun.cn

[T21] Swift：遍历
来源：http://chc.52xcode.cn

for x in a { print(x) }
来源：http://bpj.dashuyun.cn

[T22] Swift：字典
来源：http://lvz.fengsongda.top

var d = ["a": 1];  d["b"] = 2
来源：http://jdh.havefunace.top

[T23] Swift：函数
来源：http://iho.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wnh.52xcode.cn

[T24] Swift：闭包
来源：http://ruz.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sot.hnqzz.top

[T25] Swift：结构体
来源：http://hjy.cucudq.cn

struct P { var x: Int }
来源：http://bod.smart0.xyz

[T26] Swift：类与重写
来源：http://uty.tianlin.xyz

class A: Base { override func f() {} }
来源：http://lov.ehwqpu.com

[T27] Swift：错误处理
来源：http://oqk.yj202588.top

do { try f() } catch { print(error) }
来源：http://rbv.wangshuangyany.cn

[T28] Swift：枚举
来源：http://wye.jqgfzy.top

enum Color { case red, green }
来源：http://kzm.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://ufj.nanxuanxn.top

guard let x = opt else { return }
来源：http://mzl.smart0.xyz

[T30] Swift：协议
来源：http://aeo.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://tpd.ctjpmb.com

[T31] Lua：Hello World
来源：http://xuo.dianchejie.cn

print("Hello")
来源：http://apc.andypj.xyz

[T32] Lua：局部变量
来源：http://hqd.zdbjq.cn

local a = 1
来源：http://qad.havefunace.top

[T33] Lua：表（数组）
来源：http://orl.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cnr.fzhhl.top

[T34] Lua：遍历表
来源：http://lvd.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kiv.sweek.top

[T35] Lua：字典表
来源：http://pjk.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://dtl.ctjpmb.com

[T36] Lua：函数
来源：http://myd.yvedp.cn

function add(a, b) return a + b end
来源：http://rbu.sxryk.cn

[T37] Lua：字符串拼接
来源：http://zrt.shanyushiyangtech.top

"a" .. "b"
来源：http://kmo.kuanghao11.cn

[T38] Lua：条件
来源：http://kjf.hnqzz.top

if x > 0 then print("正") end
来源：http://tcl.pycfn.com

[T39] Lua：模式匹配
来源：http://uod.daria6918.cn

string.find(s, "%d+")
来源：http://tqa.yongpay.top

[T40] Lua：元表
来源：http://may.cheryme.top

setmetatable({}, { __index = base })
来源：http://prk.hfpthk.cn

[T41] Perl：Hello World
来源：http://nna.hywenlv.cn

print "Hello\n";
来源：http://vbm.ybcxt.top

[T42] Perl：变量类型
来源：http://gjq.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://htw.chenlongwang.top

[T43] Perl：字符串插值
来源：http://edj.yueranfly.top

"值: $a"
来源：http://tgf.guannengcc.top

[T44] Perl：条件
来源：http://yav.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://koz.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://bzo.xuetiantiany.cn

for my $x (@arr) { print $x; }
来源：http://kpd.daxiang520.top

[T46] Perl：哈希操作
来源：http://ikv.jiagoushi.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yjt.gzhubu.top

[T47] Perl：正则捕获
来源：http://ipb.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qts.yangfankeji.com

[T48] Perl：正则替换
来源：http://ngy.meibo888.top

$s =~ s/old/new/g;
来源：http://onf.yuanzhike.top

[T49] Perl：函数
来源：http://ezs.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eui.smart0.xyz

[T50] Perl：逐行读文件
来源：http://djb.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gcc.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://eym.daria6918.cn

[T51] Scala：Hello World
来源：http://obm.ppjwa.cn

println("Hello")
来源：http://wqs.yj202588.top

[T52] Scala：变量
来源：http://hgv.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://oan.aizwys.cn

[T53] Scala：字符串插值
来源：http://odx.jinqigfzy.top

s"值: $b"
来源：http://qmp.jiagoushi.top

[T54] Scala：集合映射
来源：http://oxj.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://mvu.daria6918.cn

[T55] Scala：集合过滤
来源：http://vgp.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://yug.iojbl.cn

[T56] Scala：样例类
来源：http://xmh.haohaochexian.top

case class User(name: String, age: Int)
来源：http://qyj.yj202588.top

[T57] Scala：模式匹配
来源：http://zec.tianlin.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://jck.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://srw.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://prl.nanxuanxn.top

[T59] Scala：循环
来源：http://gzi.gaohongyu789.top

for (i <- 1 to 10) println(i)
来源：http://rug.sxryk.cn

[T60] Scala：折叠
来源：http://ifz.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lat.hywenlv.cn

================================================================================
来源：http://gcz.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qiy.cdnleiting.top

================================================================================
来源：http://tpe.xuanzx.com

[U01] Py：创建虚拟环境
来源：http://prv.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vxz.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://lfw.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mln.tanke756.top

[U03] Py：加载 .env 配置
来源：http://wnf.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kwc.fzhhl.top

[U04] Py：变量调试打印
来源：http://fal.yongpay.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bbg.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://noo.aizwys.cn

list(dict.fromkeys(arr))
来源：http://mak.zhixingplan.top

[U06] Py：合并两个字典
来源：http://khi.fanxiaobao.xyz

{**a, **b}
来源：http://qag.zhengqikj.top

[U07] Py：反转字典键值
来源：http://pcx.gzhubu.top

{v: k for k, v in d.items()}
来源：http://kej.feifeiyinyue.top

[U08] Py：展平二维列表
来源：http://kwp.jqgufenzy.top

[y for x in nested for y in x]
来源：http://wlc.ydzc1.top

[U09] Py：字典取最大值的键
来源：http://xzr.jianghu66.top

max(d, key=d.get)
来源：http://jyd.yangfankeji.com

[U10] Py：按值排序字典
来源：http://vku.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wlq.yvedp.cn

[U11] Py：生成器表达式
来源：http://srp.nanxinkj.top

(x * 2 for x in arr)
来源：http://qqu.ydzc1.top

[U12] Py：取出现最多的 3 个元素
来源：http://ucd.zdbjq.cn

Counter(arr).most_common(3)
来源：http://emw.yj20258.top

[U13] Py：固定长度队列
来源：http://ggh.redwolf501.top

deque(maxlen=10)
来源：http://gxo.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://tlf.kuanghao11.cn

defaultdict(list)
来源：http://pdh.wangdashe.top

[U15] Py：高精度计时
来源：http://rfl.zhiwuduotai.top

t = time.perf_counter()
来源：http://cky.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://eqd.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mkb.meibo888.top

[U17] Py：初始化日志
来源：http://stl.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://yti.yj20258888.top

[U18] Py：预编译正则
来源：http://ucu.aibaodan.cn

pat = re.compile(r"\d+")
来源：http://tsb.daria6918.cn

[U19] Py：正则替换带回调
来源：http://anv.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ats.yvedp.cn

[U20] Py：缓存函数结果
来源：http://svq.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://kiz.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://cgh.pengpengdd.cyou

@contextlib.contextmanager
来源：http://bik.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://mlr.hnxiangtu.top

list(zip(*m))
来源：http://dmo.zdqjudy.top

[U23] Py：分块读取大文件
来源：http://uwx.guannengcc.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ynn.316326.xyz

[U24] Py：路径操作
来源：http://mnz.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://onb.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://sgm.vqdsnc.cn

csv.DictReader(f)
来源：http://zuv.ybcxt.top

[U26] Py：并发下载
来源：http://oca.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kgr.zycfv.cn

[U27] Py：异步 HTTP
来源：http://ogu.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://rnm.jyoumei.cn

[U28] Py：类型别名
来源：http://esq.yangfankeji.com

UserId = int
来源：http://urt.nanxuanxn.top

[U29] Py：属性校验
来源：http://upf.xylfe.cn

@property 与 @x.setter 配合
来源：http://fda.redwolf501.top

[U30] Py：数据类
来源：http://jro.gotoacloud.top

@dataclass(slots=True)
来源：http://ffs.316326.xyz

[U31] Py：单测
来源：http://rdi.yuxming.cn

python -m pytest -q
来源：http://xjx.c1oappe.top

[U32] Py：代码格式化
来源：http://ytx.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://vjd.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://jst.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://lwh.tanke756.top

[U34] Py：判断编码
来源：http://clz.pengpengdd.cyou

chardet.detect(raw)
来源：http://ywa.zhijiandao.cn

[U35] Py：发送邮件
来源：http://kfa.snrcjt.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kia.yuxming.cn

[U36] Py：定时任务
来源：http://jkk.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://hmv.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://wsj.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uep.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://jza.feifeiyinyue.top

Path(__file__).resolve().parent
来源：http://crp.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://tiy.0kj1m.cn

sys.stdout.isatty()
来源：http://glx.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://gio.dianchejie.cn

print("err", file=sys.stderr)
来源：http://dzz.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://yeq.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xkx.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://gev.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kqb.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://inq.aibaodan.cn

namespace App\Http;
来源：http://dlu.tanke756.top

[U44] PHP：开启严格类型
来源：http://cud.jyoumei.cn

declare(strict_types=1);
来源：http://fny.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://sul.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://cvq.jqgfzy.top

[U46] PHP：可空类型
来源：http://ptr.feifeiyinyue.top

?string $name = null
来源：http://xyl.gaohongyu789.top

[U47] PHP：联合类型
来源：http://rza.wangdashe.top

int|string $id
来源：http://oti.zdbjq.cn

[U48] PHP：纯枚举
来源：http://yyz.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lkh.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://lvh.hcnkem.com

public readonly string $name
来源：http://cwq.hywenlv.cn

[U50] PHP：构造器属性提升
来源：http://vyh.tianlin.xyz

public function __construct(private int $id) {}
来源：http://cxp.uphjek.com

[U51] PHP：数组解构
来源：http://vud.yj20258.top

[$a, $b] = $arr;
来源：http://irk.cucudq.cn

[U52] PHP：箭头函数
来源：http://slx.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://ulp.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://ukg.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://gtp.wangdashe.top

[U54] PHP：空安全调用
来源：http://cyn.ydjk.org.cn

$obj?->method()
来源：http://dxu.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://vkr.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eri.fktsv.cn

[U56] PHP：命名参数
来源：http://bak.hnxiangtu.top

f(a: 1, b: 2)
来源：http://nfc.iojbl.cn

[U57] PHP：字符串插值
来源：http://wmh.snrcjt.cn

"值: {$a}"
来源：http://uhj.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://gfg.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ttw.hfpthk.cn

[U59] PHP：自定义排序
来源：http://quf.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dzo.zhijiandao.cn

[U60] PHP：JSON 编解码
来源：http://qgx.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://suf.zhixingplan.top

[U61] PHP：正则
来源：http://myi.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tmy.havefunace.top

[U62] PHP：日期对象
来源：http://efg.hesvh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ihf.nanxinkj.top

[U63] PHP：文件读写
来源：http://vig.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://box.ybcxt.top

[U64] PHP：目录遍历
来源：http://ywj.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://qwr.chenlongwang.top

[U65] PHP：会话
来源：http://vee.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://uxc.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://wom.zhijiandao.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://skn.yanxiufei.cn

[U67] PHP：处理文件上传
来源：http://rxh.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://way.xinyue.icu

[U68] PHP：PDO 连接
来源：http://jkr.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wwk.tianlin.xyz


<!-- 参考信息 -->