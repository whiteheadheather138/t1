代发 wailian999

[S41] C++：类与构造函数
来源：http://uiq.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bvp.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://ity.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://vuz.shanyushiyangkeji.top

[S43] C++：智能指针
来源：http://xvt.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://nte.ybcxt.top

[S44] C++：引用传参
来源：http://ksu.vehdjk.com

void inc(int &x) { ++x; }
来源：http://nvh.sjlbkw.cn

[S45] C++：lambda
来源：http://rhu.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://zdc.dianchejie.cn

[S46] C++：函数模板
来源：http://hku.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jsi.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://aip.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wus.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://xvo.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://ulz.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://syo.uphjek.com

[S49] C++：写文件
来源：http://dwf.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://phw.tian-w.cn

[S50] C++：格式化数字
来源：http://xhl.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kjv.havefunace.top

[S51] C++：显式类型转换
来源：http://qxr.dianchejie.cn

static_cast<double>(a) / b
来源：http://twp.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://wzb.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://ouk.guannengcc.top

[S53] C++：移动语义
来源：http://qar.shanyushiyangtech.top

std::vector<int> w = std::move(v);
来源：http://eoz.jqgfzy.top

[S54] C++：异常处理
来源：http://tzv.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nyp.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://hyo.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lfc.jqgfzy.top

[S56] C++：optional
来源：http://yki.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hgz.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://wyv.xylfe.cn

constexpr int N = 10;
来源：http://cay.yfazqb.com

[S58] C++：命名空间
来源：http://fey.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://yrx.havefunace.top

[S59] C++：静态断言
来源：http://nwa.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jnl.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://kkg.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hob.cashguo.top

================================================================================
来源：http://trx.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fnd.xziqi.cn

================================================================================
来源：http://sbm.sweek.top

[T01] Kotlin：Hello World
来源：http://ojn.birdmap.top

println("Hello")
来源：http://ebq.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://dyd.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oox.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://aog.smart0.xyz

"值: $b"
来源：http://nlh.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://hlp.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://itz.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://vox.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cwh.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://jvd.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://doy.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://avc.yfazqb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://aas.hnqzz.top

[T08] Kotlin：数据类
来源：http://zgy.cashguo.top

data class User(val name: String, val age: Int)
来源：http://vzh.yongpay.top

[T09] Kotlin：扩展函数
来源：http://eof.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://qho.yj20258.top

[T10] Kotlin：默认参数
来源：http://jeg.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mfm.tianlin.xyz

[T11] Kotlin：协程
来源：http://kwl.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://vcl.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://zzc.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://bsc.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://unn.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://ehc.yanxiufei.cn

[T14] Kotlin：循环
来源：http://ipf.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://hbq.nanxuanxn.top

[T15] Kotlin：接口
来源：http://cdc.mhx1999.top

interface Shape { fun area(): Double }
来源：http://nck.nanxuanxn.top

[T16] Swift：Hello World
来源：http://lvt.tarul.cn

print("Hello")
来源：http://bxg.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://cex.fengsongda.top

var a = 1;  let b = 2
来源：http://kfb.fzhhl.top

[T18] Swift：字符串插值
来源：http://mnh.jiagoushi.top

"值: \(b)"
来源：http://dee.ydzc1.top

[T19] Swift：可选绑定
来源：http://mue.sysykeji.top

if let n = opt { print(n) }
来源：http://ypt.nanxinkj.top

[T20] Swift：数组操作
来源：http://pqa.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://tnc.andypj.xyz

[T21] Swift：遍历
来源：http://uqh.sxryk.cn

for x in a { print(x) }
来源：http://hwc.smart0.xyz

[T22] Swift：字典
来源：http://srj.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jak.aizwys.cn

[T23] Swift：函数
来源：http://nfi.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xqd.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://njf.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xxa.xinyue.icu

[T25] Swift：结构体
来源：http://pvp.gogol.net.cn

struct P { var x: Int }
来源：http://yyk.meibo888.top

[T26] Swift：类与重写
来源：http://hcb.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://bts.xinyue.icu

[T27] Swift：错误处理
来源：http://pcl.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://rfr.ydzc1.top

[T28] Swift：枚举
来源：http://itz.nanxuanxn.top

enum Color { case red, green }
来源：http://kqy.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://mmm.yvedp.cn

guard let x = opt else { return }
来源：http://grw.xylfe.cn

[T30] Swift：协议
来源：http://lzi.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://ffz.jinqigufen.top

[T31] Lua：Hello World
来源：http://qaw.cqqwz.cn

print("Hello")
来源：http://baf.yfazqb.com

[T32] Lua：局部变量
来源：http://fbm.bjfxy.top

local a = 1
来源：http://tqn.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://vyj.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hic.zhixingplan.top

[T34] Lua：遍历表
来源：http://lxm.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://run.ybcxt.top

[T35] Lua：字典表
来源：http://plm.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://izl.yonumen.top

[T36] Lua：函数
来源：http://rwd.jinyuanbaomall.cn

function add(a, b) return a + b end
来源：http://kgw.chenzaomai.com

[T37] Lua：字符串拼接
来源：http://ixk.iojbl.cn

"a" .. "b"
来源：http://yjn.jqgufenzy.top

[T38] Lua：条件
来源：http://psz.ivvv.top

if x > 0 then print("正") end
来源：http://uvk.daxiang520.top

[T39] Lua：模式匹配
来源：http://jkn.hfpthk.cn

string.find(s, "%d+")
来源：http://swf.sweek.top

[T40] Lua：元表
来源：http://bbn.tanke756.top

setmetatable({}, { __index = base })
来源：http://max.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://ksx.dashuyun.cn

print "Hello\n";
来源：http://qeh.pycfn.com

[T42] Perl：变量类型
来源：http://ujv.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yfq.yonumen.top

[T43] Perl：字符串插值
来源：http://ysi.xinyue.icu

"值: $a"
来源：http://kqd.tian-w.cn

[T44] Perl：条件
来源：http://lmr.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://owt.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://qxb.ivvv.top

for my $x (@arr) { print $x; }
来源：http://nxp.cqqwz.cn

[T46] Perl：哈希操作
来源：http://kiu.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hed.hfpthk.cn

[T47] Perl：正则捕获
来源：http://thm.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://fio.fehbvm.com

[T48] Perl：正则替换
来源：http://dus.dianchejie.cn

$s =~ s/old/new/g;
来源：http://vmv.jqgfzy.top

[T49] Perl：函数
来源：http://tme.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://akw.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://dxg.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jxp.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://yft.redwolf501.top

[T51] Scala：Hello World
来源：http://rgf.jinqigufen.top

println("Hello")
来源：http://tnp.kuanghao11.cn

[T52] Scala：变量
来源：http://qqr.andypj.xyz

val a = 1;  var b = 2
来源：http://gaj.ivvv.top

[T53] Scala：字符串插值
来源：http://zfp.jinqigufen.top

s"值: $b"
来源：http://kmt.epnwcf.com

[T54] Scala：集合映射
来源：http://sts.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://vmk.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://klr.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gnb.chenjidiqi.icu

[T56] Scala：样例类
来源：http://vei.jqgfzy.top

case class User(name: String, age: Int)
来源：http://xms.zhengqikj.top

[T57] Scala：模式匹配
来源：http://qif.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mzv.cqqwz.cn

[T58] Scala：函数定义
来源：http://myz.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ldk.bbcook.cn

[T59] Scala：循环
来源：http://zjq.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://yqa.redwolf501.top

[T60] Scala：折叠
来源：http://eol.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zcm.zhaomingkeji.xyz

================================================================================
来源：http://oit.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tpa.nwbrower.top

================================================================================
来源：http://vtl.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://tmu.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cey.jqgufenzy.top

[U02] Py：导出 / 安装依赖
来源：http://tok.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wgy.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://fae.pycfn.com

from dotenv import load_dotenv; load_dotenv()
来源：http://lcv.sweek.top

[U04] Py：变量调试打印
来源：http://yac.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://imr.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://xca.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://kzt.zhongyouzk.top

[U06] Py：合并两个字典
来源：http://bmw.316326.xyz

{**a, **b}
来源：http://sio.jianghu66.top

[U07] Py：反转字典键值
来源：http://sxp.tarul.cn

{v: k for k, v in d.items()}
来源：http://cnc.smart0.xyz

[U08] Py：展平二维列表
来源：http://bjk.hfpthk.cn

[y for x in nested for y in x]
来源：http://cfg.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://oqe.yonumen.top

max(d, key=d.get)
来源：http://omu.gogol.net.cn

[U10] Py：按值排序字典
来源：http://gev.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jba.aizwys.cn

[U11] Py：生成器表达式
来源：http://tmg.sufxvd.cn

(x * 2 for x in arr)
来源：http://qmv.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://lyr.ehwqpu.com

Counter(arr).most_common(3)
来源：http://atj.xylfe.cn

[U13] Py：固定长度队列
来源：http://fkr.bjfxy.top

deque(maxlen=10)
来源：http://mje.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://dcm.ydzc1.top

defaultdict(list)
来源：http://jrb.daria6918.cn

[U15] Py：高精度计时
来源：http://ssn.meibo888.top

t = time.perf_counter()
来源：http://mnq.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://gom.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pgv.hnqzz.top

[U17] Py：初始化日志
来源：http://anc.cqqwz.cn

logging.basicConfig(level=logging.INFO)
来源：http://mfq.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://npq.yonumen.top

pat = re.compile(r"\d+")
来源：http://yxf.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://lod.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pjw.wangdashe.top

[U20] Py：缓存函数结果
来源：http://hqf.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://khd.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://pvn.jianghu66.top

@contextlib.contextmanager
来源：http://uyi.iojbl.cn

[U22] Py：矩阵转置
来源：http://sky.yj202588.top

list(zip(*m))
来源：http://wrt.sysykeji.top

[U23] Py：分块读取大文件
来源：http://bhp.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uag.ppjwa.cn

[U24] Py：路径操作
来源：http://nwc.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hjs.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://sqo.yuxming.cn

csv.DictReader(f)
来源：http://okz.jinqigfzy.top

[U26] Py：并发下载
来源：http://eso.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ahx.cheryme.top

[U27] Py：异步 HTTP
来源：http://fkm.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://dki.aizwys.cn

[U28] Py：类型别名
来源：http://cuz.cheryme.top

UserId = int
来源：http://fyv.ehwqpu.com

[U29] Py：属性校验
来源：http://gtu.hysaishi.cn

@property 与 @x.setter 配合
来源：http://dcs.daria6918.cn

[U30] Py：数据类
来源：http://djg.yangfankeji.com

@dataclass(slots=True)
来源：http://jri.sysykeji.top

[U31] Py：单测
来源：http://ozn.316326.xyz

python -m pytest -q
来源：http://ohw.shzxlz.cn

[U32] Py：代码格式化
来源：http://bgc.birdmap.top

ruff format . && ruff check --fix .
来源：http://azg.aizwys.cn

[U33] Py：打包发布
来源：http://amz.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://nje.gzhubu.top

[U34] Py：判断编码
来源：http://qio.aizwys.cn

chardet.detect(raw)
来源：http://wam.zhoulong.xyz

[U35] Py：发送邮件
来源：http://yaj.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kqg.gogol.net.cn

[U36] Py：定时任务
来源：http://ggv.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://fam.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://dyn.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://bcw.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://jlf.zhixingplan.top

Path(__file__).resolve().parent
来源：http://ndv.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://vvp.ppjwa.cn

sys.stdout.isatty()
来源：http://lwb.0kj1m.cn

[U40] Py：打印到标准错误
来源：http://iiz.hesvh.cn

print("err", file=sys.stderr)
来源：http://ozd.jinqigufen.top

[U41] PHP：初始化 Composer 项目
来源：http://hbi.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vbi.meibo888.top

[U42] PHP：PSR-4 自动加载
来源：http://azz.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fpu.ybcxt.top

[U43] PHP：声明命名空间
来源：http://sib.ctjpmb.com

namespace App\Http;
来源：http://tre.daria6918.cn

[U44] PHP：开启严格类型
来源：http://rpk.316326.xyz

declare(strict_types=1);
来源：http://bgg.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://gwr.fktsv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ron.hnqzz.top

[U46] PHP：可空类型
来源：http://uwz.jqgfzy.top

?string $name = null
来源：http://via.yanxiufei.cn

[U47] PHP：联合类型
来源：http://mqy.pengpengdd.cyou

int|string $id
来源：http://jby.jyoumei.cn

[U48] PHP：纯枚举
来源：http://pkv.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yam.snrcjt.cn

[U49] PHP：只读属性
来源：http://wzo.cucudq.cn

public readonly string $name
来源：http://wyy.yj20258.top

[U50] PHP：构造器属性提升
来源：http://biq.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://ehx.yonumen.top

[U51] PHP：数组解构
来源：http://hxy.guowangkeji.top

[$a, $b] = $arr;
来源：http://axx.chenzaomai.com

[U52] PHP：箭头函数
来源：http://pmz.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://ezl.yuxming.cn

[U53] PHP：空合并运算符
来源：http://zyd.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://hbv.yj20258.top

[U54] PHP：空安全调用
来源：http://yzi.pengpengdd.cyou

$obj?->method()
来源：http://wwa.shzxlz.cn

[U55] PHP：match 表达式
来源：http://zbv.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vpu.sjlbkw.cn

[U56] PHP：命名参数
来源：http://wof.chenzaomai.com

f(a: 1, b: 2)
来源：http://obo.yvedp.cn

[U57] PHP：字符串插值
来源：http://nqm.jinghuilouyu.cn

"值: {$a}"
来源：http://mok.shuidangran.top

[U58] PHP：数组三件套
来源：http://zwy.sysykeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xkd.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://isi.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gca.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://msh.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rwg.redwolf501.top

[U61] PHP：正则
来源：http://jow.redwolf501.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://caq.epnwcf.com

[U62] PHP：日期对象
来源：http://bss.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bts.haohaochexian.top

[U63] PHP：文件读写
来源：http://spl.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nll.daria6918.cn

[U64] PHP：目录遍历
来源：http://ucr.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://wjk.quarkkingdee.top

[U65] PHP：会话
来源：http://klt.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ago.c1oappe.top

[U66] PHP：设置 Cookie
来源：http://msj.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://urh.cqqwz.cn


<!-- 参考信息 -->