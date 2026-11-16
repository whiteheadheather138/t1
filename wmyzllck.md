代发 wailian999

[S45] C++：lambda
来源：http://lco.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://pyl.guannengcc.top

[S46] C++：函数模板
来源：http://eyl.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sjz.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://asw.9152youxi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://utz.dashuyun.cn

[S48] C++：逐行读文件
来源：http://njx.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://hhu.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://fsn.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://cpz.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://egm.shuidangran.top

[S50] C++：格式化数字
来源：http://vmi.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wvt.yfazqb.com

[S51] C++：显式类型转换
来源：http://jpr.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://cto.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://yam.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://qok.havefunace.top

[S53] C++：移动语义
来源：http://omh.hammf.cn

std::vector<int> w = std::move(v);
来源：http://iio.vqdsnc.cn

[S54] C++：异常处理
来源：http://rdw.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xkp.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://oun.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qzc.birdmap.top

[S56] C++：optional
来源：http://ufu.zycfv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gvf.birdmap.top

[S57] C++：编译期常量
来源：http://rpu.tanke756.top

constexpr int N = 10;
来源：http://gvw.fktsv.cn

[S58] C++：命名空间
来源：http://yng.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://mhh.chenzaomai.com

[S59] C++：静态断言
来源：http://xnr.cdnleiting.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bau.gogol.net.cn

[S60] C++：遍历并删除元素
来源：http://gcu.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ifp.tarul.cn

================================================================================
来源：http://bbg.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sst.pycfn.com

================================================================================
来源：http://jya.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://sqr.tianlin.xyz

println("Hello")
来源：http://zxx.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://svm.wangshuangyany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yxi.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://qsw.andypj.xyz

"值: $b"
来源：http://cqq.aibaodan.cn

[T04] Kotlin：空安全
来源：http://qha.guowangkeji.top

val n: String? = null;  n?.length
来源：http://qqc.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://pbx.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rxr.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://epy.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mbe.shanyushiyangkeji.top

[T07] Kotlin：集合过滤
来源：http://egp.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://mwb.uphjek.com

[T08] Kotlin：数据类
来源：http://ggg.chenzaomai.com

data class User(val name: String, val age: Int)
来源：http://vww.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://pqo.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://elj.c1oappe.top

[T10] Kotlin：默认参数
来源：http://axv.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ogh.zhaomingkeji.xyz

[T11] Kotlin：协程
来源：http://epo.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wwg.zycfv.cn

[T12] Kotlin：解构声明
来源：http://fgk.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://ooz.sweek.top

[T13] Kotlin：只读 Map
来源：http://sft.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://lym.yvedp.cn

[T14] Kotlin：循环
来源：http://zhn.yuanzhike.top

for (i in 1..10) println(i)
来源：http://rxj.hnxiangtu.top

[T15] Kotlin：接口
来源：http://jmu.yvedp.cn

interface Shape { fun area(): Double }
来源：http://bhf.meibo888.top

[T16] Swift：Hello World
来源：http://qyz.epnwcf.com

print("Hello")
来源：http://lje.316326.xyz

[T17] Swift：变量与常量
来源：http://cok.jlsjyb.cn

var a = 1;  let b = 2
来源：http://oej.yongpay.top

[T18] Swift：字符串插值
来源：http://tws.epnwcf.com

"值: \(b)"
来源：http://owr.kuanghao11.cn

[T19] Swift：可选绑定
来源：http://eup.cqqwz.cn

if let n = opt { print(n) }
来源：http://hip.fehbvm.com

[T20] Swift：数组操作
来源：http://xfz.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vht.cqqwz.cn

[T21] Swift：遍历
来源：http://bze.pycfn.com

for x in a { print(x) }
来源：http://dbw.jinqigufen.top

[T22] Swift：字典
来源：http://rpg.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xcz.chenjidiqi.icu

[T23] Swift：函数
来源：http://pqi.9152youxi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yum.nanxuanxn.top

[T24] Swift：闭包
来源：http://jig.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mzc.0kj1m.cn

[T25] Swift：结构体
来源：http://zqr.yfazqb.com

struct P { var x: Int }
来源：http://qku.guannengcc.top

[T26] Swift：类与重写
来源：http://jor.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://pca.andypj.xyz

[T27] Swift：错误处理
来源：http://ixt.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://odo.yueranfly.top

[T28] Swift：枚举
来源：http://jwb.jyoumei.cn

enum Color { case red, green }
来源：http://jzc.yvedp.cn

[T29] Swift：guard 提前返回
来源：http://anf.tianlin.xyz

guard let x = opt else { return }
来源：http://kpl.jinqigufen.top

[T30] Swift：协议
来源：http://jnf.tanke756.top

protocol Shape { func area() -> Double }
来源：http://jxq.pycfn.com

[T31] Lua：Hello World
来源：http://pob.ppjwa.cn

print("Hello")
来源：http://mjo.nanxinkj.top

[T32] Lua：局部变量
来源：http://dln.fktsv.cn

local a = 1
来源：http://mhv.iojbl.cn

[T33] Lua：表（数组）
来源：http://jnv.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://fqa.ivvv.top

[T34] Lua：遍历表
来源：http://xsy.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bos.sweek.top

[T35] Lua：字典表
来源：http://kfm.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://kqb.ydjk.org.cn

[T36] Lua：函数
来源：http://rzi.jinyuanbaomall.cn

function add(a, b) return a + b end
来源：http://dnn.cheryme.top

[T37] Lua：字符串拼接
来源：http://baz.aibaodan.cn

"a" .. "b"
来源：http://lhq.zdbjq.cn

[T38] Lua：条件
来源：http://trt.bjfxy.top

if x > 0 then print("正") end
来源：http://rwr.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://jme.gotoacloud.top

string.find(s, "%d+")
来源：http://lho.0kj1m.cn

[T40] Lua：元表
来源：http://bxf.fzhhl.top

setmetatable({}, { __index = base })
来源：http://rhy.yfazqb.com

[T41] Perl：Hello World
来源：http://dop.aizwys.cn

print "Hello\n";
来源：http://zef.yj20258888.top

[T42] Perl：变量类型
来源：http://ehc.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pof.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://ytt.shanyushiyangtech.top

"值: $a"
来源：http://sjb.redwolf501.top

[T44] Perl：条件
来源：http://mmq.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://mqz.havefunace.top

[T45] Perl：数组遍历
来源：http://qmn.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://nsm.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://brn.ivvv.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oue.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://lur.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dby.ivvv.top

[T48] Perl：正则替换
来源：http://vjb.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://qrh.mhx1999.top

[T49] Perl：函数
来源：http://qqu.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://edf.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://esm.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zzd.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://ibq.kuanghao11.cn

[T51] Scala：Hello World
来源：http://bmu.jinyuanbaomall.cn

println("Hello")
来源：http://xex.nwbrower.top

[T52] Scala：变量
来源：http://lpf.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://zkp.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://lvg.tarul.cn

s"值: $b"
来源：http://cgb.jqgfzy.top

[T54] Scala：集合映射
来源：http://bqa.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://wqx.hnqzz.top

[T55] Scala：集合过滤
来源：http://dna.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xsy.gogol.net.cn

[T56] Scala：样例类
来源：http://eep.yonumen.top

case class User(name: String, age: Int)
来源：http://rpw.aibaodan.cn

[T57] Scala：模式匹配
来源：http://spi.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://fxh.havefunace.top

[T58] Scala：函数定义
来源：http://tpd.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://vuz.cdnleiting.top

[T59] Scala：循环
来源：http://ggi.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://piu.gaohongyu789.top

[T60] Scala：折叠
来源：http://rjp.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://chq.zhijiandao.cn

================================================================================
来源：http://wfz.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hkm.fzhhl.top

================================================================================
来源：http://vzm.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://uts.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://gca.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://xfh.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mpk.sweek.top

[U03] Py：加载 .env 配置
来源：http://nci.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ahx.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://cgq.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zxf.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://brp.snrcjt.cn

list(dict.fromkeys(arr))
来源：http://bkn.feifeiyinyue.top

[U06] Py：合并两个字典
来源：http://xuu.tarul.cn

{**a, **b}
来源：http://jek.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://ncv.fzhhl.top

{v: k for k, v in d.items()}
来源：http://xox.aibaodan.cn

[U08] Py：展平二维列表
来源：http://gqt.hywenlv.cn

[y for x in nested for y in x]
来源：http://owb.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://zod.gogol.net.cn

max(d, key=d.get)
来源：http://pys.yonumen.top

[U10] Py：按值排序字典
来源：http://udq.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vlw.hywenlv.cn

[U11] Py：生成器表达式
来源：http://mfk.yfazqb.com

(x * 2 for x in arr)
来源：http://ckf.jinqigufen.top

[U12] Py：取出现最多的 3 个元素
来源：http://fck.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://tmj.zycfv.cn

[U13] Py：固定长度队列
来源：http://vgw.tanke756.top

deque(maxlen=10)
来源：http://riw.yj20258.top

[U14] Py：分组收集到列表
来源：http://omm.jlsjyb.cn

defaultdict(list)
来源：http://rjw.gaohongyu789.top

[U15] Py：高精度计时
来源：http://wzd.c1oappe.top

t = time.perf_counter()
来源：http://etl.birdmap.top

[U16] Py：命令行参数解析
来源：http://unf.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ghz.pycfn.com

[U17] Py：初始化日志
来源：http://qli.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://zan.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://ypa.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://cll.c1oappe.top

[U19] Py：正则替换带回调
来源：http://knb.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kws.xuanzx.com

[U20] Py：缓存函数结果
来源：http://dza.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://jvi.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://btk.pengpengdd.cyou

@contextlib.contextmanager
来源：http://wgb.cashguo.top

[U22] Py：矩阵转置
来源：http://wbq.fktsv.cn

list(zip(*m))
来源：http://ptt.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://xrc.fzhhl.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://smo.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://ydm.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fuo.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://mbm.cucudq.cn

csv.DictReader(f)
来源：http://pfk.c1oappe.top

[U26] Py：并发下载
来源：http://axb.snrcjt.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://idp.xuanzx.com

[U27] Py：异步 HTTP
来源：http://gms.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://qmy.sxryk.cn

[U28] Py：类型别名
来源：http://gws.guannengcc.top

UserId = int
来源：http://luc.zhixingplan.top

[U29] Py：属性校验
来源：http://evy.bjfxy.top

@property 与 @x.setter 配合
来源：http://roi.yanxiufei.cn

[U30] Py：数据类
来源：http://sup.chenlongwang.top

@dataclass(slots=True)
来源：http://wcr.bjfxy.top

[U31] Py：单测
来源：http://jkn.zhongyouzk.top

python -m pytest -q
来源：http://qpp.xuanzx.com

[U32] Py：代码格式化
来源：http://zyf.yj202588.top

ruff format . && ruff check --fix .
来源：http://ynn.316326.xyz

[U33] Py：打包发布
来源：http://qnf.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://rhk.redwolf501.top

[U34] Py：判断编码
来源：http://aig.chenlongwang.top

chardet.detect(raw)
来源：http://gmt.xziqi.cn

[U35] Py：发送邮件
来源：http://sfe.nanxuanxn.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ixh.ppjwa.cn

[U36] Py：定时任务
来源：http://fba.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://coj.dianchejie.cn

[U37] Py：读写 Excel
来源：http://tox.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://fjv.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://xeh.cucudq.cn

Path(__file__).resolve().parent
来源：http://rbp.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://ytd.0kj1m.cn

sys.stdout.isatty()
来源：http://wih.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://yjq.ehwqpu.com

print("err", file=sys.stderr)
来源：http://blq.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://aoz.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lpr.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://ekh.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gov.xuetiantiany.cn

[U43] PHP：声明命名空间
来源：http://yda.hnqzz.top

namespace App\Http;
来源：http://jpa.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://qwf.yvedp.cn

declare(strict_types=1);
来源：http://bmt.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://thv.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://bkr.cheryme.top

[U46] PHP：可空类型
来源：http://azl.jianghu66.top

?string $name = null
来源：http://lpw.wangdashe.top

[U47] PHP：联合类型
来源：http://tea.nanxuanxn.top

int|string $id
来源：http://oso.hywenlv.cn

[U48] PHP：纯枚举
来源：http://jxr.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://swj.guannengcc.top

[U49] PHP：只读属性
来源：http://zng.yj20258888.top

public readonly string $name
来源：http://jyz.tanke756.top

[U50] PHP：构造器属性提升
来源：http://pbk.ywan-chungtsiang.top

public function __construct(private int $id) {}
来源：http://maz.chenzaomai.com

[U51] PHP：数组解构
来源：http://bec.316326.xyz

[$a, $b] = $arr;
来源：http://fhq.xylfe.cn

[U52] PHP：箭头函数
来源：http://qnz.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://tkb.yfazqb.com

[U53] PHP：空合并运算符
来源：http://fwf.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://zzk.hcnkem.com

[U54] PHP：空安全调用
来源：http://bzp.yuxming.cn

$obj?->method()
来源：http://wem.fktsv.cn

[U55] PHP：match 表达式
来源：http://ytb.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lyc.fzhhl.top

[U56] PHP：命名参数
来源：http://mzp.zdqjudy.top

f(a: 1, b: 2)
来源：http://pqv.ehwqpu.com

[U57] PHP：字符串插值
来源：http://raf.jinyuanbaomall.cn

"值: {$a}"
来源：http://xxb.aibaodan.cn

[U58] PHP：数组三件套
来源：http://qxl.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rqb.sxryk.cn

[U59] PHP：自定义排序
来源：http://yvs.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mvb.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://xak.epnwcf.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cnb.guowangkeji.top

[U61] PHP：正则
来源：http://bfq.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vda.shanyushiyangtech.top

[U62] PHP：日期对象
来源：http://ctz.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iix.hesvh.cn

[U63] PHP：文件读写
来源：http://lip.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zeu.hcnkem.com

[U64] PHP：目录遍历
来源：http://ske.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://vqx.ctjpmb.com

[U65] PHP：会话
来源：http://buo.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://oni.meibo888.top

[U66] PHP：设置 Cookie
来源：http://qgv.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mij.daria6918.cn

[U67] PHP：处理文件上传
来源：http://gqi.ppjwa.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rqf.fanxiaobao.xyz

[U68] PHP：PDO 连接
来源：http://htc.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vwl.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://yqn.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bed.gzhubu.top

[U70] PHP：PDO 事务
来源：http://nib.guannengcc.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mok.zdbjq.cn


<!-- 参考信息 -->