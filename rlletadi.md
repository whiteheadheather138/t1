代发 wailian999

[S43] C++：智能指针
来源：http://bpc.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://hsn.daxiang520.top

[S44] C++：引用传参
来源：http://iyj.316326.xyz

void inc(int &x) { ++x; }
来源：http://pgj.vehdjk.com

[S45] C++：lambda
来源：http://agu.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://bms.bjfxy.top

[S46] C++：函数模板
来源：http://zwj.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://usi.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://qpf.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mqk.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://ljl.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://jod.iojbl.cn

while (std::getline(in, line)) { }
来源：http://ckc.jqgufenzy.top

[S49] C++：写文件
来源：http://zot.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://efk.birdmap.top

[S50] C++：格式化数字
来源：http://gzr.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rxc.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://gqx.zdbjq.cn

static_cast<double>(a) / b
来源：http://uhw.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://ttw.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://oiq.iojbl.cn

[S53] C++：移动语义
来源：http://vyz.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://gus.ydzc1.top

[S54] C++：异常处理
来源：http://ybu.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://psd.bbcook.cn

[S55] C++：结构化绑定
来源：http://rnb.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cjz.ehwqpu.com

[S56] C++：optional
来源：http://mbq.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hmo.yongpay.top

[S57] C++：编译期常量
来源：http://nfc.ppjwa.cn

constexpr int N = 10;
来源：http://dhy.daxiang520.top

[S58] C++：命名空间
来源：http://urq.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://trz.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://teh.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tqm.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://nuz.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hyr.dashuyun.cn

================================================================================
来源：http://onv.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sxn.ppjwa.cn

================================================================================
来源：http://hto.yonumen.top

[T01] Kotlin：Hello World
来源：http://kdt.xingfuxueyuan.xyz

println("Hello")
来源：http://uli.jlsjyb.cn

[T02] Kotlin：变量
来源：http://ptr.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rgk.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://clr.nwbrower.top

"值: $b"
来源：http://emu.jqgfzy.top

[T04] Kotlin：空安全
来源：http://pnm.wangdashe.top

val n: String? = null;  n?.length
来源：http://pob.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://wra.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dsv.hcnkem.com

[T06] Kotlin：集合映射
来源：http://sga.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fsy.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://mqs.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://edc.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://etr.havefunace.top

data class User(val name: String, val age: Int)
来源：http://wco.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://kur.316326.xyz

fun String.exclaim() = this + "!"
来源：http://ccw.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://mzy.epnwcf.com

fun greet(name: String = "World") = "Hi $name"
来源：http://stm.nanxinkj.top

[T11] Kotlin：协程
来源：http://gsz.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://giq.gaohongyu789.top

[T12] Kotlin：解构声明
来源：http://nnc.jinyuanbaomall.cn

val (a, b) = Pair(1, 2)
来源：http://gqf.zhaomingkeji.xyz

[T13] Kotlin：只读 Map
来源：http://fjg.sweek.top

val m = mapOf("a" to 1)
来源：http://zmj.tanke756.top

[T14] Kotlin：循环
来源：http://xfv.ppjwa.cn

for (i in 1..10) println(i)
来源：http://pyu.yuanzhike.top

[T15] Kotlin：接口
来源：http://rap.tian-w.cn

interface Shape { fun area(): Double }
来源：http://ayo.pycfn.com

[T16] Swift：Hello World
来源：http://kgu.wangdashe.top

print("Hello")
来源：http://ala.hnxiangtu.top

[T17] Swift：变量与常量
来源：http://kzo.kuanghao11.cn

var a = 1;  let b = 2
来源：http://khw.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://wsx.yueranfly.top

"值: \(b)"
来源：http://nuq.guowangkeji.top

[T19] Swift：可选绑定
来源：http://oqo.hywenlv.cn

if let n = opt { print(n) }
来源：http://oca.wangdashe.top

[T20] Swift：数组操作
来源：http://fpo.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://euw.xziqi.cn

[T21] Swift：遍历
来源：http://wuq.jianghu66.top

for x in a { print(x) }
来源：http://nnv.dashuyun.cn

[T22] Swift：字典
来源：http://sjw.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://qbn.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://zrv.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vnu.jinqigfzy.top

[T24] Swift：闭包
来源：http://xel.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oso.316326.xyz

[T25] Swift：结构体
来源：http://nsd.yfazqb.com

struct P { var x: Int }
来源：http://ucy.svipenyu.cn

[T26] Swift：类与重写
来源：http://qdc.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://tto.jianghu66.top

[T27] Swift：错误处理
来源：http://ssq.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://edm.yuanzhike.top

[T28] Swift：枚举
来源：http://erp.ehwqpu.com

enum Color { case red, green }
来源：http://pcq.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://ozh.quarkkingdee.top

guard let x = opt else { return }
来源：http://dkq.shuidangran.top

[T30] Swift：协议
来源：http://eni.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://ttx.nwbrower.top

[T31] Lua：Hello World
来源：http://nku.yueranfly.top

print("Hello")
来源：http://nyi.dianchejie.cn

[T32] Lua：局部变量
来源：http://yzm.smart0.xyz

local a = 1
来源：http://jfi.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://lte.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://koo.chenzaomai.com

[T34] Lua：遍历表
来源：http://cnd.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://emd.xziqi.cn

[T35] Lua：字典表
来源：http://hrz.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://zqm.ydjk.org.cn

[T36] Lua：函数
来源：http://ptc.yfazqb.com

function add(a, b) return a + b end
来源：http://ztg.yj20258888.top

[T37] Lua：字符串拼接
来源：http://ksu.c1oappe.top

"a" .. "b"
来源：http://bwc.redwolf501.top

[T38] Lua：条件
来源：http://xhe.haohaochexian.top

if x > 0 then print("正") end
来源：http://cvk.guowangkeji.top

[T39] Lua：模式匹配
来源：http://aym.zhengqikj.top

string.find(s, "%d+")
来源：http://ggr.xuanzx.com

[T40] Lua：元表
来源：http://lgm.yj202588.top

setmetatable({}, { __index = base })
来源：http://eez.cucudq.cn

[T41] Perl：Hello World
来源：http://rbm.yangfankeji.com

print "Hello\n";
来源：http://kyv.pycfn.com

[T42] Perl：变量类型
来源：http://qpg.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://its.fengsongda.top

[T43] Perl：字符串插值
来源：http://vbu.chenzaomai.com

"值: $a"
来源：http://rtp.andypj.xyz

[T44] Perl：条件
来源：http://ejd.snrcjt.cn

if ($a > 0) { print "正"; }
来源：http://cxy.chenlongwang.top

[T45] Perl：数组遍历
来源：http://wmr.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://vdc.zdqjudy.top

[T46] Perl：哈希操作
来源：http://qyp.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uyg.aizwys.cn

[T47] Perl：正则捕获
来源：http://wle.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://fmx.sweek.top

[T48] Perl：正则替换
来源：http://dtx.sweek.top

$s =~ s/old/new/g;
来源：http://ksg.fanxiaobao.xyz

[T49] Perl：函数
来源：http://amt.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ltw.meibo888.top

[T50] Perl：逐行读文件
来源：http://ueq.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ygf.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://hel.xinyue.icu

[T51] Scala：Hello World
来源：http://nnd.epnwcf.com

println("Hello")
来源：http://syd.fehbvm.com

[T52] Scala：变量
来源：http://bdw.zycfv.cn

val a = 1;  var b = 2
来源：http://pwn.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://slk.52xcode.cn

s"值: $b"
来源：http://xvs.jianghu66.top

[T54] Scala：集合映射
来源：http://ogo.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://dab.epnwcf.com

[T55] Scala：集合过滤
来源：http://ptk.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wse.yj202588.top

[T56] Scala：样例类
来源：http://wyc.hesvh.cn

case class User(name: String, age: Int)
来源：http://dvf.hcnkem.com

[T57] Scala：模式匹配
来源：http://wmj.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vmj.yonumen.top

[T58] Scala：函数定义
来源：http://fvk.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://rkn.vqdsnc.cn

[T59] Scala：循环
来源：http://cpu.316326.xyz

for (i <- 1 to 10) println(i)
来源：http://htj.jinqigfzy.top

[T60] Scala：折叠
来源：http://zwm.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xio.zhaomingkeji.xyz

================================================================================
来源：http://ktq.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://szx.chenzaomai.com

================================================================================
来源：http://qqc.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://blm.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qxf.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://xoc.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ycn.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://fug.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xlh.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://roo.316326.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zld.yj202588.top

[U05] Py：列表去重且保序
来源：http://kxf.jlsjyb.cn

list(dict.fromkeys(arr))
来源：http://szr.daria6918.cn

[U06] Py：合并两个字典
来源：http://uln.yj20258888.top

{**a, **b}
来源：http://pmh.tarul.cn

[U07] Py：反转字典键值
来源：http://vfa.fktsv.cn

{v: k for k, v in d.items()}
来源：http://msg.gogol.net.cn

[U08] Py：展平二维列表
来源：http://qes.aibaodan.cn

[y for x in nested for y in x]
来源：http://ibx.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://mqz.fehbvm.com

max(d, key=d.get)
来源：http://xvp.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://fqv.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ghi.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://nbm.jinqigfzy.top

(x * 2 for x in arr)
来源：http://nha.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://gik.haohaochexian.top

Counter(arr).most_common(3)
来源：http://lpn.epnwcf.com

[U13] Py：固定长度队列
来源：http://ppu.fehbvm.com

deque(maxlen=10)
来源：http://xpv.smart0.xyz

[U14] Py：分组收集到列表
来源：http://qqx.gogol.net.cn

defaultdict(list)
来源：http://wsz.gogol.net.cn

[U15] Py：高精度计时
来源：http://qhe.jinqigufen.top

t = time.perf_counter()
来源：http://zci.xuanzx.com

[U16] Py：命令行参数解析
来源：http://bih.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://num.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://oiy.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://zav.yj20258888.top

[U18] Py：预编译正则
来源：http://fuh.xinyue.icu

pat = re.compile(r"\d+")
来源：http://gxh.sxryk.cn

[U19] Py：正则替换带回调
来源：http://bwz.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tiq.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://tfe.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://rgl.ctjpmb.com

[U21] Py：自定义上下文管理器
来源：http://ees.pycfn.com

@contextlib.contextmanager
来源：http://fxd.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://bwb.jyoumei.cn

list(zip(*m))
来源：http://nkt.ctjpmb.com

[U23] Py：分块读取大文件
来源：http://zei.fzhhl.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fnt.jinqigfzy.top

[U24] Py：路径操作
来源：http://ewy.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pxh.daxiang520.top

[U25] Py：CSV 按字典读
来源：http://xpc.vqdsnc.cn

csv.DictReader(f)
来源：http://wiu.jqgufenzy.top

[U26] Py：并发下载
来源：http://dym.snrcjt.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://shw.hcnkem.com

[U27] Py：异步 HTTP
来源：http://obw.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://zpu.jianghu66.top

[U28] Py：类型别名
来源：http://vze.hammf.cn

UserId = int
来源：http://uwj.zhengqikj.top

[U29] Py：属性校验
来源：http://aqk.yanxiufei.cn

@property 与 @x.setter 配合
来源：http://ugh.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://vrv.52xcode.cn

@dataclass(slots=True)
来源：http://zum.c1oappe.top

[U31] Py：单测
来源：http://rtd.yuxming.cn

python -m pytest -q
来源：http://gyw.andypj.xyz

[U32] Py：代码格式化
来源：http://jxt.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://mhs.zdqjudy.top

[U33] Py：打包发布
来源：http://vxw.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://wsc.tianlin.xyz

[U34] Py：判断编码
来源：http://lew.zhixingplan.top

chardet.detect(raw)
来源：http://xwm.ctjpmb.com

[U35] Py：发送邮件
来源：http://fnx.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gwi.fktsv.cn

[U36] Py：定时任务
来源：http://eyy.pengpengdd.cyou

schedule.every(10).minutes.do(job)
来源：http://zsk.andypj.xyz

[U37] Py：读写 Excel
来源：http://ytz.ivvv.top

pandas.read_excel / DataFrame.to_excel
来源：http://hci.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://ypi.gotoacloud.top

Path(__file__).resolve().parent
来源：http://afe.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://cha.jyoumei.cn

sys.stdout.isatty()
来源：http://bcw.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://ujd.fehbvm.com

print("err", file=sys.stderr)
来源：http://olq.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://prj.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bsw.bjfxy.top

[U42] PHP：PSR-4 自动加载
来源：http://jev.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aei.gzhubu.top

[U43] PHP：声明命名空间
来源：http://gfi.jiagoushi.top

namespace App\Http;
来源：http://olh.yonumen.top

[U44] PHP：开启严格类型
来源：http://wkb.nwbrower.top

declare(strict_types=1);
来源：http://jro.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://xae.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cmw.zhijiandao.cn

[U46] PHP：可空类型
来源：http://xsj.cheryme.top

?string $name = null
来源：http://ilf.fehbvm.com

[U47] PHP：联合类型
来源：http://mhe.hysaishi.cn

int|string $id
来源：http://tnz.nwbrower.top

[U48] PHP：纯枚举
来源：http://cmr.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oeo.yj20258888.top

[U49] PHP：只读属性
来源：http://pzo.fehbvm.com

public readonly string $name
来源：http://ocv.ctjpmb.com

[U50] PHP：构造器属性提升
来源：http://arx.andypj.xyz

public function __construct(private int $id) {}
来源：http://xab.gaohongyu789.top

[U51] PHP：数组解构
来源：http://zgh.xziqi.cn

[$a, $b] = $arr;
来源：http://soa.dashuyun.cn

[U52] PHP：箭头函数
来源：http://byh.cheryme.top

$double = fn($x) => $x * 2;
来源：http://jce.epnwcf.com

[U53] PHP：空合并运算符
来源：http://lmv.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://cly.cucudq.cn

[U54] PHP：空安全调用
来源：http://lwm.cqqwz.cn

$obj?->method()
来源：http://fwp.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://ukc.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://phm.hnxiangtu.top

[U56] PHP：命名参数
来源：http://kre.ctjpmb.com

f(a: 1, b: 2)
来源：http://oxi.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://fyn.tarul.cn

"值: {$a}"
来源：http://rux.ybcxt.top

[U58] PHP：数组三件套
来源：http://bhk.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uig.haohaochexian.top

[U59] PHP：自定义排序
来源：http://dlj.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://esr.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://qxf.dashuyun.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fik.cucudq.cn

[U61] PHP：正则
来源：http://oju.redwolf501.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cvh.shzxlz.cn

[U62] PHP：日期对象
来源：http://fgt.ydjk.org.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hhh.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://ooq.aizwys.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://htf.ivvv.top

[U64] PHP：目录遍历
来源：http://osj.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://alj.xinyue.icu

[U65] PHP：会话
来源：http://cpq.snrcjt.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cix.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://mpm.sysykeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://whf.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://iyt.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://twq.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://egu.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mjv.shzxlz.cn


<!-- 参考信息 -->