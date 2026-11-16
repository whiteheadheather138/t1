代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://mnw.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mtw.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://ysy.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://wwj.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://yjk.bbcook.cn

[S49] C++：写文件
来源：http://lpv.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gox.fktsv.cn

[S50] C++：格式化数字
来源：http://koj.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uzo.ctjpmb.com

[S51] C++：显式类型转换
来源：http://szp.jyoumei.cn

static_cast<double>(a) / b
来源：http://zex.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://lsv.yongpay.top

int size() const noexcept { return n_; }
来源：http://xod.ivvv.top

[S53] C++：移动语义
来源：http://esl.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://ohc.yfazqb.com

[S54] C++：异常处理
来源：http://agr.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rmo.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://hwd.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zys.nanxuanxn.top

[S56] C++：optional
来源：http://jsh.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xta.yueranfly.top

[S57] C++：编译期常量
来源：http://bmi.chenlongwang.top

constexpr int N = 10;
来源：http://qds.jqgfzy.top

[S58] C++：命名空间
来源：http://pgk.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://sav.bbcook.cn

[S59] C++：静态断言
来源：http://uup.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pba.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://xqq.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ejb.aibaodan.cn

================================================================================
来源：http://yjs.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hyf.aibaodan.cn

================================================================================
来源：http://oqo.xuanzx.com

[T01] Kotlin：Hello World
来源：http://fra.tanke756.top

println("Hello")
来源：http://lqe.yfazqb.com

[T02] Kotlin：变量
来源：http://pfj.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kvc.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://hmi.yj20258.top

"值: $b"
来源：http://txv.yfazqb.com

[T04] Kotlin：空安全
来源：http://twr.mhx1999.top

val n: String? = null;  n?.length
来源：http://upd.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://mgk.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wdq.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://fhw.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pky.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://igp.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nnr.jianghu66.top

[T08] Kotlin：数据类
来源：http://bzi.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://vpw.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://vah.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://mhh.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://vox.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uck.yonumen.top

[T11] Kotlin：协程
来源：http://ozj.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://lqe.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://txd.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://eht.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://wpj.sysykeji.top

val m = mapOf("a" to 1)
来源：http://qep.52xcode.cn

[T14] Kotlin：循环
来源：http://ioc.gzhubu.top

for (i in 1..10) println(i)
来源：http://bmj.shuidangran.top

[T15] Kotlin：接口
来源：http://ime.bjfxy.top

interface Shape { fun area(): Double }
来源：http://iom.ctjpmb.com

[T16] Swift：Hello World
来源：http://xyz.hysaishi.cn

print("Hello")
来源：http://ddo.fktsv.cn

[T17] Swift：变量与常量
来源：http://vww.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://arc.dashuyun.cn

[T18] Swift：字符串插值
来源：http://gyc.ywan-chungtsiang.top

"值: \(b)"
来源：http://agn.fehbvm.com

[T19] Swift：可选绑定
来源：http://nsq.yongpay.top

if let n = opt { print(n) }
来源：http://myo.xylfe.cn

[T20] Swift：数组操作
来源：http://rkd.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://xrd.yangfankeji.com

[T21] Swift：遍历
来源：http://eyq.cheryme.top

for x in a { print(x) }
来源：http://nyk.jiagoushi.top

[T22] Swift：字典
来源：http://ntr.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://fjn.zhijiandao.cn

[T23] Swift：函数
来源：http://uif.ybcxt.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tvt.xuetiantiany.cn

[T24] Swift：闭包
来源：http://whg.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tnx.feifeiyinyue.top

[T25] Swift：结构体
来源：http://erk.tian-w.cn

struct P { var x: Int }
来源：http://orq.zhiwuduotai.top

[T26] Swift：类与重写
来源：http://yab.gotoacloud.top

class A: Base { override func f() {} }
来源：http://dle.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://cnk.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://bqd.ppjwa.cn

[T28] Swift：枚举
来源：http://ddc.jqgufenzy.top

enum Color { case red, green }
来源：http://ecs.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://ghb.sweek.top

guard let x = opt else { return }
来源：http://rbi.vehdjk.com

[T30] Swift：协议
来源：http://qgr.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://had.gaohongyu789.top

[T31] Lua：Hello World
来源：http://wgs.jyoumei.cn

print("Hello")
来源：http://acn.cucudq.cn

[T32] Lua：局部变量
来源：http://sih.yj20258.top

local a = 1
来源：http://qog.nanxinkj.top

[T33] Lua：表（数组）
来源：http://qio.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ahk.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://lhb.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://alx.hnqzz.top

[T35] Lua：字典表
来源：http://fsq.hongshengwenyu.top

local d = { a = 1 };  d.b = 2
来源：http://jjh.fktsv.cn

[T36] Lua：函数
来源：http://rit.kuanghao11.cn

function add(a, b) return a + b end
来源：http://vzs.fzhhl.top

[T37] Lua：字符串拼接
来源：http://bam.aibaodan.cn

"a" .. "b"
来源：http://sbf.vehdjk.com

[T38] Lua：条件
来源：http://six.haohaochexian.top

if x > 0 then print("正") end
来源：http://vuh.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://nyi.nanxuanxn.top

string.find(s, "%d+")
来源：http://rkd.hywenlv.cn

[T40] Lua：元表
来源：http://lpv.c1oappe.top

setmetatable({}, { __index = base })
来源：http://pyu.tanke756.top

[T41] Perl：Hello World
来源：http://pul.sxryk.cn

print "Hello\n";
来源：http://lbr.yongpay.top

[T42] Perl：变量类型
来源：http://rgj.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gnc.ppjwa.cn

[T43] Perl：字符串插值
来源：http://jhh.fktsv.cn

"值: $a"
来源：http://fkc.zhengqikj.top

[T44] Perl：条件
来源：http://qss.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://gwp.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://plk.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://nww.nanxinkj.top

[T46] Perl：哈希操作
来源：http://yeu.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zko.cucudq.cn

[T47] Perl：正则捕获
来源：http://mrr.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gqd.daria6918.cn

[T48] Perl：正则替换
来源：http://znf.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://uyt.chenlongwang.top

[T49] Perl：函数
来源：http://eht.daxiang520.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cco.hesvh.cn

[T50] Perl：逐行读文件
来源：http://xnr.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ygb.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://gpi.vqdsnc.cn

[T51] Scala：Hello World
来源：http://pyh.yj20258888.top

println("Hello")
来源：http://jwk.gogol.net.cn

[T52] Scala：变量
来源：http://qzr.zhoulong.xyz

val a = 1;  var b = 2
来源：http://ria.daxiang520.top

[T53] Scala：字符串插值
来源：http://fnj.zhixingplan.top

s"值: $b"
来源：http://pdh.aizwys.cn

[T54] Scala：集合映射
来源：http://xyx.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://yka.nanxuanxn.top

[T55] Scala：集合过滤
来源：http://xsa.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://auf.cqqwz.cn

[T56] Scala：样例类
来源：http://sqf.ctjpmb.com

case class User(name: String, age: Int)
来源：http://fdq.dianchejie.cn

[T57] Scala：模式匹配
来源：http://adg.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://low.sufxvd.cn

[T58] Scala：函数定义
来源：http://xkb.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://fku.birdmap.top

[T59] Scala：循环
来源：http://efq.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://rgd.hnqzz.top

[T60] Scala：折叠
来源：http://vfs.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qil.smart0.xyz

================================================================================
来源：http://yxq.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kmz.tanke756.top

================================================================================
来源：http://dkb.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://lgq.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uge.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://pak.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gic.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://xep.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://itp.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://eni.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ohu.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://fod.yvedp.cn

list(dict.fromkeys(arr))
来源：http://mir.yfazqb.com

[U06] Py：合并两个字典
来源：http://xqg.yuanzhike.top

{**a, **b}
来源：http://jbd.smart0.xyz

[U07] Py：反转字典键值
来源：http://wdx.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://yab.cashguo.top

[U08] Py：展平二维列表
来源：http://zxl.pycfn.com

[y for x in nested for y in x]
来源：http://ybs.bbcook.cn

[U09] Py：字典取最大值的键
来源：http://yom.aibaodan.cn

max(d, key=d.get)
来源：http://jfa.xziqi.cn

[U10] Py：按值排序字典
来源：http://gwb.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bqu.c1oappe.top

[U11] Py：生成器表达式
来源：http://rny.jiagoushi.top

(x * 2 for x in arr)
来源：http://uuq.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://gvr.aizwys.cn

Counter(arr).most_common(3)
来源：http://sho.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://nyq.jinqigfzy.top

deque(maxlen=10)
来源：http://ztd.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://iue.jinqigfzy.top

defaultdict(list)
来源：http://kux.yanxiufei.cn

[U15] Py：高精度计时
来源：http://lkl.hammf.cn

t = time.perf_counter()
来源：http://bxx.hnqzz.top

[U16] Py：命令行参数解析
来源：http://jbt.meibo888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://scg.hfpthk.cn

[U17] Py：初始化日志
来源：http://jyo.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://oam.cqqwz.cn

[U18] Py：预编译正则
来源：http://jyi.yongpay.top

pat = re.compile(r"\d+")
来源：http://xhx.xinyue.icu

[U19] Py：正则替换带回调
来源：http://tdb.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zlj.ydzc1.top

[U20] Py：缓存函数结果
来源：http://gea.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://uzf.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://fxf.pycfn.com

@contextlib.contextmanager
来源：http://zbh.jiagoushi.top

[U22] Py：矩阵转置
来源：http://qrc.hfpthk.cn

list(zip(*m))
来源：http://ddf.yonumen.top

[U23] Py：分块读取大文件
来源：http://moz.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpz.tanke756.top

[U24] Py：路径操作
来源：http://kzz.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pex.wangdashe.top

[U25] Py：CSV 按字典读
来源：http://kzz.zhijiandao.cn

csv.DictReader(f)
来源：http://rng.aizwys.cn

[U26] Py：并发下载
来源：http://nur.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://llu.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://ojl.wangshuangyany.cn

aiohttp.ClientSession() 配合 async with
来源：http://vcr.jinyuanbaomall.cn

[U28] Py：类型别名
来源：http://alt.xylfe.cn

UserId = int
来源：http://oex.pycfn.com

[U29] Py：属性校验
来源：http://xjy.fktsv.cn

@property 与 @x.setter 配合
来源：http://tfo.ydzc1.top

[U30] Py：数据类
来源：http://snq.jiagoushi.top

@dataclass(slots=True)
来源：http://rjy.chenjidiqi.icu

[U31] Py：单测
来源：http://kbm.sufxvd.cn

python -m pytest -q
来源：http://bvx.tianlin.xyz

[U32] Py：代码格式化
来源：http://bvr.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://kxs.vehdjk.com

[U33] Py：打包发布
来源：http://ein.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://omh.pengpengdd.cyou

[U34] Py：判断编码
来源：http://uzf.yvedp.cn

chardet.detect(raw)
来源：http://oiy.cheryme.top

[U35] Py：发送邮件
来源：http://jat.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://urm.ehwqpu.com

[U36] Py：定时任务
来源：http://jhv.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://yhe.yj20258888.top

[U37] Py：读写 Excel
来源：http://glf.cqqwz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://knr.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://gia.tanke756.top

Path(__file__).resolve().parent
来源：http://rug.52xcode.cn

[U39] Py：判断是否在交互环境
来源：http://opy.shzxlz.cn

sys.stdout.isatty()
来源：http://kvi.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://trn.tianlin.xyz

print("err", file=sys.stderr)
来源：http://vuq.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://ccm.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://etk.zhoulong.xyz

[U42] PHP：PSR-4 自动加载
来源：http://jly.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pxd.xinyue.icu

[U43] PHP：声明命名空间
来源：http://cjb.jqgufenzy.top

namespace App\Http;
来源：http://zbm.yj20258888.top

[U44] PHP：开启严格类型
来源：http://fwk.hysaishi.cn

declare(strict_types=1);
来源：http://vhq.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://ftb.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://flj.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://dnb.aizwys.cn

?string $name = null
来源：http://yon.hnxiangtu.top

[U47] PHP：联合类型
来源：http://zja.vehdjk.com

int|string $id
来源：http://xnp.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://kqj.shanyushiyangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ddt.zhoulong.xyz

[U49] PHP：只读属性
来源：http://sqq.hammf.cn

public readonly string $name
来源：http://saf.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://sgw.cashguo.top

public function __construct(private int $id) {}
来源：http://pyj.wangdashe.top

[U51] PHP：数组解构
来源：http://toj.pycfn.com

[$a, $b] = $arr;
来源：http://jrm.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://ezg.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://zog.uphjek.com

[U53] PHP：空合并运算符
来源：http://pzj.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://hbr.xingfuxueyuan.xyz

[U54] PHP：空安全调用
来源：http://wpu.redwolf501.top

$obj?->method()
来源：http://xyy.cheryme.top

[U55] PHP：match 表达式
来源：http://nbi.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nyl.hnxiangtu.top

[U56] PHP：命名参数
来源：http://ehv.zhijiandao.cn

f(a: 1, b: 2)
来源：http://fut.jinqigufen.top

[U57] PHP：字符串插值
来源：http://jkl.cqqwz.cn

"值: {$a}"
来源：http://qjn.ywan-chungtsiang.top

[U58] PHP：数组三件套
来源：http://rlv.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mxz.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://zop.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gtm.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://gvu.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tjc.zhongyouzk.top

[U61] PHP：正则
来源：http://kos.sweek.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dyp.zdqjudy.top

[U62] PHP：日期对象
来源：http://lxz.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://btm.wangdashe.top

[U63] PHP：文件读写
来源：http://ncx.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hqn.meibo888.top

[U64] PHP：目录遍历
来源：http://wql.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://nkp.zhijiandao.cn

[U65] PHP：会话
来源：http://ooy.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rxb.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://rrb.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xlm.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://via.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lpm.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://sbu.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ehw.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://hwg.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://giz.hesvh.cn

[U70] PHP：PDO 事务
来源：http://ysy.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wbo.ppjwa.cn

[U71] PHP：抛出异常
来源：http://fkq.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://ajx.hfpthk.cn

[U72] PHP：写错误日志
来源：http://zly.chenzaomai.com

error_log("失败: " . $e->getMessage());
来源：http://drk.hfpthk.cn


<!-- 参考信息 -->