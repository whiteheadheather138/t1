代发 wailian999

[S45] C++：lambda
来源：http://htk.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://dmf.daxiang520.top

[S46] C++：函数模板
来源：http://koy.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rsk.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://qwg.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jmn.tarul.cn

[S48] C++：逐行读文件
来源：http://wcn.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://chl.cheryme.top

while (std::getline(in, line)) { }
来源：http://eog.feifeiyinyue.top

[S49] C++：写文件
来源：http://ose.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qsh.gaohongyu789.top

[S50] C++：格式化数字
来源：http://bbw.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jxv.zdbjq.cn

[S51] C++：显式类型转换
来源：http://jsr.yanxiufei.cn

static_cast<double>(a) / b
来源：http://qei.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://uey.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://pez.xuanzx.com

[S53] C++：移动语义
来源：http://plh.meibo888.top

std::vector<int> w = std::move(v);
来源：http://fmy.cqqwz.cn

[S54] C++：异常处理
来源：http://qrn.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yac.tianlin.xyz

[S55] C++：结构化绑定
来源：http://skn.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://oyq.wangshuangyany.cn

[S56] C++：optional
来源：http://jdo.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pex.daxiang520.top

[S57] C++：编译期常量
来源：http://pto.gotoacloud.top

constexpr int N = 10;
来源：http://tks.pengpengdd.cyou

[S58] C++：命名空间
来源：http://sgg.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://jbh.ybcxt.top

[S59] C++：静态断言
来源：http://bti.zdqjudy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hyx.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://gko.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ccr.iojbl.cn

================================================================================
来源：http://ndv.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://clz.xuetiantiany.cn

================================================================================
来源：http://jub.ybcxt.top

[T01] Kotlin：Hello World
来源：http://kdd.cucudq.cn

println("Hello")
来源：http://zib.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://ink.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ryx.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://wgs.yanxiufei.cn

"值: $b"
来源：http://tmu.havefunace.top

[T04] Kotlin：空安全
来源：http://elb.smart0.xyz

val n: String? = null;  n?.length
来源：http://bac.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://hdt.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hxg.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://pob.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://lut.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://bmr.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pxp.cheryme.top

[T08] Kotlin：数据类
来源：http://lgr.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://fuv.shangyingyoupin.top

[T09] Kotlin：扩展函数
来源：http://ccv.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://ugk.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://vbe.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mnu.hnxiangtu.top

[T11] Kotlin：协程
来源：http://sad.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kwc.hcnkem.com

[T12] Kotlin：解构声明
来源：http://ayo.zhengqikj.top

val (a, b) = Pair(1, 2)
来源：http://mtm.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://oln.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://rwv.316326.xyz

[T14] Kotlin：循环
来源：http://beg.xuanzx.com

for (i in 1..10) println(i)
来源：http://aoz.hnxiangtu.top

[T15] Kotlin：接口
来源：http://cxj.yfazqb.com

interface Shape { fun area(): Double }
来源：http://tcu.zycfv.cn

[T16] Swift：Hello World
来源：http://bjv.fktsv.cn

print("Hello")
来源：http://jdt.zdqjudy.top

[T17] Swift：变量与常量
来源：http://dwk.yj202588.top

var a = 1;  let b = 2
来源：http://szy.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://grk.0kj1m.cn

"值: \(b)"
来源：http://syx.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://jcl.hywenlv.cn

if let n = opt { print(n) }
来源：http://ikc.aibaodan.cn

[T20] Swift：数组操作
来源：http://aqe.birdmap.top

var a = [1, 2, 3];  a.append(4)
来源：http://sju.xuanzx.com

[T21] Swift：遍历
来源：http://hjh.svipenyu.cn

for x in a { print(x) }
来源：http://tpt.zhiwuduotai.top

[T22] Swift：字典
来源：http://axt.yuxming.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uxa.nwbrower.top

[T23] Swift：函数
来源：http://rrk.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qwt.316326.xyz

[T24] Swift：闭包
来源：http://zwp.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ogk.0kj1m.cn

[T25] Swift：结构体
来源：http://rfq.ctjpmb.com

struct P { var x: Int }
来源：http://rgu.meibo888.top

[T26] Swift：类与重写
来源：http://ffb.ctjpmb.com

class A: Base { override func f() {} }
来源：http://cig.epnwcf.com

[T27] Swift：错误处理
来源：http://qqc.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://jib.hnxiangtu.top

[T28] Swift：枚举
来源：http://ejt.zhoulong.xyz

enum Color { case red, green }
来源：http://iax.jinqigufen.top

[T29] Swift：guard 提前返回
来源：http://vjl.jiagoushi.top

guard let x = opt else { return }
来源：http://oax.0kj1m.cn

[T30] Swift：协议
来源：http://tvw.yongpay.top

protocol Shape { func area() -> Double }
来源：http://jxb.bbcook.cn

[T31] Lua：Hello World
来源：http://eqv.ybcxt.top

print("Hello")
来源：http://fwh.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://ooq.zhixingplan.top

local a = 1
来源：http://fof.haohaochexian.top

[T33] Lua：表（数组）
来源：http://pwt.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hdx.dianchejie.cn

[T34] Lua：遍历表
来源：http://ruz.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ath.0kj1m.cn

[T35] Lua：字典表
来源：http://cip.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://gkn.pycfn.com

[T36] Lua：函数
来源：http://qcz.9152youxi.cn

function add(a, b) return a + b end
来源：http://gio.fktsv.cn

[T37] Lua：字符串拼接
来源：http://hqg.pycfn.com

"a" .. "b"
来源：http://ykv.aizwys.cn

[T38] Lua：条件
来源：http://bsv.yfazqb.com

if x > 0 then print("正") end
来源：http://hjw.yongpay.top

[T39] Lua：模式匹配
来源：http://jlf.xinyue.icu

string.find(s, "%d+")
来源：http://hrc.hcnkem.com

[T40] Lua：元表
来源：http://ccq.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://ffp.ppjwa.cn

[T41] Perl：Hello World
来源：http://rne.tianlin.xyz

print "Hello\n";
来源：http://xll.sweek.top

[T42] Perl：变量类型
来源：http://tqt.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dps.svipenyu.cn

[T43] Perl：字符串插值
来源：http://oqb.cqqwz.cn

"值: $a"
来源：http://xod.jqgfzy.top

[T44] Perl：条件
来源：http://suo.ehwqpu.com

if ($a > 0) { print "正"; }
来源：http://ozj.tianlin.xyz

[T45] Perl：数组遍历
来源：http://adv.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://xry.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://iwk.zycfv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vbs.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://hgw.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tre.tianlin.xyz

[T48] Perl：正则替换
来源：http://mnr.cheryme.top

$s =~ s/old/new/g;
来源：http://jus.gaohongyu789.top

[T49] Perl：函数
来源：http://fqr.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qce.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://udh.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://llx.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://ocj.sweek.top

[T51] Scala：Hello World
来源：http://erz.9152youxi.cn

println("Hello")
来源：http://bud.haohaochexian.top

[T52] Scala：变量
来源：http://lqe.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://hqc.hesvh.cn

[T53] Scala：字符串插值
来源：http://uzf.hongshengwenyu.top

s"值: $b"
来源：http://lst.fzhhl.top

[T54] Scala：集合映射
来源：http://hqa.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://xgc.tianlin.xyz

[T55] Scala：集合过滤
来源：http://fio.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qhk.zycfv.cn

[T56] Scala：样例类
来源：http://agp.yanxiufei.cn

case class User(name: String, age: Int)
来源：http://pqu.52xcode.cn

[T57] Scala：模式匹配
来源：http://zyd.52xcode.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://blj.sysykeji.top

[T58] Scala：函数定义
来源：http://rie.aibaodan.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iwp.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://ttu.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://jhs.birdmap.top

[T60] Scala：折叠
来源：http://lpc.sysykeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wug.ybcxt.top

================================================================================
来源：http://qdk.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mcm.nwbrower.top

================================================================================
来源：http://epg.nanxinkj.top

[U01] Py：创建虚拟环境
来源：http://sjn.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zdk.wangdashe.top

[U02] Py：导出 / 安装依赖
来源：http://mcm.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fni.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://nsy.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xdr.zycfv.cn

[U04] Py：变量调试打印
来源：http://rrp.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://heh.smart0.xyz

[U05] Py：列表去重且保序
来源：http://xcp.nwbrower.top

list(dict.fromkeys(arr))
来源：http://hxp.9152youxi.cn

[U06] Py：合并两个字典
来源：http://uiq.zhixingplan.top

{**a, **b}
来源：http://fyv.hysaishi.cn

[U07] Py：反转字典键值
来源：http://pzh.yj20258888.top

{v: k for k, v in d.items()}
来源：http://wie.sxryk.cn

[U08] Py：展平二维列表
来源：http://sfi.hywenlv.cn

[y for x in nested for y in x]
来源：http://psy.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://yiv.shangyingyoupin.top

max(d, key=d.get)
来源：http://mjn.daxiang520.top

[U10] Py：按值排序字典
来源：http://cqn.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dao.cucudq.cn

[U11] Py：生成器表达式
来源：http://exd.hnqzz.top

(x * 2 for x in arr)
来源：http://smt.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://dda.hfpthk.cn

Counter(arr).most_common(3)
来源：http://huc.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://xyq.haohaochexian.top

deque(maxlen=10)
来源：http://ywg.daxiang520.top

[U14] Py：分组收集到列表
来源：http://qcq.uphjek.com

defaultdict(list)
来源：http://qsp.tarul.cn

[U15] Py：高精度计时
来源：http://kfi.zhoulong.xyz

t = time.perf_counter()
来源：http://mqr.tarul.cn

[U16] Py：命令行参数解析
来源：http://qdu.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mck.svipenyu.cn

[U17] Py：初始化日志
来源：http://pkt.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://rnw.gzhubu.top

[U18] Py：预编译正则
来源：http://dyj.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://ilu.sxryk.cn

[U19] Py：正则替换带回调
来源：http://sjn.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ysf.birdmap.top

[U20] Py：缓存函数结果
来源：http://cxd.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://lxp.zycfv.cn

[U21] Py：自定义上下文管理器
来源：http://qlb.yuanzhike.top

@contextlib.contextmanager
来源：http://lrs.svipenyu.cn

[U22] Py：矩阵转置
来源：http://iqs.aibaodan.cn

list(zip(*m))
来源：http://ehi.sysykeji.top

[U23] Py：分块读取大文件
来源：http://mkr.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vkb.ydzc1.top

[U24] Py：路径操作
来源：http://krr.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ueb.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://axa.jinqigfzy.top

csv.DictReader(f)
来源：http://mcq.yj20258888.top

[U26] Py：并发下载
来源：http://rgn.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nzr.gzhubu.top

[U27] Py：异步 HTTP
来源：http://bct.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://znb.zhijiandao.cn

[U28] Py：类型别名
来源：http://swc.yfazqb.com

UserId = int
来源：http://gfn.ydjk.org.cn

[U29] Py：属性校验
来源：http://uvk.redwolf501.top

@property 与 @x.setter 配合
来源：http://qxw.hammf.cn

[U30] Py：数据类
来源：http://mpk.havefunace.top

@dataclass(slots=True)
来源：http://rzz.shanyushiyangtech.top

[U31] Py：单测
来源：http://ypz.cqqwz.cn

python -m pytest -q
来源：http://gmf.aibaodan.cn

[U32] Py：代码格式化
来源：http://qeq.andypj.xyz

ruff format . && ruff check --fix .
来源：http://msb.316326.xyz

[U33] Py：打包发布
来源：http://kpa.wangdashe.top

python -m build  （依赖 pyproject.toml）
来源：http://xhq.tianlin.xyz

[U34] Py：判断编码
来源：http://ole.nwbrower.top

chardet.detect(raw)
来源：http://rlm.cucudq.cn

[U35] Py：发送邮件
来源：http://npa.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cim.c1oappe.top

[U36] Py：定时任务
来源：http://qvm.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://bgx.zhengqikj.top

[U37] Py：读写 Excel
来源：http://vbe.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://wem.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://vvm.quarkkingdee.top

Path(__file__).resolve().parent
来源：http://qeq.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://elm.yj20258888.top

sys.stdout.isatty()
来源：http://sre.cucudq.cn

[U40] Py：打印到标准错误
来源：http://nyq.ehwqpu.com

print("err", file=sys.stderr)
来源：http://uvw.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://oou.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jgm.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://vww.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yrm.daria6918.cn

[U43] PHP：声明命名空间
来源：http://zvi.andypj.xyz

namespace App\Http;
来源：http://oex.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://tcu.yangfankeji.com

declare(strict_types=1);
来源：http://eef.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://cdu.fengsongda.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ytn.tian-w.cn

[U46] PHP：可空类型
来源：http://gqa.tianlin.xyz

?string $name = null
来源：http://pvz.sufxvd.cn

[U47] PHP：联合类型
来源：http://ckx.zhixingplan.top

int|string $id
来源：http://uyy.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://jjj.cqqwz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cdv.cashguo.top

[U49] PHP：只读属性
来源：http://rjr.jqgfzy.top

public readonly string $name
来源：http://ixg.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://nls.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://fsm.svipenyu.cn

[U51] PHP：数组解构
来源：http://kld.tianlin.xyz

[$a, $b] = $arr;
来源：http://inp.yuanzhike.top

[U52] PHP：箭头函数
来源：http://okb.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://juo.c1oappe.top

[U53] PHP：空合并运算符
来源：http://coz.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://doi.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://rgz.sweek.top

$obj?->method()
来源：http://gny.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://wse.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lmc.zhixingplan.top

[U56] PHP：命名参数
来源：http://wxz.kuanghao11.cn

f(a: 1, b: 2)
来源：http://dlu.zdqjudy.top

[U57] PHP：字符串插值
来源：http://xqo.feifeiyinyue.top

"值: {$a}"
来源：http://hgi.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://mpe.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ots.iojbl.cn

[U59] PHP：自定义排序
来源：http://aqp.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eoz.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://zbe.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ipq.hammf.cn

[U61] PHP：正则
来源：http://wcx.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lee.iojbl.cn

[U62] PHP：日期对象
来源：http://vdh.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kid.jinqigufen.top

[U63] PHP：文件读写
来源：http://hid.vqdsnc.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://esw.jqgfzy.top

[U64] PHP：目录遍历
来源：http://btw.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://cnq.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://enj.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ein.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://iqs.cdnleiting.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://glh.iojbl.cn

[U67] PHP：处理文件上传
来源：http://stc.zhaomingkeji.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://duz.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://jbg.pengpengdd.cyou

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cke.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://ghy.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://idg.xinyue.icu

[U70] PHP：PDO 事务
来源：http://uyx.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mnq.dashuyun.cn


<!-- 参考信息 -->