代发 wailian999

[S41] C++：类与构造函数
来源：http://plb.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zkb.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://voe.zhengqikj.top

class B : public Base { public: void f() override {} };
来源：http://lck.jinqigufen.top

[S43] C++：智能指针
来源：http://jue.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://mgz.chenlongwang.top

[S44] C++：引用传参
来源：http://ybs.birdmap.top

void inc(int &x) { ++x; }
来源：http://ozr.zhiwuduotai.top

[S45] C++：lambda
来源：http://vyf.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://fiq.hfpthk.cn

[S46] C++：函数模板
来源：http://cjm.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xjv.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://isu.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mpk.aibaodan.cn

[S48] C++：逐行读文件
来源：http://blx.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wju.yongpay.top

while (std::getline(in, line)) { }
来源：http://kjm.andypj.xyz

[S49] C++：写文件
来源：http://kku.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mnp.zdbjq.cn

[S50] C++：格式化数字
来源：http://afh.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vuv.aibaodan.cn

[S51] C++：显式类型转换
来源：http://pte.pycfn.com

static_cast<double>(a) / b
来源：http://awv.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://epl.epnwcf.com

int size() const noexcept { return n_; }
来源：http://wfp.hfpthk.cn

[S53] C++：移动语义
来源：http://kcg.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://dau.zdbjq.cn

[S54] C++：异常处理
来源：http://yfs.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nrx.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://cvg.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://spz.haohaochexian.top

[S56] C++：optional
来源：http://tbo.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mps.tianlin.xyz

[S57] C++：编译期常量
来源：http://ytc.nanxuanxn.top

constexpr int N = 10;
来源：http://uub.smart0.xyz

[S58] C++：命名空间
来源：http://aca.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://wjy.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://xsn.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cbl.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://ulf.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gnc.gotoacloud.top

================================================================================
来源：http://cue.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dbq.pycfn.com

================================================================================
来源：http://kja.guannengcc.top

[T01] Kotlin：Hello World
来源：http://xsj.sjlbkw.cn

println("Hello")
来源：http://glu.fengsongda.top

[T02] Kotlin：变量
来源：http://nxe.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kmb.sweek.top

[T03] Kotlin：字符串模板
来源：http://sjo.chenlongwang.top

"值: $b"
来源：http://udm.epnwcf.com

[T04] Kotlin：空安全
来源：http://zgy.ehwqpu.com

val n: String? = null;  n?.length
来源：http://fde.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://jjs.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jqk.cucudq.cn

[T06] Kotlin：集合映射
来源：http://bos.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rtn.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://aml.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tam.jiagoushi.top

[T08] Kotlin：数据类
来源：http://ego.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://ofy.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://ndk.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://vlv.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://vcu.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jkl.haohaochexian.top

[T11] Kotlin：协程
来源：http://epp.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://upq.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://ghj.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://tiv.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://fad.zhaomingkeji.xyz

val m = mapOf("a" to 1)
来源：http://cqr.jqgufenzy.top

[T14] Kotlin：循环
来源：http://ixl.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://rnm.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://mni.c1oappe.top

interface Shape { fun area(): Double }
来源：http://xtg.nwbrower.top

[T16] Swift：Hello World
来源：http://kbm.yj20258.top

print("Hello")
来源：http://lvt.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://pqj.316326.xyz

var a = 1;  let b = 2
来源：http://mkb.nwbrower.top

[T18] Swift：字符串插值
来源：http://ykk.svipenyu.cn

"值: \(b)"
来源：http://stf.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://wam.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://jhu.aibaodan.cn

[T20] Swift：数组操作
来源：http://nrv.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oct.ehwqpu.com

[T21] Swift：遍历
来源：http://eqn.shanyushiyangtech.top

for x in a { print(x) }
来源：http://irw.xuetiantiany.cn

[T22] Swift：字典
来源：http://vjm.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wgt.0kj1m.cn

[T23] Swift：函数
来源：http://fkd.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fqj.kuanghao11.cn

[T24] Swift：闭包
来源：http://unm.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lba.dianchejie.cn

[T25] Swift：结构体
来源：http://esy.hcnkem.com

struct P { var x: Int }
来源：http://nbw.jinqigfzy.top

[T26] Swift：类与重写
来源：http://niq.cqqwz.cn

class A: Base { override func f() {} }
来源：http://zpo.fengsongda.top

[T27] Swift：错误处理
来源：http://ham.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://nmv.hfpthk.cn

[T28] Swift：枚举
来源：http://qqc.nanxuanxn.top

enum Color { case red, green }
来源：http://fdy.uphjek.com

[T29] Swift：guard 提前返回
来源：http://uoe.chenzaomai.com

guard let x = opt else { return }
来源：http://sua.ehwqpu.com

[T30] Swift：协议
来源：http://upg.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://hat.fzhhl.top

[T31] Lua：Hello World
来源：http://dvy.sysykeji.top

print("Hello")
来源：http://qlt.zhixingplan.top

[T32] Lua：局部变量
来源：http://xwx.sweek.top

local a = 1
来源：http://clq.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://arn.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://rkd.hammf.cn

[T34] Lua：遍历表
来源：http://cxe.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wcg.uphjek.com

[T35] Lua：字典表
来源：http://qqm.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://ani.pycfn.com

[T36] Lua：函数
来源：http://bjc.xylfe.cn

function add(a, b) return a + b end
来源：http://sfr.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://nym.andypj.xyz

"a" .. "b"
来源：http://imj.haohaochexian.top

[T38] Lua：条件
来源：http://iuz.smart0.xyz

if x > 0 then print("正") end
来源：http://yxb.chenlongwang.top

[T39] Lua：模式匹配
来源：http://cev.52xcode.cn

string.find(s, "%d+")
来源：http://otu.hywenlv.cn

[T40] Lua：元表
来源：http://fwa.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://njp.guowangkeji.top

[T41] Perl：Hello World
来源：http://jyr.fehbvm.com

print "Hello\n";
来源：http://uvb.xinyue.icu

[T42] Perl：变量类型
来源：http://sxn.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jgf.guannengcc.top

[T43] Perl：字符串插值
来源：http://isb.shangyingyoupin.top

"值: $a"
来源：http://hqd.jqgfzy.top

[T44] Perl：条件
来源：http://twi.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://zdx.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://hyf.dashuyun.cn

for my $x (@arr) { print $x; }
来源：http://jih.c1oappe.top

[T46] Perl：哈希操作
来源：http://lov.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hvf.tianlin.xyz

[T47] Perl：正则捕获
来源：http://xwn.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://div.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://xmc.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://oux.xuetiantiany.cn

[T49] Perl：函数
来源：http://aax.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mtr.yueranfly.top

[T50] Perl：逐行读文件
来源：http://cod.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sux.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://gco.yanxiufei.cn

[T51] Scala：Hello World
来源：http://zwk.52xcode.cn

println("Hello")
来源：http://vzj.yangfankeji.com

[T52] Scala：变量
来源：http://bbo.jinqigfzy.top

val a = 1;  var b = 2
来源：http://wgb.ctjpmb.com

[T53] Scala：字符串插值
来源：http://uql.nanxuanxn.top

s"值: $b"
来源：http://ycd.zhengqikj.top

[T54] Scala：集合映射
来源：http://hex.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://rfc.cqqwz.cn

[T55] Scala：集合过滤
来源：http://ddq.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://xbl.gogol.net.cn

[T56] Scala：样例类
来源：http://bqm.c1oappe.top

case class User(name: String, age: Int)
来源：http://fjo.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://bak.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iwl.jiagoushi.top

[T58] Scala：函数定义
来源：http://tgz.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cbu.nanxuanxn.top

[T59] Scala：循环
来源：http://voa.yuanzhike.top

for (i <- 1 to 10) println(i)
来源：http://iel.aibaodan.cn

[T60] Scala：折叠
来源：http://ixv.yfazqb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ask.tarul.cn

================================================================================
来源：http://mcg.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zrp.xingfuxueyuan.xyz

================================================================================
来源：http://gsw.yvedp.cn

[U01] Py：创建虚拟环境
来源：http://erc.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://aqf.andypj.xyz

[U02] Py：导出 / 安装依赖
来源：http://atd.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tsu.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://wuk.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yzq.havefunace.top

[U04] Py：变量调试打印
来源：http://vdx.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://igx.feifeiyinyue.top

[U05] Py：列表去重且保序
来源：http://ixc.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://xuq.yj202588.top

[U06] Py：合并两个字典
来源：http://veg.epnwcf.com

{**a, **b}
来源：http://lca.havefunace.top

[U07] Py：反转字典键值
来源：http://vcp.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://xie.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://bgl.fktsv.cn

[y for x in nested for y in x]
来源：http://roz.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://bau.epnwcf.com

max(d, key=d.get)
来源：http://sjg.bjfxy.top

[U10] Py：按值排序字典
来源：http://hji.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://onm.tianlin.xyz

[U11] Py：生成器表达式
来源：http://rgg.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://nym.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://zij.hesvh.cn

Counter(arr).most_common(3)
来源：http://cim.ivvv.top

[U13] Py：固定长度队列
来源：http://gvo.sweek.top

deque(maxlen=10)
来源：http://kvd.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://eyx.nanxinkj.top

defaultdict(list)
来源：http://yxx.meibo888.top

[U15] Py：高精度计时
来源：http://bub.smart0.xyz

t = time.perf_counter()
来源：http://fjf.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://bvx.ppjwa.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mwp.jqgfzy.top

[U17] Py：初始化日志
来源：http://oox.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://epq.cdnleiting.top

[U18] Py：预编译正则
来源：http://hfo.yj20258888.top

pat = re.compile(r"\d+")
来源：http://hoh.ydzc1.top

[U19] Py：正则替换带回调
来源：http://kri.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://alq.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://odd.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://xmj.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://rcy.svipenyu.cn

@contextlib.contextmanager
来源：http://gsy.jyoumei.cn

[U22] Py：矩阵转置
来源：http://weu.snrcjt.cn

list(zip(*m))
来源：http://rqk.yongpay.top

[U23] Py：分块读取大文件
来源：http://kza.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fgu.zycfv.cn

[U24] Py：路径操作
来源：http://qch.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ost.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://cin.cashguo.top

csv.DictReader(f)
来源：http://etz.yvedp.cn

[U26] Py：并发下载
来源：http://hgt.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://exv.cucudq.cn

[U27] Py：异步 HTTP
来源：http://voj.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://cxn.wangdashe.top

[U28] Py：类型别名
来源：http://crw.sweek.top

UserId = int
来源：http://thz.xylfe.cn

[U29] Py：属性校验
来源：http://iyu.hesvh.cn

@property 与 @x.setter 配合
来源：http://pak.gotoacloud.top

[U30] Py：数据类
来源：http://eaq.vehdjk.com

@dataclass(slots=True)
来源：http://ryg.zdbjq.cn

[U31] Py：单测
来源：http://skb.chenlongwang.top

python -m pytest -q
来源：http://vet.cdnleiting.top

[U32] Py：代码格式化
来源：http://fxg.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://vkq.dianchejie.cn

[U33] Py：打包发布
来源：http://tnt.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://fku.nanxuanxn.top

[U34] Py：判断编码
来源：http://fwu.vehdjk.com

chardet.detect(raw)
来源：http://ydm.yj202588.top

[U35] Py：发送邮件
来源：http://gqu.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ovn.bjfxy.top

[U36] Py：定时任务
来源：http://fhb.sweek.top

schedule.every(10).minutes.do(job)
来源：http://tso.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://tgs.ybcxt.top

pandas.read_excel / DataFrame.to_excel
来源：http://llw.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://ntl.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://jan.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://szi.hongshengwenyu.top

sys.stdout.isatty()
来源：http://ltu.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://nzy.chenjidiqi.icu

print("err", file=sys.stderr)
来源：http://rob.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://two.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://efw.shanyushiyangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://byg.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bfm.xinyue.icu

[U43] PHP：声明命名空间
来源：http://mym.sufxvd.cn

namespace App\Http;
来源：http://jap.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://mjn.redwolf501.top

declare(strict_types=1);
来源：http://nba.gotoacloud.top

[U45] PHP：类型声明与返回类型
来源：http://brn.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uew.nanxinkj.top

[U46] PHP：可空类型
来源：http://cor.hnqzz.top

?string $name = null
来源：http://dco.jinqigfzy.top

[U47] PHP：联合类型
来源：http://wii.tarul.cn

int|string $id
来源：http://bok.ydzc1.top

[U48] PHP：纯枚举
来源：http://krh.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://igl.nanxinkj.top

[U49] PHP：只读属性
来源：http://zov.yueranfly.top

public readonly string $name
来源：http://ikc.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://eyl.xinyue.icu

public function __construct(private int $id) {}
来源：http://kuu.zdqjudy.top

[U51] PHP：数组解构
来源：http://qic.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://cnv.bbcook.cn

[U52] PHP：箭头函数
来源：http://iho.gogol.net.cn

$double = fn($x) => $x * 2;
来源：http://jbr.meibo888.top

[U53] PHP：空合并运算符
来源：http://taq.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://dhe.yongpay.top

[U54] PHP：空安全调用
来源：http://lwl.cqqwz.cn

$obj?->method()
来源：http://thr.ppjwa.cn

[U55] PHP：match 表达式
来源：http://put.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gfr.gogol.net.cn

[U56] PHP：命名参数
来源：http://zna.mhx1999.top

f(a: 1, b: 2)
来源：http://ohn.gotoacloud.top

[U57] PHP：字符串插值
来源：http://hel.hnxiangtu.top

"值: {$a}"
来源：http://xid.gzhubu.top

[U58] PHP：数组三件套
来源：http://kye.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://htw.dianchejie.cn

[U59] PHP：自定义排序
来源：http://ecr.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ftu.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://sxc.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blx.guannengcc.top

[U61] PHP：正则
来源：http://sxd.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xao.chenjidiqi.icu

[U62] PHP：日期对象
来源：http://yze.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uxj.chenzaomai.com

[U63] PHP：文件读写
来源：http://lew.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kqt.uphjek.com

[U64] PHP：目录遍历
来源：http://mbw.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://rwv.zhijiandao.cn

[U65] PHP：会话
来源：http://mzc.zhiwuduotai.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xqp.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://xun.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yhf.zhoulong.xyz


<!-- 参考信息 -->