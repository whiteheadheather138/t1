代发 wailian999

[S43] C++：智能指针
来源：http://qbj.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://vro.zdbjq.cn

[S44] C++：引用传参
来源：http://hyg.fengsongda.top

void inc(int &x) { ++x; }
来源：http://dmy.jlsjyb.cn

[S45] C++：lambda
来源：http://eqj.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://llt.9152youxi.cn

[S46] C++：函数模板
来源：http://aqr.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oyf.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://har.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dcp.vehdjk.com

[S48] C++：逐行读文件
来源：http://xhe.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gcv.yonumen.top

while (std::getline(in, line)) { }
来源：http://yfl.chenzaomai.com

[S49] C++：写文件
来源：http://vfy.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zhj.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://rcm.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tkj.pycfn.com

[S51] C++：显式类型转换
来源：http://pvp.ehwqpu.com

static_cast<double>(a) / b
来源：http://emc.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://nmu.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://ido.feifeiyinyue.top

[S53] C++：移动语义
来源：http://cco.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://dia.daria6918.cn

[S54] C++：异常处理
来源：http://qjq.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aqp.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://wef.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fcu.xuetiantiany.cn

[S56] C++：optional
来源：http://fbx.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jss.hesvh.cn

[S57] C++：编译期常量
来源：http://hwc.redwolf501.top

constexpr int N = 10;
来源：http://lmr.quarkkingdee.top

[S58] C++：命名空间
来源：http://xhp.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://clf.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://gtp.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ufs.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://kfy.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cbt.nanxuanxn.top

================================================================================
来源：http://zdu.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vhn.jinqigfzy.top

================================================================================
来源：http://wji.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://gfu.aibaodan.cn

println("Hello")
来源：http://lpx.jinqigufen.top

[T02] Kotlin：变量
来源：http://mhj.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yoo.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://wvq.bbcook.cn

"值: $b"
来源：http://ttn.zhixingplan.top

[T04] Kotlin：空安全
来源：http://trx.jiagoushi.top

val n: String? = null;  n?.length
来源：http://vwk.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://hpj.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uir.yonumen.top

[T06] Kotlin：集合映射
来源：http://zfw.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qtt.yj20258.top

[T07] Kotlin：集合过滤
来源：http://awc.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mmi.xylfe.cn

[T08] Kotlin：数据类
来源：http://ltf.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://rzg.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://xvm.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://mgq.tarul.cn

[T10] Kotlin：默认参数
来源：http://rwf.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://cvj.ctjpmb.com

[T11] Kotlin：协程
来源：http://xho.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hcc.fehbvm.com

[T12] Kotlin：解构声明
来源：http://cda.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://mmi.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://its.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://aqt.ydzc1.top

[T14] Kotlin：循环
来源：http://lri.jqgfzy.top

for (i in 1..10) println(i)
来源：http://byb.yuanzhike.top

[T15] Kotlin：接口
来源：http://yec.bbcook.cn

interface Shape { fun area(): Double }
来源：http://med.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://jfm.yfazqb.com

print("Hello")
来源：http://gkh.hcnkem.com

[T17] Swift：变量与常量
来源：http://gwq.hnqzz.top

var a = 1;  let b = 2
来源：http://vrn.hesvh.cn

[T18] Swift：字符串插值
来源：http://dgq.guowangkeji.top

"值: \(b)"
来源：http://jqv.ctjpmb.com

[T19] Swift：可选绑定
来源：http://lty.jqgufenzy.top

if let n = opt { print(n) }
来源：http://lys.yvedp.cn

[T20] Swift：数组操作
来源：http://kjy.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://thw.aizwys.cn

[T21] Swift：遍历
来源：http://uxx.xinyue.icu

for x in a { print(x) }
来源：http://syb.hywenlv.cn

[T22] Swift：字典
来源：http://boo.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://emd.jianghu66.top

[T23] Swift：函数
来源：http://ydr.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://enw.dashuyun.cn

[T24] Swift：闭包
来源：http://snu.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://cii.yuxming.cn

[T25] Swift：结构体
来源：http://ovs.chenzaomai.com

struct P { var x: Int }
来源：http://znx.shuidangran.top

[T26] Swift：类与重写
来源：http://kdf.sysykeji.top

class A: Base { override func f() {} }
来源：http://wkt.yueranfly.top

[T27] Swift：错误处理
来源：http://iva.yangfankeji.com

do { try f() } catch { print(error) }
来源：http://hsp.jianghu66.top

[T28] Swift：枚举
来源：http://kgy.yj202588.top

enum Color { case red, green }
来源：http://kew.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://yka.kuanghao11.cn

guard let x = opt else { return }
来源：http://uei.chenlongwang.top

[T30] Swift：协议
来源：http://yjd.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://zxr.yanxiufei.cn

[T31] Lua：Hello World
来源：http://hea.sxryk.cn

print("Hello")
来源：http://tsu.gzhubu.top

[T32] Lua：局部变量
来源：http://aek.hfpthk.cn

local a = 1
来源：http://zdn.gotoacloud.top

[T33] Lua：表（数组）
来源：http://bxc.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dvf.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://bps.kuanghao11.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mmt.yuanzhike.top

[T35] Lua：字典表
来源：http://inj.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://ddh.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://bgu.yuanzhike.top

function add(a, b) return a + b end
来源：http://wfl.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://zgj.sufxvd.cn

"a" .. "b"
来源：http://zmf.haohaochexian.top

[T38] Lua：条件
来源：http://sxz.fktsv.cn

if x > 0 then print("正") end
来源：http://fvc.birdmap.top

[T39] Lua：模式匹配
来源：http://cea.hysaishi.cn

string.find(s, "%d+")
来源：http://ves.pengpengdd.cyou

[T40] Lua：元表
来源：http://gmc.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://yyw.tianlin.xyz

[T41] Perl：Hello World
来源：http://cvv.jqgfzy.top

print "Hello\n";
来源：http://phu.nwbrower.top

[T42] Perl：变量类型
来源：http://ufa.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nrn.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://ffu.mhx1999.top

"值: $a"
来源：http://myf.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://hhz.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://wlu.tian-w.cn

[T45] Perl：数组遍历
来源：http://cou.cdnleiting.top

for my $x (@arr) { print $x; }
来源：http://ctn.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://ecq.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nos.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://uin.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nba.svipenyu.cn

[T48] Perl：正则替换
来源：http://alz.redwolf501.top

$s =~ s/old/new/g;
来源：http://eoi.ivvv.top

[T49] Perl：函数
来源：http://sya.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dfq.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://fjk.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://edm.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://ruc.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://lpk.yanxiufei.cn

println("Hello")
来源：http://vvz.ybcxt.top

[T52] Scala：变量
来源：http://gll.ctjpmb.com

val a = 1;  var b = 2
来源：http://irf.zdbjq.cn

[T53] Scala：字符串插值
来源：http://mpv.fzhhl.top

s"值: $b"
来源：http://dod.sysykeji.top

[T54] Scala：集合映射
来源：http://hcc.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://ypp.dashuyun.cn

[T55] Scala：集合过滤
来源：http://axk.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://veb.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://hgx.fanxiaobao.xyz

case class User(name: String, age: Int)
来源：http://puu.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://cov.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ysw.birdmap.top

[T58] Scala：函数定义
来源：http://dua.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://cpi.aizwys.cn

[T59] Scala：循环
来源：http://aph.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://zdt.yuanzhike.top

[T60] Scala：折叠
来源：http://eld.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cvu.hywenlv.cn

================================================================================
来源：http://znj.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hyv.tanke756.top

================================================================================
来源：http://qkq.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://prl.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://ibn.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://bek.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kbe.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://iyf.yj202588.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kzi.ehwqpu.com

[U04] Py：变量调试打印
来源：http://ybq.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dlx.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://qae.fehbvm.com

list(dict.fromkeys(arr))
来源：http://olr.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://syg.daria6918.cn

{**a, **b}
来源：http://ccn.fehbvm.com

[U07] Py：反转字典键值
来源：http://jag.yj20258888.top

{v: k for k, v in d.items()}
来源：http://hqs.ydzc1.top

[U08] Py：展平二维列表
来源：http://oyj.guowangkeji.top

[y for x in nested for y in x]
来源：http://sue.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://vqn.hcnkem.com

max(d, key=d.get)
来源：http://krd.xziqi.cn

[U10] Py：按值排序字典
来源：http://sai.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tfg.cheryme.top

[U11] Py：生成器表达式
来源：http://ler.fehbvm.com

(x * 2 for x in arr)
来源：http://ndh.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://szu.xziqi.cn

Counter(arr).most_common(3)
来源：http://iux.hfpthk.cn

[U13] Py：固定长度队列
来源：http://ipf.cucudq.cn

deque(maxlen=10)
来源：http://gos.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://zsj.zhengqikj.top

defaultdict(list)
来源：http://xcj.316326.xyz

[U15] Py：高精度计时
来源：http://mxu.gogol.net.cn

t = time.perf_counter()
来源：http://vgq.iojbl.cn

[U16] Py：命令行参数解析
来源：http://jht.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bvf.vehdjk.com

[U17] Py：初始化日志
来源：http://dne.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://ioi.cqqwz.cn

[U18] Py：预编译正则
来源：http://jzq.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://fml.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://kap.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zoa.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://vha.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://uxj.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://ajl.chenzaomai.com

@contextlib.contextmanager
来源：http://ptc.nanxinkj.top

[U22] Py：矩阵转置
来源：http://pln.cashguo.top

list(zip(*m))
来源：http://rjh.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://mtz.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xpl.vqdsnc.cn

[U24] Py：路径操作
来源：http://dpx.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jra.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://dfa.shanyushiyangkeji.top

csv.DictReader(f)
来源：http://cmi.aizwys.cn

[U26] Py：并发下载
来源：http://mlb.daxiang520.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pga.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://sec.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://wxc.0kj1m.cn

[U28] Py：类型别名
来源：http://try.shuidangran.top

UserId = int
来源：http://fdx.mhx1999.top

[U29] Py：属性校验
来源：http://lfq.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://zxz.xuetiantiany.cn

[U30] Py：数据类
来源：http://uan.yuanzhike.top

@dataclass(slots=True)
来源：http://bqg.zhongyouzk.top

[U31] Py：单测
来源：http://mdu.nanxinkj.top

python -m pytest -q
来源：http://pzh.xylfe.cn

[U32] Py：代码格式化
来源：http://ory.svipenyu.cn

ruff format . && ruff check --fix .
来源：http://ptv.hammf.cn

[U33] Py：打包发布
来源：http://dnw.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://keq.zdqjudy.top

[U34] Py：判断编码
来源：http://atr.zhijiandao.cn

chardet.detect(raw)
来源：http://ukt.nwbrower.top

[U35] Py：发送邮件
来源：http://aep.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rjq.daxiang520.top

[U36] Py：定时任务
来源：http://rsy.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://fgy.mhx1999.top

[U37] Py：读写 Excel
来源：http://hik.gaohongyu789.top

pandas.read_excel / DataFrame.to_excel
来源：http://wbc.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://dqq.fzhhl.top

Path(__file__).resolve().parent
来源：http://wwa.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://coa.dashuyun.cn

sys.stdout.isatty()
来源：http://isx.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://vwz.aizwys.cn

print("err", file=sys.stderr)
来源：http://tft.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://roc.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pzs.tarul.cn

[U42] PHP：PSR-4 自动加载
来源：http://wxm.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pex.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://mnw.xylfe.cn

namespace App\Http;
来源：http://jzs.uphjek.com

[U44] PHP：开启严格类型
来源：http://egv.dashuyun.cn

declare(strict_types=1);
来源：http://fzs.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://fxq.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zkj.wangdashe.top

[U46] PHP：可空类型
来源：http://ysh.zhixingplan.top

?string $name = null
来源：http://fis.yvedp.cn

[U47] PHP：联合类型
来源：http://sry.jiagoushi.top

int|string $id
来源：http://imc.daxiang520.top

[U48] PHP：纯枚举
来源：http://kzu.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://csc.havefunace.top

[U49] PHP：只读属性
来源：http://eam.ywan-chungtsiang.top

public readonly string $name
来源：http://tzo.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://sgh.sjlbkw.cn

public function __construct(private int $id) {}
来源：http://pcj.zhongyouzk.top

[U51] PHP：数组解构
来源：http://apz.9152youxi.cn

[$a, $b] = $arr;
来源：http://ohz.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://xtg.ehwqpu.com

$double = fn($x) => $x * 2;
来源：http://gyu.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://hvq.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://esw.ydzc1.top

[U54] PHP：空安全调用
来源：http://wry.ywan-chungtsiang.top

$obj?->method()
来源：http://riq.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://gdz.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nce.gotoacloud.top

[U56] PHP：命名参数
来源：http://ier.zhoulong.xyz

f(a: 1, b: 2)
来源：http://qdb.zhixingplan.top

[U57] PHP：字符串插值
来源：http://efe.cucudq.cn

"值: {$a}"
来源：http://nwq.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://nes.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://geu.zdqjudy.top

[U59] PHP：自定义排序
来源：http://tek.gzhubu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sek.ivvv.top

[U60] PHP：JSON 编解码
来源：http://xuq.52xcode.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gpd.dianchejie.cn

[U61] PHP：正则
来源：http://nbt.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://edk.sweek.top

[U62] PHP：日期对象
来源：http://zvg.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hrz.ywan-chungtsiang.top

[U63] PHP：文件读写
来源：http://ijj.xingfuxueyuan.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cux.zhiwuduotai.top

[U64] PHP：目录遍历
来源：http://ufo.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://peq.zhiwuduotai.top

[U65] PHP：会话
来源：http://fxl.wangshuangyany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hqi.sxryk.cn

[U66] PHP：设置 Cookie
来源：http://tfm.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mlo.yj20258888.top

[U67] PHP：处理文件上传
来源：http://ioe.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yzj.c1oappe.top

[U68] PHP：PDO 连接
来源：http://yfa.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fdm.shanyushiyangkeji.top


<!-- 参考信息 -->