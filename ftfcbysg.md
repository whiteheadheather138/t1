代发 wailian999

[S45] C++：lambda
来源：http://swl.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xpk.gogol.net.cn

[S46] C++：函数模板
来源：http://taf.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ohd.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://oww.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hgf.hywenlv.cn

[S48] C++：逐行读文件
来源：http://ayy.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://mfb.fktsv.cn

while (std::getline(in, line)) { }
来源：http://vba.yuanzhike.top

[S49] C++：写文件
来源：http://pma.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oup.yonumen.top

[S50] C++：格式化数字
来源：http://mmd.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gou.c1oappe.top

[S51] C++：显式类型转换
来源：http://jwy.zhixingplan.top

static_cast<double>(a) / b
来源：http://fjq.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://fvq.havefunace.top

int size() const noexcept { return n_; }
来源：http://rxn.316326.xyz

[S53] C++：移动语义
来源：http://nmo.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://ffb.nanxuanxn.top

[S54] C++：异常处理
来源：http://uqq.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://odw.redwolf501.top

[S55] C++：结构化绑定
来源：http://zzu.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://osh.mhx1999.top

[S56] C++：optional
来源：http://wrm.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rfc.zhongyouzk.top

[S57] C++：编译期常量
来源：http://kud.ehwqpu.com

constexpr int N = 10;
来源：http://rpv.0kj1m.cn

[S58] C++：命名空间
来源：http://lyb.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://yyy.0kj1m.cn

[S59] C++：静态断言
来源：http://xyu.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jha.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://wsu.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xbi.uphjek.com

================================================================================
来源：http://gmw.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fmb.havefunace.top

================================================================================
来源：http://xyv.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://ywi.52xcode.cn

println("Hello")
来源：http://ezq.zhongyouzk.top

[T02] Kotlin：变量
来源：http://tha.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gzu.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://yku.daria6918.cn

"值: $b"
来源：http://gio.pycfn.com

[T04] Kotlin：空安全
来源：http://geh.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://vlc.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://swg.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hne.havefunace.top

[T06] Kotlin：集合映射
来源：http://exm.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kms.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://lig.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kpc.dashuyun.cn

[T08] Kotlin：数据类
来源：http://obn.cashguo.top

data class User(val name: String, val age: Int)
来源：http://ngg.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://ntk.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://ctf.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://qfx.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ezg.zhongyouzk.top

[T11] Kotlin：协程
来源：http://gak.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vys.cheryme.top

[T12] Kotlin：解构声明
来源：http://qwe.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://umc.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://tbl.sysykeji.top

val m = mapOf("a" to 1)
来源：http://nyf.meibo888.top

[T14] Kotlin：循环
来源：http://eqi.jinqigfzy.top

for (i in 1..10) println(i)
来源：http://rfm.zhijiandao.cn

[T15] Kotlin：接口
来源：http://kkk.fehbvm.com

interface Shape { fun area(): Double }
来源：http://qss.jianghu66.top

[T16] Swift：Hello World
来源：http://tvr.cucudq.cn

print("Hello")
来源：http://qjc.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://kwa.hcnkem.com

var a = 1;  let b = 2
来源：http://iot.ctjpmb.com

[T18] Swift：字符串插值
来源：http://ewl.svipenyu.cn

"值: \(b)"
来源：http://xgg.yj20258.top

[T19] Swift：可选绑定
来源：http://iap.ehwqpu.com

if let n = opt { print(n) }
来源：http://uga.haohaochexian.top

[T20] Swift：数组操作
来源：http://ieh.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://yql.chenzaomai.com

[T21] Swift：遍历
来源：http://vfx.c1oappe.top

for x in a { print(x) }
来源：http://pwg.cucudq.cn

[T22] Swift：字典
来源：http://gyl.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://gwm.dashuyun.cn

[T23] Swift：函数
来源：http://mig.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://knc.fktsv.cn

[T24] Swift：闭包
来源：http://clp.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vxu.cashguo.top

[T25] Swift：结构体
来源：http://tdl.tianlin.xyz

struct P { var x: Int }
来源：http://vdv.yonumen.top

[T26] Swift：类与重写
来源：http://ebu.fengsongda.top

class A: Base { override func f() {} }
来源：http://khg.daxiang520.top

[T27] Swift：错误处理
来源：http://bne.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://vef.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://dpq.pengpengdd.cyou

enum Color { case red, green }
来源：http://fno.xuetiantiany.cn

[T29] Swift：guard 提前返回
来源：http://mzf.jiagoushi.top

guard let x = opt else { return }
来源：http://qcg.jinqigufen.top

[T30] Swift：协议
来源：http://qqf.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://vsz.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://xjm.ydjk.org.cn

print("Hello")
来源：http://fim.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://edw.ppjwa.cn

local a = 1
来源：http://aeo.ivvv.top

[T33] Lua：表（数组）
来源：http://vda.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ycc.zhijiandao.cn

[T34] Lua：遍历表
来源：http://hsg.jianghu66.top

for i, v in ipairs(t) do print(i, v) end
来源：http://llc.birdmap.top

[T35] Lua：字典表
来源：http://pku.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://jqs.gzhubu.top

[T36] Lua：函数
来源：http://pqz.nanxuanxn.top

function add(a, b) return a + b end
来源：http://qgf.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://rsz.cqqwz.cn

"a" .. "b"
来源：http://bwm.hywenlv.cn

[T38] Lua：条件
来源：http://tkh.316326.xyz

if x > 0 then print("正") end
来源：http://iqq.smart0.xyz

[T39] Lua：模式匹配
来源：http://itm.yuxming.cn

string.find(s, "%d+")
来源：http://kxc.dashuyun.cn

[T40] Lua：元表
来源：http://zlh.jqgufenzy.top

setmetatable({}, { __index = base })
来源：http://kbw.zycfv.cn

[T41] Perl：Hello World
来源：http://eoc.xuanzx.com

print "Hello\n";
来源：http://ryw.yfazqb.com

[T42] Perl：变量类型
来源：http://pgs.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tau.chenzaomai.com

[T43] Perl：字符串插值
来源：http://ksg.hysaishi.cn

"值: $a"
来源：http://qnb.9152youxi.cn

[T44] Perl：条件
来源：http://hav.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://efr.uphjek.com

[T45] Perl：数组遍历
来源：http://uxy.fktsv.cn

for my $x (@arr) { print $x; }
来源：http://sza.sysykeji.top

[T46] Perl：哈希操作
来源：http://qts.gzhubu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sct.jinqigufen.top

[T47] Perl：正则捕获
来源：http://gyx.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dhk.bjfxy.top

[T48] Perl：正则替换
来源：http://zll.hnqzz.top

$s =~ s/old/new/g;
来源：http://hpg.ctjpmb.com

[T49] Perl：函数
来源：http://urw.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pwm.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://pmo.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ojt.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://gkq.yfazqb.com

[T51] Scala：Hello World
来源：http://ugv.haohaochexian.top

println("Hello")
来源：http://cil.gogol.net.cn

[T52] Scala：变量
来源：http://tjy.jyoumei.cn

val a = 1;  var b = 2
来源：http://rpm.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://doz.316326.xyz

s"值: $b"
来源：http://ivp.zhixingplan.top

[T54] Scala：集合映射
来源：http://jie.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://pjq.cashguo.top

[T55] Scala：集合过滤
来源：http://eas.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://aph.guowangkeji.top

[T56] Scala：样例类
来源：http://liy.smart0.xyz

case class User(name: String, age: Int)
来源：http://mdy.sweek.top

[T57] Scala：模式匹配
来源：http://wqb.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://inb.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://oxp.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://hqo.aibaodan.cn

[T59] Scala：循环
来源：http://gzn.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://zka.jianghu66.top

[T60] Scala：折叠
来源：http://nax.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ayq.hesvh.cn

================================================================================
来源：http://qqe.xziqi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iuk.fehbvm.com

================================================================================
来源：http://yvk.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://mlm.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://ksv.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://ger.meibo888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://diu.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://rnk.sweek.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ogl.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://fgu.zycfv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ntb.chenzaomai.com

[U05] Py：列表去重且保序
来源：http://nfm.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://oed.tianlin.xyz

[U06] Py：合并两个字典
来源：http://dnq.sweek.top

{**a, **b}
来源：http://hbx.hammf.cn

[U07] Py：反转字典键值
来源：http://xsw.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://swl.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://dov.nanxuanxn.top

[y for x in nested for y in x]
来源：http://peh.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://iwf.sxryk.cn

max(d, key=d.get)
来源：http://bxr.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://ayo.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rmn.fengsongda.top

[U11] Py：生成器表达式
来源：http://szq.cucudq.cn

(x * 2 for x in arr)
来源：http://pej.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://ugm.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://bez.andypj.xyz

[U13] Py：固定长度队列
来源：http://rvg.yvedp.cn

deque(maxlen=10)
来源：http://pfr.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://tph.jinqigufen.top

defaultdict(list)
来源：http://gyd.jyoumei.cn

[U15] Py：高精度计时
来源：http://noi.uphjek.com

t = time.perf_counter()
来源：http://itf.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://iml.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://svq.yanxiufei.cn

[U17] Py：初始化日志
来源：http://bbc.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://vxl.gotoacloud.top

[U18] Py：预编译正则
来源：http://yax.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://abf.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://wmf.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pog.sjlbkw.cn

[U20] Py：缓存函数结果
来源：http://xoq.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://zud.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://tfb.snrcjt.cn

@contextlib.contextmanager
来源：http://eph.tianlin.xyz

[U22] Py：矩阵转置
来源：http://dnp.fengsongda.top

list(zip(*m))
来源：http://sdx.xylfe.cn

[U23] Py：分块读取大文件
来源：http://ijo.zhoulong.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iab.mhx1999.top

[U24] Py：路径操作
来源：http://oyg.haohaochexian.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jid.sysykeji.top

[U25] Py：CSV 按字典读
来源：http://sws.iojbl.cn

csv.DictReader(f)
来源：http://yvn.yanxiufei.cn

[U26] Py：并发下载
来源：http://dyq.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://auq.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://hcl.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://pfi.jinghuilouyu.cn

[U28] Py：类型别名
来源：http://eoi.yfazqb.com

UserId = int
来源：http://stx.nanxuanxn.top

[U29] Py：属性校验
来源：http://smx.snrcjt.cn

@property 与 @x.setter 配合
来源：http://xay.yj20258888.top

[U30] Py：数据类
来源：http://kzh.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://fvd.zdbjq.cn

[U31] Py：单测
来源：http://dkc.feifeiyinyue.top

python -m pytest -q
来源：http://vhz.bjfxy.top

[U32] Py：代码格式化
来源：http://qdy.bbcook.cn

ruff format . && ruff check --fix .
来源：http://nzc.tarul.cn

[U33] Py：打包发布
来源：http://ymv.pengpengdd.cyou

python -m build  （依赖 pyproject.toml）
来源：http://tku.yj20258.top

[U34] Py：判断编码
来源：http://gyv.ctjpmb.com

chardet.detect(raw)
来源：http://mgs.jinqigfzy.top

[U35] Py：发送邮件
来源：http://qyi.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ixo.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://mtx.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://izy.meibo888.top

[U37] Py：读写 Excel
来源：http://xqj.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://ppg.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://caf.ybcxt.top

Path(__file__).resolve().parent
来源：http://afg.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://wjy.zhiwuduotai.top

sys.stdout.isatty()
来源：http://ain.xziqi.cn

[U40] Py：打印到标准错误
来源：http://mwd.fktsv.cn

print("err", file=sys.stderr)
来源：http://lvy.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://lyb.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://xbi.jinghuilouyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://twx.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tpf.yj20258888.top

[U43] PHP：声明命名空间
来源：http://ypg.jinghuilouyu.cn

namespace App\Http;
来源：http://gqh.ydjk.org.cn

[U44] PHP：开启严格类型
来源：http://hqb.yongpay.top

declare(strict_types=1);
来源：http://ufb.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://elv.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xcg.nwbrower.top

[U46] PHP：可空类型
来源：http://pfv.havefunace.top

?string $name = null
来源：http://bun.c1oappe.top

[U47] PHP：联合类型
来源：http://wim.yj20258888.top

int|string $id
来源：http://gxd.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://jil.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ana.hnxiangtu.top

[U49] PHP：只读属性
来源：http://usr.yvedp.cn

public readonly string $name
来源：http://oio.tarul.cn

[U50] PHP：构造器属性提升
来源：http://hmu.daria6918.cn

public function __construct(private int $id) {}
来源：http://flb.hesvh.cn

[U51] PHP：数组解构
来源：http://elq.yongpay.top

[$a, $b] = $arr;
来源：http://kmt.fanxiaobao.xyz

[U52] PHP：箭头函数
来源：http://szn.tanke756.top

$double = fn($x) => $x * 2;
来源：http://rhm.guannengcc.top

[U53] PHP：空合并运算符
来源：http://htt.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://eje.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://eqt.0kj1m.cn

$obj?->method()
来源：http://tnu.yfazqb.com

[U55] PHP：match 表达式
来源：http://meu.guannengcc.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wst.jqgfzy.top

[U56] PHP：命名参数
来源：http://rpo.52xcode.cn

f(a: 1, b: 2)
来源：http://erm.316326.xyz

[U57] PHP：字符串插值
来源：http://wxg.kuanghao11.cn

"值: {$a}"
来源：http://xnw.jinqigufen.top

[U58] PHP：数组三件套
来源：http://nup.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ihr.gotoacloud.top

[U59] PHP：自定义排序
来源：http://run.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://srk.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://xaz.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mqf.bbcook.cn

[U61] PHP：正则
来源：http://bbj.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dhm.yj20258888.top

[U62] PHP：日期对象
来源：http://fzg.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://htl.iojbl.cn

[U63] PHP：文件读写
来源：http://zkz.52xcode.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://clp.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://bgq.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://klq.316326.xyz

[U65] PHP：会话
来源：http://yat.jinghuilouyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dol.yonumen.top

[U66] PHP：设置 Cookie
来源：http://cir.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://whl.ydzc1.top

[U67] PHP：处理文件上传
来源：http://suy.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ojl.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://rig.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://syu.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://oap.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pyw.wangdashe.top

[U70] PHP：PDO 事务
来源：http://hjp.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://onb.iojbl.cn


<!-- 参考信息 -->