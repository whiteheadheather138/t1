代发 wailian999

[S45] C++：lambda
来源：http://ykx.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pwo.jinqigufen.top

[S46] C++：函数模板
来源：http://ryj.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ghr.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://crg.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tyx.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://vei.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xsh.havefunace.top

while (std::getline(in, line)) { }
来源：http://wfz.ydjk.org.cn

[S49] C++：写文件
来源：http://bux.nwbrower.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xzx.hysaishi.cn

[S50] C++：格式化数字
来源：http://tja.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mdi.tian-w.cn

[S51] C++：显式类型转换
来源：http://knp.xinyue.icu

static_cast<double>(a) / b
来源：http://rup.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://bmn.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://zvn.nanxinkj.top

[S53] C++：移动语义
来源：http://llf.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://vyr.yvedp.cn

[S54] C++：异常处理
来源：http://iow.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ffe.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://yjf.cucudq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nli.sysykeji.top

[S56] C++：optional
来源：http://shx.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zru.nanxuanxn.top

[S57] C++：编译期常量
来源：http://rwr.fktsv.cn

constexpr int N = 10;
来源：http://phj.zhixingplan.top

[S58] C++：命名空间
来源：http://nfn.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://dpq.jinqigufen.top

[S59] C++：静态断言
来源：http://umt.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cpw.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://chu.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rwy.wangshuangyany.cn

================================================================================
来源：http://stz.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jup.zdbjq.cn

================================================================================
来源：http://szm.bjfxy.top

[T01] Kotlin：Hello World
来源：http://seg.dianchejie.cn

println("Hello")
来源：http://fke.tanke756.top

[T02] Kotlin：变量
来源：http://czm.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pmf.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://bhk.hywenlv.cn

"值: $b"
来源：http://fwz.52xcode.cn

[T04] Kotlin：空安全
来源：http://izx.316326.xyz

val n: String? = null;  n?.length
来源：http://yoc.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://dwd.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://roi.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://qxc.yvedp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mlm.uphjek.com

[T07] Kotlin：集合过滤
来源：http://nko.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tch.jianghu66.top

[T08] Kotlin：数据类
来源：http://qvt.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://njh.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://hme.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://xqj.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://oag.yuxming.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oed.kuanghao11.cn

[T11] Kotlin：协程
来源：http://vqe.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fth.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://ebt.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://oha.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://lfo.vqdsnc.cn

val m = mapOf("a" to 1)
来源：http://dhn.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://tmd.sweek.top

for (i in 1..10) println(i)
来源：http://liu.epnwcf.com

[T15] Kotlin：接口
来源：http://niy.sweek.top

interface Shape { fun area(): Double }
来源：http://npu.jianghu66.top

[T16] Swift：Hello World
来源：http://bhf.jiagoushi.top

print("Hello")
来源：http://gpu.0kj1m.cn

[T17] Swift：变量与常量
来源：http://edg.yuanzhike.top

var a = 1;  let b = 2
来源：http://csy.xinyue.icu

[T18] Swift：字符串插值
来源：http://vqx.gaohongyu789.top

"值: \(b)"
来源：http://rde.sweek.top

[T19] Swift：可选绑定
来源：http://eag.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://yrl.smart0.xyz

[T20] Swift：数组操作
来源：http://ala.fanxiaobao.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://kca.52xcode.cn

[T21] Swift：遍历
来源：http://atj.daria6918.cn

for x in a { print(x) }
来源：http://ioz.nwbrower.top

[T22] Swift：字典
来源：http://xet.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://jac.tian-w.cn

[T23] Swift：函数
来源：http://ddc.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ihk.snrcjt.cn

[T24] Swift：闭包
来源：http://fos.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://slc.fengsongda.top

[T25] Swift：结构体
来源：http://zay.yj20258.top

struct P { var x: Int }
来源：http://kyc.hammf.cn

[T26] Swift：类与重写
来源：http://tqs.316326.xyz

class A: Base { override func f() {} }
来源：http://eol.hfpthk.cn

[T27] Swift：错误处理
来源：http://lsh.yvedp.cn

do { try f() } catch { print(error) }
来源：http://xtr.epnwcf.com

[T28] Swift：枚举
来源：http://uiq.nanxinkj.top

enum Color { case red, green }
来源：http://aee.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://smy.yvedp.cn

guard let x = opt else { return }
来源：http://ihj.cashguo.top

[T30] Swift：协议
来源：http://joz.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://wku.daxiang520.top

[T31] Lua：Hello World
来源：http://jrd.svipenyu.cn

print("Hello")
来源：http://hsc.jinqigufen.top

[T32] Lua：局部变量
来源：http://zzi.chenjidiqi.icu

local a = 1
来源：http://xvh.gotoacloud.top

[T33] Lua：表（数组）
来源：http://fky.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ioh.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://thb.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qri.yonumen.top

[T35] Lua：字典表
来源：http://wdw.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://bpk.sjlbkw.cn

[T36] Lua：函数
来源：http://mxu.uphjek.com

function add(a, b) return a + b end
来源：http://vhw.nwbrower.top

[T37] Lua：字符串拼接
来源：http://lyq.yfazqb.com

"a" .. "b"
来源：http://rip.fengsongda.top

[T38] Lua：条件
来源：http://yhm.jinqigufen.top

if x > 0 then print("正") end
来源：http://bif.yangfankeji.com

[T39] Lua：模式匹配
来源：http://xnq.jqgufenzy.top

string.find(s, "%d+")
来源：http://zav.shzxlz.cn

[T40] Lua：元表
来源：http://jic.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://jgb.yongpay.top

[T41] Perl：Hello World
来源：http://spe.zycfv.cn

print "Hello\n";
来源：http://sma.meibo888.top

[T42] Perl：变量类型
来源：http://vxg.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://viw.fengsongda.top

[T43] Perl：字符串插值
来源：http://ltg.nanxuanxn.top

"值: $a"
来源：http://jvi.hammf.cn

[T44] Perl：条件
来源：http://vic.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://lqb.jinqigufen.top

[T45] Perl：数组遍历
来源：http://xnb.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://zmr.yongpay.top

[T46] Perl：哈希操作
来源：http://pxx.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kgk.yfazqb.com

[T47] Perl：正则捕获
来源：http://nuz.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kgf.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://svs.yvedp.cn

$s =~ s/old/new/g;
来源：http://mye.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://ixu.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pzh.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://zmy.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://upw.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://fny.cqqwz.cn

[T51] Scala：Hello World
来源：http://jji.mhx1999.top

println("Hello")
来源：http://mgc.ydzc1.top

[T52] Scala：变量
来源：http://mya.ybcxt.top

val a = 1;  var b = 2
来源：http://pcp.epnwcf.com

[T53] Scala：字符串插值
来源：http://pht.jianghu66.top

s"值: $b"
来源：http://dtt.ydjk.org.cn

[T54] Scala：集合映射
来源：http://vxs.0kj1m.cn

List(1, 2, 3).map(_ * 2)
来源：http://xke.shuidangran.top

[T55] Scala：集合过滤
来源：http://muo.uphjek.com

List(1, 2, 3).filter(_ > 1)
来源：http://jzh.ydjk.org.cn

[T56] Scala：样例类
来源：http://uuu.zdbjq.cn

case class User(name: String, age: Int)
来源：http://xzw.haohaochexian.top

[T57] Scala：模式匹配
来源：http://wed.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nrj.zhoulong.xyz

[T58] Scala：函数定义
来源：http://uei.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tsc.ybcxt.top

[T59] Scala：循环
来源：http://cht.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://plp.hongshengwenyu.top

[T60] Scala：折叠
来源：http://tiz.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ekh.chenzaomai.com

================================================================================
来源：http://qcr.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mle.gogol.net.cn

================================================================================
来源：http://dzx.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://gph.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://kyg.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://vil.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rtn.havefunace.top

[U03] Py：加载 .env 配置
来源：http://yij.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qvx.hcnkem.com

[U04] Py：变量调试打印
来源：http://kgt.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ese.fengsongda.top

[U05] Py：列表去重且保序
来源：http://vzv.hesvh.cn

list(dict.fromkeys(arr))
来源：http://shu.fengsongda.top

[U06] Py：合并两个字典
来源：http://dkb.redwolf501.top

{**a, **b}
来源：http://sip.ybcxt.top

[U07] Py：反转字典键值
来源：http://bpm.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://umm.yangfankeji.com

[U08] Py：展平二维列表
来源：http://bvd.tianlin.xyz

[y for x in nested for y in x]
来源：http://lzm.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://fdi.52xcode.cn

max(d, key=d.get)
来源：http://jvm.aizwys.cn

[U10] Py：按值排序字典
来源：http://qtf.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ert.ybcxt.top

[U11] Py：生成器表达式
来源：http://fhk.havefunace.top

(x * 2 for x in arr)
来源：http://lwc.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yjr.ctjpmb.com

Counter(arr).most_common(3)
来源：http://jpn.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://vdw.dashuyun.cn

deque(maxlen=10)
来源：http://ymo.mhx1999.top

[U14] Py：分组收集到列表
来源：http://bsx.zhongyouzk.top

defaultdict(list)
来源：http://smp.sweek.top

[U15] Py：高精度计时
来源：http://tst.aibaodan.cn

t = time.perf_counter()
来源：http://kkf.ybcxt.top

[U16] Py：命令行参数解析
来源：http://tou.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mgt.fengsongda.top

[U17] Py：初始化日志
来源：http://yun.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://sfj.jinqigfzy.top

[U18] Py：预编译正则
来源：http://tft.cucudq.cn

pat = re.compile(r"\d+")
来源：http://snn.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://zrh.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wrf.iojbl.cn

[U20] Py：缓存函数结果
来源：http://lze.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://bti.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://qvk.cucudq.cn

@contextlib.contextmanager
来源：http://uwo.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://gwo.jqgufenzy.top

list(zip(*m))
来源：http://jsz.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://fmo.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qiq.zhiwuduotai.top

[U24] Py：路径操作
来源：http://smn.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wcs.hcnkem.com

[U25] Py：CSV 按字典读
来源：http://fms.quarkkingdee.top

csv.DictReader(f)
来源：http://fpu.hammf.cn

[U26] Py：并发下载
来源：http://dhc.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fio.andypj.xyz

[U27] Py：异步 HTTP
来源：http://scy.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://prg.tian-w.cn

[U28] Py：类型别名
来源：http://nxf.ehwqpu.com

UserId = int
来源：http://lkn.yj202588.top

[U29] Py：属性校验
来源：http://oxa.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://asf.nwbrower.top

[U30] Py：数据类
来源：http://exi.ppjwa.cn

@dataclass(slots=True)
来源：http://snu.ctjpmb.com

[U31] Py：单测
来源：http://nhq.wangdashe.top

python -m pytest -q
来源：http://vyc.mhx1999.top

[U32] Py：代码格式化
来源：http://lfo.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://qxu.yanxiufei.cn

[U33] Py：打包发布
来源：http://bmc.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://uzw.yangfankeji.com

[U34] Py：判断编码
来源：http://piv.0kj1m.cn

chardet.detect(raw)
来源：http://ipp.redwolf501.top

[U35] Py：发送邮件
来源：http://cnc.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hpp.hfpthk.cn

[U36] Py：定时任务
来源：http://dfs.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://qlx.yueranfly.top

[U37] Py：读写 Excel
来源：http://qrv.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://tmy.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://npg.ivvv.top

Path(__file__).resolve().parent
来源：http://rxw.sufxvd.cn

[U39] Py：判断是否在交互环境
来源：http://wvb.xylfe.cn

sys.stdout.isatty()
来源：http://bkk.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://fug.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://mgp.svipenyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://vvd.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://xdk.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://iqp.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zwh.xziqi.cn

[U43] PHP：声明命名空间
来源：http://kwa.tarul.cn

namespace App\Http;
来源：http://yce.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://awv.chenzaomai.com

declare(strict_types=1);
来源：http://nki.gotoacloud.top

[U45] PHP：类型声明与返回类型
来源：http://qyn.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kde.hcnkem.com

[U46] PHP：可空类型
来源：http://wdz.sufxvd.cn

?string $name = null
来源：http://dqo.9152youxi.cn

[U47] PHP：联合类型
来源：http://evk.zhengqikj.top

int|string $id
来源：http://rss.meibo888.top

[U48] PHP：纯枚举
来源：http://rvx.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xle.shuidangran.top

[U49] PHP：只读属性
来源：http://bfy.guowangkeji.top

public readonly string $name
来源：http://ynm.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://gkr.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://ogr.sxryk.cn

[U51] PHP：数组解构
来源：http://guu.daria6918.cn

[$a, $b] = $arr;
来源：http://pfq.svipenyu.cn

[U52] PHP：箭头函数
来源：http://dhy.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://teg.tian-w.cn

[U53] PHP：空合并运算符
来源：http://omr.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://hbb.haohaochexian.top

[U54] PHP：空安全调用
来源：http://ijm.jlsjyb.cn

$obj?->method()
来源：http://jul.chenlongwang.top

[U55] PHP：match 表达式
来源：http://nmb.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jfh.zhijiandao.cn

[U56] PHP：命名参数
来源：http://fic.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://vev.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://pzo.mhx1999.top

"值: {$a}"
来源：http://kee.zhixingplan.top

[U58] PHP：数组三件套
来源：http://vxb.yuanzhike.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ztt.hysaishi.cn

[U59] PHP：自定义排序
来源：http://mma.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ygb.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://ygy.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lda.jqgfzy.top

[U61] PHP：正则
来源：http://tqg.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zle.zdbjq.cn

[U62] PHP：日期对象
来源：http://fng.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wmk.ywan-chungtsiang.top

[U63] PHP：文件读写
来源：http://apf.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tja.svipenyu.cn

[U64] PHP：目录遍历
来源：http://ouj.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://fbv.hongshengwenyu.top

[U65] PHP：会话
来源：http://wmk.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://bsg.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://oxo.yangfankeji.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qnx.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://vpd.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iom.yj20258888.top

[U68] PHP：PDO 连接
来源：http://djj.cucudq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qdw.birdmap.top

[U69] PHP：PDO 预处理
来源：http://vgm.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nmz.yonumen.top

[U70] PHP：PDO 事务
来源：http://kww.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xhy.zdbjq.cn


<!-- 参考信息 -->