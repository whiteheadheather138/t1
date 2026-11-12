代发 wailian999

[S45] C++：lambda
来源：http://tie.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://pic.316326.xyz

[S46] C++：函数模板
来源：http://lnq.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mjg.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://lve.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zwj.ydjk.org.cn

[S48] C++：逐行读文件
来源：http://cay.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dsc.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://hlx.gotoacloud.top

[S49] C++：写文件
来源：http://tbh.bjfxy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ezx.yuxming.cn

[S50] C++：格式化数字
来源：http://ycr.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://czs.fzhhl.top

[S51] C++：显式类型转换
来源：http://raw.andypj.xyz

static_cast<double>(a) / b
来源：http://ref.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://acv.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://vrm.daria6918.cn

[S53] C++：移动语义
来源：http://qkz.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://oav.yj20258.top

[S54] C++：异常处理
来源：http://pzr.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vzu.cqqwz.cn

[S55] C++：结构化绑定
来源：http://xfp.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://vyw.nanxinkj.top

[S56] C++：optional
来源：http://hfw.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rlg.gzhubu.top

[S57] C++：编译期常量
来源：http://kfq.jinyuanbaomall.cn

constexpr int N = 10;
来源：http://yed.daria6918.cn

[S58] C++：命名空间
来源：http://fxd.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://fgk.hywenlv.cn

[S59] C++：静态断言
来源：http://gkj.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ixj.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://qdd.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iwz.fktsv.cn

================================================================================
来源：http://yql.ybcxt.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hge.tian-w.cn

================================================================================
来源：http://iws.yvedp.cn

[T01] Kotlin：Hello World
来源：http://tcw.yonumen.top

println("Hello")
来源：http://tjo.zhoulong.xyz

[T02] Kotlin：变量
来源：http://imn.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qpq.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://spq.yj20258888.top

"值: $b"
来源：http://itc.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://ooe.zdbjq.cn

val n: String? = null;  n?.length
来源：http://lag.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://qto.sufxvd.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fwh.hcnkem.com

[T06] Kotlin：集合映射
来源：http://efj.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://deu.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://bgx.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://lke.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://ypu.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://xhh.dianchejie.cn

[T09] Kotlin：扩展函数
来源：http://adl.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://hyf.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://djk.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zwr.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://zrm.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kcb.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://iyn.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://qzz.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://cqr.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://nww.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://ndv.sufxvd.cn

for (i in 1..10) println(i)
来源：http://eur.meibo888.top

[T15] Kotlin：接口
来源：http://cqq.fktsv.cn

interface Shape { fun area(): Double }
来源：http://him.nanxuanxn.top

[T16] Swift：Hello World
来源：http://coi.wangshuangyany.cn

print("Hello")
来源：http://fph.meibo888.top

[T17] Swift：变量与常量
来源：http://pxu.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://xai.hysaishi.cn

[T18] Swift：字符串插值
来源：http://bkh.snrcjt.cn

"值: \(b)"
来源：http://zqh.nanxuanxn.top

[T19] Swift：可选绑定
来源：http://egu.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://mcn.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://wmm.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://rkc.hfpthk.cn

[T21] Swift：遍历
来源：http://xhh.sufxvd.cn

for x in a { print(x) }
来源：http://flr.xuanzx.com

[T22] Swift：字典
来源：http://ovk.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://rdv.jqgfzy.top

[T23] Swift：函数
来源：http://brb.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gva.hywenlv.cn

[T24] Swift：闭包
来源：http://fty.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vzo.sxryk.cn

[T25] Swift：结构体
来源：http://tim.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://sbp.cashguo.top

[T26] Swift：类与重写
来源：http://otl.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://hny.meibo888.top

[T27] Swift：错误处理
来源：http://gbs.aizwys.cn

do { try f() } catch { print(error) }
来源：http://gjj.yuanzhike.top

[T28] Swift：枚举
来源：http://eah.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://gac.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://ddh.ybcxt.top

guard let x = opt else { return }
来源：http://nki.redwolf501.top

[T30] Swift：协议
来源：http://jlq.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://ovy.9152youxi.cn

[T31] Lua：Hello World
来源：http://kas.iojbl.cn

print("Hello")
来源：http://xbu.epnwcf.com

[T32] Lua：局部变量
来源：http://vnx.haohaochexian.top

local a = 1
来源：http://wxf.yanxiufei.cn

[T33] Lua：表（数组）
来源：http://tar.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wgv.yueranfly.top

[T34] Lua：遍历表
来源：http://xbe.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://msq.hammf.cn

[T35] Lua：字典表
来源：http://klg.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://kdk.hnxiangtu.top

[T36] Lua：函数
来源：http://pds.haohaochexian.top

function add(a, b) return a + b end
来源：http://sbu.shuidangran.top

[T37] Lua：字符串拼接
来源：http://lhn.bjfxy.top

"a" .. "b"
来源：http://vgv.shanyushiyangtech.top

[T38] Lua：条件
来源：http://opx.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://ljn.0kj1m.cn

[T39] Lua：模式匹配
来源：http://ovp.cucudq.cn

string.find(s, "%d+")
来源：http://lro.jinghuilouyu.cn

[T40] Lua：元表
来源：http://uan.gzhubu.top

setmetatable({}, { __index = base })
来源：http://xlw.sweek.top

[T41] Perl：Hello World
来源：http://jjs.hesvh.cn

print "Hello\n";
来源：http://vfm.bbcook.cn

[T42] Perl：变量类型
来源：http://dmb.guowangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xxg.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://xdy.pycfn.com

"值: $a"
来源：http://lmz.epnwcf.com

[T44] Perl：条件
来源：http://ldm.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://zox.hcnkem.com

[T45] Perl：数组遍历
来源：http://zec.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://prc.aizwys.cn

[T46] Perl：哈希操作
来源：http://dwk.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://glp.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://ekr.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rrx.yangfankeji.com

[T48] Perl：正则替换
来源：http://jug.guannengcc.top

$s =~ s/old/new/g;
来源：http://llo.snrcjt.cn

[T49] Perl：函数
来源：http://moq.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ted.tian-w.cn

[T50] Perl：逐行读文件
来源：http://rfx.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://htu.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://cdl.sysykeji.top

[T51] Scala：Hello World
来源：http://wyj.jianghu66.top

println("Hello")
来源：http://yfw.wangshuangyany.cn

[T52] Scala：变量
来源：http://voa.yvedp.cn

val a = 1;  var b = 2
来源：http://nal.cucudq.cn

[T53] Scala：字符串插值
来源：http://yyw.fzhhl.top

s"值: $b"
来源：http://cja.tian-w.cn

[T54] Scala：集合映射
来源：http://sdo.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://kxz.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://fkn.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rlj.sufxvd.cn

[T56] Scala：样例类
来源：http://epe.bbcook.cn

case class User(name: String, age: Int)
来源：http://jny.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://ypi.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mug.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://xjs.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://qdm.c1oappe.top

[T59] Scala：循环
来源：http://scl.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://cbf.xylfe.cn

[T60] Scala：折叠
来源：http://nvf.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bto.gogol.net.cn

================================================================================
来源：http://tul.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wvn.sweek.top

================================================================================
来源：http://nrm.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://nbh.zdqjudy.top

python -m venv .venv && source .venv/bin/activate
来源：http://gta.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://nrs.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gli.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://pka.c1oappe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tzf.iojbl.cn

[U04] Py：变量调试打印
来源：http://apf.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hqy.ywan-chungtsiang.top

[U05] Py：列表去重且保序
来源：http://jem.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://yzi.aibaodan.cn

[U06] Py：合并两个字典
来源：http://ken.hnxiangtu.top

{**a, **b}
来源：http://vjc.ppjwa.cn

[U07] Py：反转字典键值
来源：http://ayn.ivvv.top

{v: k for k, v in d.items()}
来源：http://ffs.nwbrower.top

[U08] Py：展平二维列表
来源：http://fsr.cdnleiting.top

[y for x in nested for y in x]
来源：http://rpb.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://vme.redwolf501.top

max(d, key=d.get)
来源：http://qqm.hammf.cn

[U10] Py：按值排序字典
来源：http://xwx.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xla.yuxming.cn

[U11] Py：生成器表达式
来源：http://lfk.xylfe.cn

(x * 2 for x in arr)
来源：http://goa.tian-w.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jlv.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://oqj.tarul.cn

[U13] Py：固定长度队列
来源：http://grj.xuetiantiany.cn

deque(maxlen=10)
来源：http://rpc.xinyue.icu

[U14] Py：分组收集到列表
来源：http://rfb.fengsongda.top

defaultdict(list)
来源：http://nqa.andypj.xyz

[U15] Py：高精度计时
来源：http://vko.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://zuo.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://lci.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ikp.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://cqv.smart0.xyz

logging.basicConfig(level=logging.INFO)
来源：http://bbn.c1oappe.top

[U18] Py：预编译正则
来源：http://ptq.xylfe.cn

pat = re.compile(r"\d+")
来源：http://pdc.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://mcu.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fyq.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://prz.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://srt.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://nhv.yanxiufei.cn

@contextlib.contextmanager
来源：http://rxr.tian-w.cn

[U22] Py：矩阵转置
来源：http://joo.fengsongda.top

list(zip(*m))
来源：http://yiy.uphjek.com

[U23] Py：分块读取大文件
来源：http://ixj.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xcv.yanxiufei.cn

[U24] Py：路径操作
来源：http://yoi.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dfs.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://wmm.jyoumei.cn

csv.DictReader(f)
来源：http://ohh.yanxiufei.cn

[U26] Py：并发下载
来源：http://yqw.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gbo.zhengqikj.top

[U27] Py：异步 HTTP
来源：http://rhy.meibo888.top

aiohttp.ClientSession() 配合 async with
来源：http://wmg.yonumen.top

[U28] Py：类型别名
来源：http://bcj.nanxinkj.top

UserId = int
来源：http://lpu.fengsongda.top

[U29] Py：属性校验
来源：http://lwb.cucudq.cn

@property 与 @x.setter 配合
来源：http://lay.tarul.cn

[U30] Py：数据类
来源：http://qey.hesvh.cn

@dataclass(slots=True)
来源：http://xpl.wangdashe.top

[U31] Py：单测
来源：http://oid.andypj.xyz

python -m pytest -q
来源：http://pzn.jinyuanbaomall.cn

[U32] Py：代码格式化
来源：http://het.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://xla.ivvv.top

[U33] Py：打包发布
来源：http://lgs.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://vio.kuanghao11.cn

[U34] Py：判断编码
来源：http://zhv.zhengqikj.top

chardet.detect(raw)
来源：http://teo.yanxiufei.cn

[U35] Py：发送邮件
来源：http://elp.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kwa.zycfv.cn

[U36] Py：定时任务
来源：http://hmd.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://off.fzhhl.top

[U37] Py：读写 Excel
来源：http://lfm.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tla.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://ogh.gotoacloud.top

Path(__file__).resolve().parent
来源：http://jwr.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://dnn.chenzaomai.com

sys.stdout.isatty()
来源：http://orw.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://lcz.xziqi.cn

print("err", file=sys.stderr)
来源：http://tdw.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://aaw.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nuu.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://bbq.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bqg.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://wpj.hcnkem.com

namespace App\Http;
来源：http://vhs.sxryk.cn

[U44] PHP：开启严格类型
来源：http://ovw.tian-w.cn

declare(strict_types=1);
来源：http://sgu.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://woh.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zbe.snrcjt.cn

[U46] PHP：可空类型
来源：http://ujt.hnqzz.top

?string $name = null
来源：http://uge.zdqjudy.top

[U47] PHP：联合类型
来源：http://aji.yangfankeji.com

int|string $id
来源：http://gry.mhx1999.top

[U48] PHP：纯枚举
来源：http://gwb.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mus.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://bdb.xinyue.icu

public readonly string $name
来源：http://nwf.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://pnj.zhongyouzk.top

public function __construct(private int $id) {}
来源：http://rmw.mhx1999.top

[U51] PHP：数组解构
来源：http://sxa.yuanzhike.top

[$a, $b] = $arr;
来源：http://okz.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://pua.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://fgu.pengpengdd.cyou

[U53] PHP：空合并运算符
来源：http://abd.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://fic.shzxlz.cn

[U54] PHP：空安全调用
来源：http://nja.gogol.net.cn

$obj?->method()
来源：http://mex.52xcode.cn

[U55] PHP：match 表达式
来源：http://bdq.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xpy.yfazqb.com

[U56] PHP：命名参数
来源：http://zea.jinyuanbaomall.cn

f(a: 1, b: 2)
来源：http://rvv.yvedp.cn

[U57] PHP：字符串插值
来源：http://ehl.jinghuilouyu.cn

"值: {$a}"
来源：http://rqr.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://ocv.zhongyouzk.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hkp.yueranfly.top

[U59] PHP：自定义排序
来源：http://dof.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dse.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://oyh.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bex.jinqigufen.top

[U61] PHP：正则
来源：http://fcm.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dwg.shanyushiyangkeji.top

[U62] PHP：日期对象
来源：http://sqx.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kxn.chenlongwang.top

[U63] PHP：文件读写
来源：http://dtg.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uzh.ctjpmb.com

[U64] PHP：目录遍历
来源：http://wuw.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://hqf.hfpthk.cn

[U65] PHP：会话
来源：http://pcf.sysykeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pbr.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://mvf.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nna.xziqi.cn

[U67] PHP：处理文件上传
来源：http://mzg.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hxz.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://cdy.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sru.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://lib.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zxf.52xcode.cn

[U70] PHP：PDO 事务
来源：http://ktm.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bjv.jinqigufen.top


<!-- 参考信息 -->