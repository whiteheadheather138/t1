代发 wailian999

[S41] C++：类与构造函数
来源：http://yks.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qys.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://isl.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://bdh.sysykeji.top

[S43] C++：智能指针
来源：http://xmg.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://viu.ivvv.top

[S44] C++：引用传参
来源：http://tas.fktsv.cn

void inc(int &x) { ++x; }
来源：http://wwi.xuetiantiany.cn

[S45] C++：lambda
来源：http://bjl.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lax.yuanzhike.top

[S46] C++：函数模板
来源：http://pdb.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kyg.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://wvy.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ywb.daxiang520.top

[S48] C++：逐行读文件
来源：http://nce.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://ths.andypj.xyz

while (std::getline(in, line)) { }
来源：http://uwd.sxryk.cn

[S49] C++：写文件
来源：http://sam.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://acf.cucudq.cn

[S50] C++：格式化数字
来源：http://con.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qgl.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://aea.nanxuanxn.top

static_cast<double>(a) / b
来源：http://jsd.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://guh.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://ktf.jyoumei.cn

[S53] C++：移动语义
来源：http://tig.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://ina.zhongyouzk.top

[S54] C++：异常处理
来源：http://akt.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bio.cucudq.cn

[S55] C++：结构化绑定
来源：http://qve.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ums.nanxinkj.top

[S56] C++：optional
来源：http://wvu.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cqy.jianghu66.top

[S57] C++：编译期常量
来源：http://idi.sweek.top

constexpr int N = 10;
来源：http://lhz.shangyingyoupin.top

[S58] C++：命名空间
来源：http://gem.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://tnd.jinqigufen.top

[S59] C++：静态断言
来源：http://soa.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ytl.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://biy.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qwo.52xcode.cn

================================================================================
来源：http://hkh.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kfv.jinqigufen.top

================================================================================
来源：http://vtf.smart0.xyz

[T01] Kotlin：Hello World
来源：http://agz.snrcjt.cn

println("Hello")
来源：http://xsn.snrcjt.cn

[T02] Kotlin：变量
来源：http://txs.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qcq.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://vcw.yfazqb.com

"值: $b"
来源：http://zun.dashuyun.cn

[T04] Kotlin：空安全
来源：http://aly.jqgfzy.top

val n: String? = null;  n?.length
来源：http://yvn.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://esb.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bqi.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://dvw.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ggi.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://txn.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ehz.guowangkeji.top

[T08] Kotlin：数据类
来源：http://vbg.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://ssx.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://yqn.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://xlg.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://ymc.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nkg.daxiang520.top

[T11] Kotlin：协程
来源：http://mua.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ltk.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://iwu.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://ydm.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://hji.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://qlg.ppjwa.cn

[T14] Kotlin：循环
来源：http://dds.9152youxi.cn

for (i in 1..10) println(i)
来源：http://uif.fehbvm.com

[T15] Kotlin：接口
来源：http://gek.zycfv.cn

interface Shape { fun area(): Double }
来源：http://djg.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://qag.yfazqb.com

print("Hello")
来源：http://ola.bbcook.cn

[T17] Swift：变量与常量
来源：http://ngg.shuidangran.top

var a = 1;  let b = 2
来源：http://wtu.zhixingplan.top

[T18] Swift：字符串插值
来源：http://amw.hongshengwenyu.top

"值: \(b)"
来源：http://wsp.ybcxt.top

[T19] Swift：可选绑定
来源：http://fgf.dashuyun.cn

if let n = opt { print(n) }
来源：http://xus.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://xbx.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aok.hysaishi.cn

[T21] Swift：遍历
来源：http://qvv.xinyue.icu

for x in a { print(x) }
来源：http://roc.jinghuilouyu.cn

[T22] Swift：字典
来源：http://iee.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cat.ctjpmb.com

[T23] Swift：函数
来源：http://wzn.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eaa.tianlin.xyz

[T24] Swift：闭包
来源：http://vhe.fengsongda.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hvn.fehbvm.com

[T25] Swift：结构体
来源：http://hwh.kuanghao11.cn

struct P { var x: Int }
来源：http://jhx.chenlongwang.top

[T26] Swift：类与重写
来源：http://kpk.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://wcj.tarul.cn

[T27] Swift：错误处理
来源：http://cub.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://bnd.chenjidiqi.icu

[T28] Swift：枚举
来源：http://fft.ivvv.top

enum Color { case red, green }
来源：http://dyg.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://snc.dianchejie.cn

guard let x = opt else { return }
来源：http://ezi.yanxiufei.cn

[T30] Swift：协议
来源：http://mzu.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://hcv.hnqzz.top

[T31] Lua：Hello World
来源：http://eem.haohaochexian.top

print("Hello")
来源：http://ksc.sysykeji.top

[T32] Lua：局部变量
来源：http://abo.jinghuilouyu.cn

local a = 1
来源：http://ylf.yfazqb.com

[T33] Lua：表（数组）
来源：http://bjr.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ijr.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://owh.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qjh.vqdsnc.cn

[T35] Lua：字典表
来源：http://xjy.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://szs.yangfankeji.com

[T36] Lua：函数
来源：http://fze.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://hof.iojbl.cn

[T37] Lua：字符串拼接
来源：http://pfu.zhoulong.xyz

"a" .. "b"
来源：http://ivd.fanxiaobao.xyz

[T38] Lua：条件
来源：http://hhy.yueranfly.top

if x > 0 then print("正") end
来源：http://gdn.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://idy.xziqi.cn

string.find(s, "%d+")
来源：http://rvh.hcnkem.com

[T40] Lua：元表
来源：http://bcp.yangfankeji.com

setmetatable({}, { __index = base })
来源：http://lkn.fzhhl.top

[T41] Perl：Hello World
来源：http://xwm.xingfuxueyuan.xyz

print "Hello\n";
来源：http://dmu.feifeiyinyue.top

[T42] Perl：变量类型
来源：http://yst.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eiv.yj202588.top

[T43] Perl：字符串插值
来源：http://gvz.ivvv.top

"值: $a"
来源：http://kgq.bbcook.cn

[T44] Perl：条件
来源：http://wsv.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://btk.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://gbd.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://zyl.birdmap.top

[T46] Perl：哈希操作
来源：http://kpu.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gwc.fengsongda.top

[T47] Perl：正则捕获
来源：http://vjk.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zrr.sjlbkw.cn

[T48] Perl：正则替换
来源：http://auw.cdnleiting.top

$s =~ s/old/new/g;
来源：http://lfi.pycfn.com

[T49] Perl：函数
来源：http://qve.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://flq.yj20258888.top

[T50] Perl：逐行读文件
来源：http://spx.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vvb.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://owo.ybcxt.top

[T51] Scala：Hello World
来源：http://mps.jinqigfzy.top

println("Hello")
来源：http://nic.uphjek.com

[T52] Scala：变量
来源：http://jzr.nwbrower.top

val a = 1;  var b = 2
来源：http://wmp.jyoumei.cn

[T53] Scala：字符串插值
来源：http://ppw.zhijiandao.cn

s"值: $b"
来源：http://bju.yj202588.top

[T54] Scala：集合映射
来源：http://mpx.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://dkd.316326.xyz

[T55] Scala：集合过滤
来源：http://ksc.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://bhd.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://hrj.dianchejie.cn

case class User(name: String, age: Int)
来源：http://psw.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://tou.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gfr.yfazqb.com

[T58] Scala：函数定义
来源：http://uuy.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hqu.zhoulong.xyz

[T59] Scala：循环
来源：http://vqa.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://ibd.andypj.xyz

[T60] Scala：折叠
来源：http://lcr.xziqi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nrz.ydzc1.top

================================================================================
来源：http://qng.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ysa.xingfuxueyuan.xyz

================================================================================
来源：http://vmu.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://put.snrcjt.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bzv.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://wfu.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://krg.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://lwr.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://wen.jianghu66.top

[U04] Py：变量调试打印
来源：http://wvw.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yot.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://jqy.yongpay.top

list(dict.fromkeys(arr))
来源：http://hbr.jyoumei.cn

[U06] Py：合并两个字典
来源：http://enl.guannengcc.top

{**a, **b}
来源：http://ycg.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://wxg.daria6918.cn

{v: k for k, v in d.items()}
来源：http://len.cdnleiting.top

[U08] Py：展平二维列表
来源：http://mgl.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://tti.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://kcv.bbcook.cn

max(d, key=d.get)
来源：http://gcj.hfpthk.cn

[U10] Py：按值排序字典
来源：http://wzm.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://isy.epnwcf.com

[U11] Py：生成器表达式
来源：http://nof.shanyushiyangkeji.top

(x * 2 for x in arr)
来源：http://kjm.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://hri.xinyue.icu

Counter(arr).most_common(3)
来源：http://gxf.9152youxi.cn

[U13] Py：固定长度队列
来源：http://nhs.jlsjyb.cn

deque(maxlen=10)
来源：http://lqd.yonumen.top

[U14] Py：分组收集到列表
来源：http://ttq.nanxinkj.top

defaultdict(list)
来源：http://jca.hnxiangtu.top

[U15] Py：高精度计时
来源：http://ssk.yfazqb.com

t = time.perf_counter()
来源：http://rxp.yongpay.top

[U16] Py：命令行参数解析
来源：http://wli.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hlg.iojbl.cn

[U17] Py：初始化日志
来源：http://vze.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://ngk.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://ttt.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://kam.yonumen.top

[U19] Py：正则替换带回调
来源：http://nik.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ufz.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://qzn.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://jkw.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://fbe.wangshuangyany.cn

@contextlib.contextmanager
来源：http://vrz.zhaomingkeji.xyz

[U22] Py：矩阵转置
来源：http://qpu.ywan-chungtsiang.top

list(zip(*m))
来源：http://yqv.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://oxs.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fqc.316326.xyz

[U24] Py：路径操作
来源：http://gui.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xgj.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://ohj.yuxming.cn

csv.DictReader(f)
来源：http://fps.sjlbkw.cn

[U26] Py：并发下载
来源：http://vdh.fengsongda.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fyx.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://gyo.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://ikg.zhixingplan.top

[U28] Py：类型别名
来源：http://dbh.smart0.xyz

UserId = int
来源：http://qzo.aibaodan.cn

[U29] Py：属性校验
来源：http://gmm.chenlongwang.top

@property 与 @x.setter 配合
来源：http://sbm.jyoumei.cn

[U30] Py：数据类
来源：http://vjq.bjfxy.top

@dataclass(slots=True)
来源：http://qve.hcnkem.com

[U31] Py：单测
来源：http://zqo.vehdjk.com

python -m pytest -q
来源：http://jbz.gaohongyu789.top

[U32] Py：代码格式化
来源：http://whw.wangdashe.top

ruff format . && ruff check --fix .
来源：http://ahw.sufxvd.cn

[U33] Py：打包发布
来源：http://era.chenlongwang.top

python -m build  （依赖 pyproject.toml）
来源：http://nbh.tanke756.top

[U34] Py：判断编码
来源：http://kqd.xingfuxueyuan.xyz

chardet.detect(raw)
来源：http://gvp.yangfankeji.com

[U35] Py：发送邮件
来源：http://zdj.xylfe.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://isx.316326.xyz

[U36] Py：定时任务
来源：http://ksr.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://nvo.zdqjudy.top

[U37] Py：读写 Excel
来源：http://btv.cqqwz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://idy.quarkkingdee.top

[U38] Py：获取脚本所在目录
来源：http://nky.yj202588.top

Path(__file__).resolve().parent
来源：http://htx.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://fgz.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://peu.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://ycx.cdnleiting.top

print("err", file=sys.stderr)
来源：http://ctx.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://dhx.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://eir.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://gve.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rts.zdbjq.cn

[U43] PHP：声明命名空间
来源：http://rjz.zycfv.cn

namespace App\Http;
来源：http://eys.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://dch.zycfv.cn

declare(strict_types=1);
来源：http://fcp.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://tbo.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oru.gotoacloud.top

[U46] PHP：可空类型
来源：http://jic.jinqigufen.top

?string $name = null
来源：http://enb.ybcxt.top

[U47] PHP：联合类型
来源：http://lae.cheryme.top

int|string $id
来源：http://xab.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://wto.daria6918.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pgf.gogol.net.cn

[U49] PHP：只读属性
来源：http://elj.xuanzx.com

public readonly string $name
来源：http://srf.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://cxb.yongpay.top

public function __construct(private int $id) {}
来源：http://cdt.yj20258.top

[U51] PHP：数组解构
来源：http://uud.ydzc1.top

[$a, $b] = $arr;
来源：http://ztj.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://tot.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://pwj.yfazqb.com

[U53] PHP：空合并运算符
来源：http://ana.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://jew.c1oappe.top

[U54] PHP：空安全调用
来源：http://eef.yvedp.cn

$obj?->method()
来源：http://tnm.yongpay.top

[U55] PHP：match 表达式
来源：http://ngk.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zvn.fktsv.cn

[U56] PHP：命名参数
来源：http://bpm.haohaochexian.top

f(a: 1, b: 2)
来源：http://sif.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://olo.quarkkingdee.top

"值: {$a}"
来源：http://obi.shuidangran.top

[U58] PHP：数组三件套
来源：http://yxf.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lcx.zhixingplan.top

[U59] PHP：自定义排序
来源：http://zpu.jinghuilouyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vax.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://pvy.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://okf.jyoumei.cn

[U61] PHP：正则
来源：http://ztp.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rvi.bbcook.cn

[U62] PHP：日期对象
来源：http://uia.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gsu.zhixingplan.top

[U63] PHP：文件读写
来源：http://poj.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nbu.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://cja.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://xpw.pengpengdd.cyou

[U65] PHP：会话
来源：http://geh.yonumen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://opl.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://kjk.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pdi.epnwcf.com


<!-- 参考信息 -->