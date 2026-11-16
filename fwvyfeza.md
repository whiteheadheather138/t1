代发 wailian999

[S43] C++：智能指针
来源：http://isu.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://mht.dianchejie.cn

[S44] C++：引用传参
来源：http://wbe.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://wnu.andypj.xyz

[S45] C++：lambda
来源：http://kck.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bln.hnqzz.top

[S46] C++：函数模板
来源：http://gcy.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fhk.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://taa.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lww.tianlin.xyz

[S48] C++：逐行读文件
来源：http://kjr.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://luo.xinyue.icu

while (std::getline(in, line)) { }
来源：http://ecx.birdmap.top

[S49] C++：写文件
来源：http://gmt.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qgr.bbcook.cn

[S50] C++：格式化数字
来源：http://xjs.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bbp.tanke756.top

[S51] C++：显式类型转换
来源：http://wvh.guannengcc.top

static_cast<double>(a) / b
来源：http://dmx.cheryme.top

[S52] C++：const 与 noexcept
来源：http://eet.guannengcc.top

int size() const noexcept { return n_; }
来源：http://vgg.guowangkeji.top

[S53] C++：移动语义
来源：http://fuq.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://jlg.yvedp.cn

[S54] C++：异常处理
来源：http://gch.fzhhl.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hiy.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://qxy.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gsb.bjfxy.top

[S56] C++：optional
来源：http://tej.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rxs.ctjpmb.com

[S57] C++：编译期常量
来源：http://lfw.52xcode.cn

constexpr int N = 10;
来源：http://bhc.zhiwuduotai.top

[S58] C++：命名空间
来源：http://xet.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://rmu.hnxiangtu.top

[S59] C++：静态断言
来源：http://way.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uxv.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://ynv.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xyr.yj20258888.top

================================================================================
来源：http://tcs.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ydh.chenlongwang.top

================================================================================
来源：http://ebg.fktsv.cn

[T01] Kotlin：Hello World
来源：http://wns.316326.xyz

println("Hello")
来源：http://ssq.ppjwa.cn

[T02] Kotlin：变量
来源：http://fez.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rwg.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://uxw.tianlin.xyz

"值: $b"
来源：http://qiv.zhengqikj.top

[T04] Kotlin：空安全
来源：http://fke.shuidangran.top

val n: String? = null;  n?.length
来源：http://box.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://ult.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://izw.tanke756.top

[T06] Kotlin：集合映射
来源：http://sbz.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cnb.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://mmu.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mkk.tianlin.xyz

[T08] Kotlin：数据类
来源：http://klh.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://vhf.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://pna.havefunace.top

fun String.exclaim() = this + "!"
来源：http://mdg.yvedp.cn

[T10] Kotlin：默认参数
来源：http://dvl.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://rlp.ppjwa.cn

[T11] Kotlin：协程
来源：http://fxk.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nrj.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://jkb.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://wgy.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://teu.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://btd.yj202588.top

[T14] Kotlin：循环
来源：http://eqi.guannengcc.top

for (i in 1..10) println(i)
来源：http://muz.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://xmn.jianghu66.top

interface Shape { fun area(): Double }
来源：http://mzm.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://vxf.tarul.cn

print("Hello")
来源：http://zjo.zdbjq.cn

[T17] Swift：变量与常量
来源：http://hjs.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://puj.mhx1999.top

[T18] Swift：字符串插值
来源：http://dgs.ehwqpu.com

"值: \(b)"
来源：http://qah.quarkkingdee.top

[T19] Swift：可选绑定
来源：http://hxy.haohaochexian.top

if let n = opt { print(n) }
来源：http://adt.bbcook.cn

[T20] Swift：数组操作
来源：http://bht.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://egy.xuanzx.com

[T21] Swift：遍历
来源：http://pms.nanxuanxn.top

for x in a { print(x) }
来源：http://fww.aibaodan.cn

[T22] Swift：字典
来源：http://mme.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://umy.sjlbkw.cn

[T23] Swift：函数
来源：http://awi.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nxv.jlsjyb.cn

[T24] Swift：闭包
来源：http://jrf.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bnd.guowangkeji.top

[T25] Swift：结构体
来源：http://fdl.hcnkem.com

struct P { var x: Int }
来源：http://xdb.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://giy.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://pna.tarul.cn

[T27] Swift：错误处理
来源：http://vyo.fehbvm.com

do { try f() } catch { print(error) }
来源：http://lip.fzhhl.top

[T28] Swift：枚举
来源：http://ffn.yfazqb.com

enum Color { case red, green }
来源：http://rvq.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://pat.redwolf501.top

guard let x = opt else { return }
来源：http://fst.jianghu66.top

[T30] Swift：协议
来源：http://fvp.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://jvk.gogol.net.cn

[T31] Lua：Hello World
来源：http://org.xylfe.cn

print("Hello")
来源：http://zdj.yanxiufei.cn

[T32] Lua：局部变量
来源：http://smu.xziqi.cn

local a = 1
来源：http://pzg.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://tsg.nwbrower.top

local t = {1, 2, 3};  t[4] = 4
来源：http://opx.hesvh.cn

[T34] Lua：遍历表
来源：http://rrr.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vjx.9152youxi.cn

[T35] Lua：字典表
来源：http://qtf.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://ufm.52xcode.cn

[T36] Lua：函数
来源：http://ezm.fktsv.cn

function add(a, b) return a + b end
来源：http://tgc.hcnkem.com

[T37] Lua：字符串拼接
来源：http://cmm.chenzaomai.com

"a" .. "b"
来源：http://hdg.fktsv.cn

[T38] Lua：条件
来源：http://uwd.jinqigufen.top

if x > 0 then print("正") end
来源：http://qie.sufxvd.cn

[T39] Lua：模式匹配
来源：http://bzz.yuxming.cn

string.find(s, "%d+")
来源：http://ysd.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://npv.sxryk.cn

setmetatable({}, { __index = base })
来源：http://evb.hammf.cn

[T41] Perl：Hello World
来源：http://clk.yuanzhike.top

print "Hello\n";
来源：http://iuc.epnwcf.com

[T42] Perl：变量类型
来源：http://btx.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rpq.nanxinkj.top

[T43] Perl：字符串插值
来源：http://zwr.jinyuanbaomall.cn

"值: $a"
来源：http://gmh.sxryk.cn

[T44] Perl：条件
来源：http://dna.pycfn.com

if ($a > 0) { print "正"; }
来源：http://tut.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://byt.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://gnu.uphjek.com

[T46] Perl：哈希操作
来源：http://gcf.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ymh.gogol.net.cn

[T47] Perl：正则捕获
来源：http://whu.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xiz.gzhubu.top

[T48] Perl：正则替换
来源：http://ebl.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://iyj.vehdjk.com

[T49] Perl：函数
来源：http://wjw.cqqwz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://biy.shanyushiyangkeji.top

[T50] Perl：逐行读文件
来源：http://slr.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fzn.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://gzg.yj20258888.top

[T51] Scala：Hello World
来源：http://yyx.sufxvd.cn

println("Hello")
来源：http://afp.feifeiyinyue.top

[T52] Scala：变量
来源：http://vfb.yonumen.top

val a = 1;  var b = 2
来源：http://bxs.tianlin.xyz

[T53] Scala：字符串插值
来源：http://dey.svipenyu.cn

s"值: $b"
来源：http://ebw.316326.xyz

[T54] Scala：集合映射
来源：http://ywb.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://fjn.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://tyr.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://yqj.quarkkingdee.top

[T56] Scala：样例类
来源：http://yqf.iojbl.cn

case class User(name: String, age: Int)
来源：http://sze.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://pti.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://kuv.52xcode.cn

[T58] Scala：函数定义
来源：http://ycq.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://zam.chenjidiqi.icu

[T59] Scala：循环
来源：http://ljw.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://jed.xuanzx.com

[T60] Scala：折叠
来源：http://jgi.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fgf.hfpthk.cn

================================================================================
来源：http://mxx.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dvp.jianghu66.top

================================================================================
来源：http://oms.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://xup.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://ekr.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://vkm.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tjr.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://xyw.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zmr.jqgfzy.top

[U04] Py：变量调试打印
来源：http://gst.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rza.zhiwuduotai.top

[U05] Py：列表去重且保序
来源：http://vbj.sweek.top

list(dict.fromkeys(arr))
来源：http://tuu.bbcook.cn

[U06] Py：合并两个字典
来源：http://zvb.quarkkingdee.top

{**a, **b}
来源：http://ets.bjfxy.top

[U07] Py：反转字典键值
来源：http://ehy.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://chz.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://inc.yuxming.cn

[y for x in nested for y in x]
来源：http://iwz.birdmap.top

[U09] Py：字典取最大值的键
来源：http://psx.chenzaomai.com

max(d, key=d.get)
来源：http://mek.chenlongwang.top

[U10] Py：按值排序字典
来源：http://wuh.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jwk.fehbvm.com

[U11] Py：生成器表达式
来源：http://nka.tianlin.xyz

(x * 2 for x in arr)
来源：http://mix.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://xgf.xinyue.icu

Counter(arr).most_common(3)
来源：http://gom.cqqwz.cn

[U13] Py：固定长度队列
来源：http://jjf.yanxiufei.cn

deque(maxlen=10)
来源：http://yos.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://uxe.xinyue.icu

defaultdict(list)
来源：http://zif.fengsongda.top

[U15] Py：高精度计时
来源：http://wif.jqgfzy.top

t = time.perf_counter()
来源：http://ubr.uphjek.com

[U16] Py：命令行参数解析
来源：http://all.yfazqb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cqt.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://wxp.andypj.xyz

logging.basicConfig(level=logging.INFO)
来源：http://xqt.tanke756.top

[U18] Py：预编译正则
来源：http://xgx.bbcook.cn

pat = re.compile(r"\d+")
来源：http://fye.jinghuilouyu.cn

[U19] Py：正则替换带回调
来源：http://gkh.zdqjudy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://spv.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://tnx.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://gki.hfpthk.cn

[U21] Py：自定义上下文管理器
来源：http://oxv.yj202588.top

@contextlib.contextmanager
来源：http://kch.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://mej.c1oappe.top

list(zip(*m))
来源：http://hvz.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://yhv.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ajw.gzhubu.top

[U24] Py：路径操作
来源：http://dph.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://owk.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://nal.vehdjk.com

csv.DictReader(f)
来源：http://aeb.cdnleiting.top

[U26] Py：并发下载
来源：http://kas.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ixa.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://xtf.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://dau.guowangkeji.top

[U28] Py：类型别名
来源：http://wze.cashguo.top

UserId = int
来源：http://cnx.zhijiandao.cn

[U29] Py：属性校验
来源：http://soo.ppjwa.cn

@property 与 @x.setter 配合
来源：http://qmf.yj202588.top

[U30] Py：数据类
来源：http://ncj.hnqzz.top

@dataclass(slots=True)
来源：http://edd.ywan-chungtsiang.top

[U31] Py：单测
来源：http://pxt.shangyingyoupin.top

python -m pytest -q
来源：http://vcm.guowangkeji.top

[U32] Py：代码格式化
来源：http://aut.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://trs.haohaochexian.top

[U33] Py：打包发布
来源：http://mep.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://jok.sufxvd.cn

[U34] Py：判断编码
来源：http://nyz.xylfe.cn

chardet.detect(raw)
来源：http://vaf.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://asz.aibaodan.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hhb.cdnleiting.top

[U36] Py：定时任务
来源：http://wqe.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://ufg.yj20258888.top

[U37] Py：读写 Excel
来源：http://lbq.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://inh.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://oht.fengsongda.top

Path(__file__).resolve().parent
来源：http://rrs.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://hez.yanxiufei.cn

sys.stdout.isatty()
来源：http://tei.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://itq.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://fyj.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://hqg.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gzb.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://gsb.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jvg.xinyue.icu

[U43] PHP：声明命名空间
来源：http://jhf.yj20258.top

namespace App\Http;
来源：http://jam.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://xwa.nanxinkj.top

declare(strict_types=1);
来源：http://cck.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://uab.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sci.jinqigufen.top

[U46] PHP：可空类型
来源：http://dii.fanxiaobao.xyz

?string $name = null
来源：http://lia.yj202588.top

[U47] PHP：联合类型
来源：http://quj.jianghu66.top

int|string $id
来源：http://yjp.zycfv.cn

[U48] PHP：纯枚举
来源：http://sef.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zuh.xziqi.cn

[U49] PHP：只读属性
来源：http://vyg.xingfuxueyuan.xyz

public readonly string $name
来源：http://aoh.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://hdm.cucudq.cn

public function __construct(private int $id) {}
来源：http://wnb.daxiang520.top

[U51] PHP：数组解构
来源：http://igk.ywan-chungtsiang.top

[$a, $b] = $arr;
来源：http://xwq.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://azp.sweek.top

$double = fn($x) => $x * 2;
来源：http://hex.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://dhd.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://wwb.yanxiufei.cn

[U54] PHP：空安全调用
来源：http://gzf.chenzaomai.com

$obj?->method()
来源：http://mfv.mhx1999.top

[U55] PHP：match 表达式
来源：http://vgz.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hwl.sjlbkw.cn

[U56] PHP：命名参数
来源：http://ies.zdbjq.cn

f(a: 1, b: 2)
来源：http://zxk.jlsjyb.cn

[U57] PHP：字符串插值
来源：http://fsp.redwolf501.top

"值: {$a}"
来源：http://ipb.cdnleiting.top

[U58] PHP：数组三件套
来源：http://dlu.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sjn.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://pza.chenjidiqi.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bxq.tanke756.top

[U60] PHP：JSON 编解码
来源：http://oqc.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nfa.gzhubu.top

[U61] PHP：正则
来源：http://fnb.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pgq.chenzaomai.com

[U62] PHP：日期对象
来源：http://dfs.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zny.316326.xyz

[U63] PHP：文件读写
来源：http://vhd.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fhm.ppjwa.cn

[U64] PHP：目录遍历
来源：http://vps.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://nht.ctjpmb.com

[U65] PHP：会话
来源：http://mom.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://ufr.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://sxp.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xqg.yvedp.cn

[U67] PHP：处理文件上传
来源：http://ebp.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tqn.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://pka.ydzc1.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eie.vehdjk.com


<!-- 参考信息 -->