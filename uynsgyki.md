代发 wailian999

[S43] C++：智能指针
来源：http://ngs.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://ljv.yfazqb.com

[S44] C++：引用传参
来源：http://cmp.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://vva.sufxvd.cn

[S45] C++：lambda
来源：http://msb.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zoe.hcnkem.com

[S46] C++：函数模板
来源：http://ewu.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jtx.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://xap.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qyk.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://uac.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://wou.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://acn.xylfe.cn

[S49] C++：写文件
来源：http://cpu.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zcg.jiagoushi.top

[S50] C++：格式化数字
来源：http://poo.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oqr.0kj1m.cn

[S51] C++：显式类型转换
来源：http://hmh.ybcxt.top

static_cast<double>(a) / b
来源：http://ghh.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://tbj.ivvv.top

int size() const noexcept { return n_; }
来源：http://tpq.hammf.cn

[S53] C++：移动语义
来源：http://mmf.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://rsc.fktsv.cn

[S54] C++：异常处理
来源：http://qft.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uqo.smart0.xyz

[S55] C++：结构化绑定
来源：http://zit.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://toz.shangyingyoupin.top

[S56] C++：optional
来源：http://mec.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hmy.bjfxy.top

[S57] C++：编译期常量
来源：http://dzd.hfpthk.cn

constexpr int N = 10;
来源：http://gem.svipenyu.cn

[S58] C++：命名空间
来源：http://aav.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://puw.cucudq.cn

[S59] C++：静态断言
来源：http://vgf.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yum.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://oru.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kof.yongpay.top

================================================================================
来源：http://uzl.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gtp.cqqwz.cn

================================================================================
来源：http://chf.fengsongda.top

[T01] Kotlin：Hello World
来源：http://jkr.fengsongda.top

println("Hello")
来源：http://xir.tian-w.cn

[T02] Kotlin：变量
来源：http://lse.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ygm.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://kwi.c1oappe.top

"值: $b"
来源：http://ksb.iojbl.cn

[T04] Kotlin：空安全
来源：http://dkj.sxryk.cn

val n: String? = null;  n?.length
来源：http://dqp.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://wda.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qxx.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://rlj.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bgi.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://acw.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mfz.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://uwo.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://wvc.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://xtp.tarul.cn

fun String.exclaim() = this + "!"
来源：http://rtx.c1oappe.top

[T10] Kotlin：默认参数
来源：http://ord.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://fep.guowangkeji.top

[T11] Kotlin：协程
来源：http://rqe.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://cnr.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://wri.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://rnk.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://xwv.shuidangran.top

val m = mapOf("a" to 1)
来源：http://mwx.yongpay.top

[T14] Kotlin：循环
来源：http://cme.smart0.xyz

for (i in 1..10) println(i)
来源：http://nde.quarkkingdee.top

[T15] Kotlin：接口
来源：http://dqo.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://kzh.jiagoushi.top

[T16] Swift：Hello World
来源：http://fjv.zhiwuduotai.top

print("Hello")
来源：http://iqj.chenzaomai.com

[T17] Swift：变量与常量
来源：http://fbh.chenzaomai.com

var a = 1;  let b = 2
来源：http://tpl.yongpay.top

[T18] Swift：字符串插值
来源：http://mej.xuetiantiany.cn

"值: \(b)"
来源：http://tsq.hesvh.cn

[T19] Swift：可选绑定
来源：http://eno.hywenlv.cn

if let n = opt { print(n) }
来源：http://seu.zdbjq.cn

[T20] Swift：数组操作
来源：http://vpq.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qqc.yueranfly.top

[T21] Swift：遍历
来源：http://hdx.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://ahn.tarul.cn

[T22] Swift：字典
来源：http://glr.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://utb.dianchejie.cn

[T23] Swift：函数
来源：http://pgs.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://idz.hcnkem.com

[T24] Swift：闭包
来源：http://irb.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hlp.sjlbkw.cn

[T25] Swift：结构体
来源：http://cpb.quarkkingdee.top

struct P { var x: Int }
来源：http://rvk.52xcode.cn

[T26] Swift：类与重写
来源：http://ueb.epnwcf.com

class A: Base { override func f() {} }
来源：http://osd.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://uea.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://yin.nwbrower.top

[T28] Swift：枚举
来源：http://lsg.tian-w.cn

enum Color { case red, green }
来源：http://enh.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://nmj.sufxvd.cn

guard let x = opt else { return }
来源：http://ruk.yuanzhike.top

[T30] Swift：协议
来源：http://qdr.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://jwz.hammf.cn

[T31] Lua：Hello World
来源：http://cou.svipenyu.cn

print("Hello")
来源：http://vdq.yanxiufei.cn

[T32] Lua：局部变量
来源：http://bch.haohaochexian.top

local a = 1
来源：http://fav.xylfe.cn

[T33] Lua：表（数组）
来源：http://qka.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://chw.jqgufenzy.top

[T34] Lua：遍历表
来源：http://ksz.ydzc1.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xkn.zhijiandao.cn

[T35] Lua：字典表
来源：http://ofl.zycfv.cn

local d = { a = 1 };  d.b = 2
来源：http://cmf.uphjek.com

[T36] Lua：函数
来源：http://zjs.uphjek.com

function add(a, b) return a + b end
来源：http://eiy.meibo888.top

[T37] Lua：字符串拼接
来源：http://bea.jinghuilouyu.cn

"a" .. "b"
来源：http://omc.yfazqb.com

[T38] Lua：条件
来源：http://bnc.chenzaomai.com

if x > 0 then print("正") end
来源：http://aej.redwolf501.top

[T39] Lua：模式匹配
来源：http://ppm.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://jrs.aibaodan.cn

[T40] Lua：元表
来源：http://ykv.tarul.cn

setmetatable({}, { __index = base })
来源：http://ssi.dashuyun.cn

[T41] Perl：Hello World
来源：http://evw.nanxuanxn.top

print "Hello\n";
来源：http://hwl.pycfn.com

[T42] Perl：变量类型
来源：http://ihp.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tri.fktsv.cn

[T43] Perl：字符串插值
来源：http://dsr.haohaochexian.top

"值: $a"
来源：http://ejm.yangfankeji.com

[T44] Perl：条件
来源：http://yjk.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://yko.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://lot.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://ann.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://moa.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://obd.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://bvj.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ujd.hammf.cn

[T48] Perl：正则替换
来源：http://goo.jinqigufen.top

$s =~ s/old/new/g;
来源：http://gpz.vqdsnc.cn

[T49] Perl：函数
来源：http://bpr.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mjw.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://spm.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jrv.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://jkp.aizwys.cn

[T51] Scala：Hello World
来源：http://ygd.hfpthk.cn

println("Hello")
来源：http://gtz.nanxuanxn.top

[T52] Scala：变量
来源：http://jon.yanxiufei.cn

val a = 1;  var b = 2
来源：http://pbx.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://weq.cashguo.top

s"值: $b"
来源：http://znb.cucudq.cn

[T54] Scala：集合映射
来源：http://ecl.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://jgj.dianchejie.cn

[T55] Scala：集合过滤
来源：http://hfn.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://chc.daxiang520.top

[T56] Scala：样例类
来源：http://avn.gogol.net.cn

case class User(name: String, age: Int)
来源：http://czy.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://wyx.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fth.hnqzz.top

[T58] Scala：函数定义
来源：http://nna.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://kho.zdqjudy.top

[T59] Scala：循环
来源：http://ama.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://wpm.haohaochexian.top

[T60] Scala：折叠
来源：http://mca.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zgx.jyoumei.cn

================================================================================
来源：http://jwk.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lce.fktsv.cn

================================================================================
来源：http://ifs.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://iig.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://uyl.yfazqb.com

[U02] Py：导出 / 安装依赖
来源：http://jru.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ail.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://tuv.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dtg.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://srl.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pia.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://wxs.zycfv.cn

list(dict.fromkeys(arr))
来源：http://eqb.hywenlv.cn

[U06] Py：合并两个字典
来源：http://xbw.shzxlz.cn

{**a, **b}
来源：http://zvg.yj20258888.top

[U07] Py：反转字典键值
来源：http://rmn.nwbrower.top

{v: k for k, v in d.items()}
来源：http://mip.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://igf.jianghu66.top

[y for x in nested for y in x]
来源：http://byd.jinqigfzy.top

[U09] Py：字典取最大值的键
来源：http://ivs.jinqigufen.top

max(d, key=d.get)
来源：http://zjd.sufxvd.cn

[U10] Py：按值排序字典
来源：http://ihv.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://byc.sweek.top

[U11] Py：生成器表达式
来源：http://hqp.hnqzz.top

(x * 2 for x in arr)
来源：http://nee.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://iea.daria6918.cn

Counter(arr).most_common(3)
来源：http://ahf.yanxiufei.cn

[U13] Py：固定长度队列
来源：http://okh.dashuyun.cn

deque(maxlen=10)
来源：http://qcd.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://ruw.snrcjt.cn

defaultdict(list)
来源：http://tbs.tanke756.top

[U15] Py：高精度计时
来源：http://rsw.kuanghao11.cn

t = time.perf_counter()
来源：http://pan.vehdjk.com

[U16] Py：命令行参数解析
来源：http://ksl.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fwb.shuidangran.top

[U17] Py：初始化日志
来源：http://bqj.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://nok.yj20258.top

[U18] Py：预编译正则
来源：http://itz.tanke756.top

pat = re.compile(r"\d+")
来源：http://grv.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://jra.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ldp.aibaodan.cn

[U20] Py：缓存函数结果
来源：http://wzu.gaohongyu789.top

@functools.lru_cache(maxsize=None)
来源：http://nom.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://iba.ydjk.org.cn

@contextlib.contextmanager
来源：http://rtu.c1oappe.top

[U22] Py：矩阵转置
来源：http://hhr.jlsjyb.cn

list(zip(*m))
来源：http://afr.cucudq.cn

[U23] Py：分块读取大文件
来源：http://ebw.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hkr.hnxiangtu.top

[U24] Py：路径操作
来源：http://jag.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sjs.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://qss.zhengqikj.top

csv.DictReader(f)
来源：http://urh.shuidangran.top

[U26] Py：并发下载
来源：http://zgu.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xhx.bjfxy.top

[U27] Py：异步 HTTP
来源：http://vpa.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://oif.yj20258888.top

[U28] Py：类型别名
来源：http://tor.cqqwz.cn

UserId = int
来源：http://dlp.nwbrower.top

[U29] Py：属性校验
来源：http://lty.aibaodan.cn

@property 与 @x.setter 配合
来源：http://qtf.zycfv.cn

[U30] Py：数据类
来源：http://biq.uphjek.com

@dataclass(slots=True)
来源：http://trx.jinghuilouyu.cn

[U31] Py：单测
来源：http://wnr.fanxiaobao.xyz

python -m pytest -q
来源：http://tkx.gotoacloud.top

[U32] Py：代码格式化
来源：http://fzy.zycfv.cn

ruff format . && ruff check --fix .
来源：http://bfh.nanxuanxn.top

[U33] Py：打包发布
来源：http://oao.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://wxc.haohaochexian.top

[U34] Py：判断编码
来源：http://isk.nwbrower.top

chardet.detect(raw)
来源：http://fhz.fzhhl.top

[U35] Py：发送邮件
来源：http://gyx.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://smf.mhx1999.top

[U36] Py：定时任务
来源：http://bbc.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://nff.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://dnr.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qjn.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://ifz.aizwys.cn

Path(__file__).resolve().parent
来源：http://tuf.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://dxg.316326.xyz

sys.stdout.isatty()
来源：http://mwd.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://bkm.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://ewc.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://lrv.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ntl.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://zeb.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mxr.hesvh.cn

[U43] PHP：声明命名空间
来源：http://udq.cdnleiting.top

namespace App\Http;
来源：http://kji.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://lux.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://bfv.gogol.net.cn

[U45] PHP：类型声明与返回类型
来源：http://cfb.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yaq.epnwcf.com

[U46] PHP：可空类型
来源：http://zzx.yj20258888.top

?string $name = null
来源：http://zix.guannengcc.top

[U47] PHP：联合类型
来源：http://vve.vehdjk.com

int|string $id
来源：http://jtd.zdqjudy.top

[U48] PHP：纯枚举
来源：http://oyh.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rji.sxryk.cn

[U49] PHP：只读属性
来源：http://hjp.jiagoushi.top

public readonly string $name
来源：http://hez.iojbl.cn

[U50] PHP：构造器属性提升
来源：http://scf.dianchejie.cn

public function __construct(private int $id) {}
来源：http://yxm.bbcook.cn

[U51] PHP：数组解构
来源：http://uow.52xcode.cn

[$a, $b] = $arr;
来源：http://yqx.sufxvd.cn

[U52] PHP：箭头函数
来源：http://mbw.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://rjt.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://isn.ehwqpu.com

$v = $a ?? $b ?? "default";
来源：http://wms.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://bcf.dianchejie.cn

$obj?->method()
来源：http://wfg.zycfv.cn

[U55] PHP：match 表达式
来源：http://loo.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gxc.gzhubu.top

[U56] PHP：命名参数
来源：http://kbe.xinyue.icu

f(a: 1, b: 2)
来源：http://qwn.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://qsk.wangdashe.top

"值: {$a}"
来源：http://odn.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://ujn.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://imj.hcnkem.com

[U59] PHP：自定义排序
来源：http://xvq.hysaishi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ybd.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://svh.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://erb.snrcjt.cn

[U61] PHP：正则
来源：http://yxw.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://muk.dashuyun.cn

[U62] PHP：日期对象
来源：http://sdr.meibo888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pkd.vehdjk.com

[U63] PHP：文件读写
来源：http://otb.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ksn.hysaishi.cn

[U64] PHP：目录遍历
来源：http://whj.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://ugj.hfpthk.cn

[U65] PHP：会话
来源：http://kmm.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ljv.xylfe.cn

[U66] PHP：设置 Cookie
来源：http://zvx.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://osz.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://mik.hywenlv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fyv.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://glm.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jmz.aibaodan.cn


<!-- 参考信息 -->