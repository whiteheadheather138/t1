代发 wailian999

[S35] C++：map
来源：http://ile.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jms.nanxuanxn.top

[S36] C++：unordered_map
来源：http://rui.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rwp.chenzaomai.com

[S37] C++：set
来源：http://ert.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wqv.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://jop.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://icl.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://ybx.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xwj.snrcjt.cn

[S40] C++：查找元素
来源：http://lrb.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aeq.fktsv.cn

[S41] C++：类与构造函数
来源：http://ozz.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dqi.uphjek.com

[S42] C++：继承与虚函数
来源：http://xve.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://wul.hfpthk.cn

[S43] C++：智能指针
来源：http://hhv.meibo888.top

auto p = std::make_unique<int>(5);
来源：http://bba.zhengqikj.top

[S44] C++：引用传参
来源：http://jht.fzhhl.top

void inc(int &x) { ++x; }
来源：http://iif.uphjek.com

[S45] C++：lambda
来源：http://aww.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://ovj.cheryme.top

[S46] C++：函数模板
来源：http://fjr.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nlm.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://wnf.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vuj.iojbl.cn

[S48] C++：逐行读文件
来源：http://imx.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://xtp.tarul.cn

while (std::getline(in, line)) { }
来源：http://mop.gzhubu.top

[S49] C++：写文件
来源：http://qpn.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mkk.birdmap.top

[S50] C++：格式化数字
来源：http://jtc.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yrc.cqqwz.cn

[S51] C++：显式类型转换
来源：http://vpe.hcnkem.com

static_cast<double>(a) / b
来源：http://jzy.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://rlp.vehdjk.com

int size() const noexcept { return n_; }
来源：http://pec.jyoumei.cn

[S53] C++：移动语义
来源：http://whg.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://vdn.quarkkingdee.top

[S54] C++：异常处理
来源：http://vhw.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xcb.jinqigufen.top

[S55] C++：结构化绑定
来源：http://elp.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://orf.hcnkem.com

[S56] C++：optional
来源：http://hud.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nzv.meibo888.top

[S57] C++：编译期常量
来源：http://kff.zhongyouzk.top

constexpr int N = 10;
来源：http://fnl.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://tou.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://uwh.aibaodan.cn

[S59] C++：静态断言
来源：http://rjc.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nrx.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://bqx.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oue.yuxming.cn

================================================================================
来源：http://vjw.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uee.zdqjudy.top

================================================================================
来源：http://dqq.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://dih.sxryk.cn

println("Hello")
来源：http://gwa.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://lll.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bbt.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://cia.zycfv.cn

"值: $b"
来源：http://ced.gotoacloud.top

[T04] Kotlin：空安全
来源：http://saw.yongpay.top

val n: String? = null;  n?.length
来源：http://npx.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://aok.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bhc.vehdjk.com

[T06] Kotlin：集合映射
来源：http://tbg.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ikf.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://hsq.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nff.cashguo.top

[T08] Kotlin：数据类
来源：http://ozw.snrcjt.cn

data class User(val name: String, val age: Int)
来源：http://dke.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://xpb.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://uwu.yj20258.top

[T10] Kotlin：默认参数
来源：http://ekg.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vvh.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://kys.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ohx.yj202588.top

[T12] Kotlin：解构声明
来源：http://zsb.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://fej.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://otu.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://rvh.fzhhl.top

[T14] Kotlin：循环
来源：http://xuu.wangdashe.top

for (i in 1..10) println(i)
来源：http://pxf.c1oappe.top

[T15] Kotlin：接口
来源：http://lbd.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://vdq.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://znq.feifeiyinyue.top

print("Hello")
来源：http://mwi.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://xbe.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://iwl.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://erb.aizwys.cn

"值: \(b)"
来源：http://img.316326.xyz

[T19] Swift：可选绑定
来源：http://toe.xylfe.cn

if let n = opt { print(n) }
来源：http://icj.cqqwz.cn

[T20] Swift：数组操作
来源：http://pfr.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tqj.yfazqb.com

[T21] Swift：遍历
来源：http://gch.nanxinkj.top

for x in a { print(x) }
来源：http://xgd.shanyushiyangtech.top

[T22] Swift：字典
来源：http://kew.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://zax.hysaishi.cn

[T23] Swift：函数
来源：http://hhg.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ynp.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://wwf.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sxs.zhongyouzk.top

[T25] Swift：结构体
来源：http://jec.ydzc1.top

struct P { var x: Int }
来源：http://rvs.sjlbkw.cn

[T26] Swift：类与重写
来源：http://ixz.cqqwz.cn

class A: Base { override func f() {} }
来源：http://zqm.316326.xyz

[T27] Swift：错误处理
来源：http://zwm.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://qqd.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://mns.nwbrower.top

enum Color { case red, green }
来源：http://gzq.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://jei.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://etl.uphjek.com

[T30] Swift：协议
来源：http://ihs.yj202588.top

protocol Shape { func area() -> Double }
来源：http://mdq.zhaomingkeji.xyz

[T31] Lua：Hello World
来源：http://hll.zhiwuduotai.top

print("Hello")
来源：http://zgn.guowangkeji.top

[T32] Lua：局部变量
来源：http://nxn.cheryme.top

local a = 1
来源：http://gyi.ydzc1.top

[T33] Lua：表（数组）
来源：http://xgg.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ear.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://jaf.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://xjx.redwolf501.top

[T35] Lua：字典表
来源：http://yrz.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://hmy.zycfv.cn

[T36] Lua：函数
来源：http://mgr.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://uzd.yj20258888.top

[T37] Lua：字符串拼接
来源：http://ime.haohaochexian.top

"a" .. "b"
来源：http://lnc.yongpay.top

[T38] Lua：条件
来源：http://uxx.bjfxy.top

if x > 0 then print("正") end
来源：http://ikr.0kj1m.cn

[T39] Lua：模式匹配
来源：http://lzk.redwolf501.top

string.find(s, "%d+")
来源：http://klh.hongshengwenyu.top

[T40] Lua：元表
来源：http://kcu.jyoumei.cn

setmetatable({}, { __index = base })
来源：http://jdh.dashuyun.cn

[T41] Perl：Hello World
来源：http://zfz.birdmap.top

print "Hello\n";
来源：http://oxi.ctjpmb.com

[T42] Perl：变量类型
来源：http://xot.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wiv.haohaochexian.top

[T43] Perl：字符串插值
来源：http://lmh.pengpengdd.cyou

"值: $a"
来源：http://sal.ivvv.top

[T44] Perl：条件
来源：http://jdv.andypj.xyz

if ($a > 0) { print "正"; }
来源：http://fhj.ctjpmb.com

[T45] Perl：数组遍历
来源：http://cuj.yongpay.top

for my $x (@arr) { print $x; }
来源：http://skw.birdmap.top

[T46] Perl：哈希操作
来源：http://bes.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bpo.redwolf501.top

[T47] Perl：正则捕获
来源：http://tuu.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://uee.jinqigfzy.top

[T48] Perl：正则替换
来源：http://blq.sufxvd.cn

$s =~ s/old/new/g;
来源：http://aam.yfazqb.com

[T49] Perl：函数
来源：http://uxp.hongshengwenyu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vih.fzhhl.top

[T50] Perl：逐行读文件
来源：http://fxi.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kfb.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://vda.bjfxy.top

[T51] Scala：Hello World
来源：http://ype.yj20258.top

println("Hello")
来源：http://xax.xinyue.icu

[T52] Scala：变量
来源：http://kgn.iojbl.cn

val a = 1;  var b = 2
来源：http://nof.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://qkw.aibaodan.cn

s"值: $b"
来源：http://rvf.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://les.0kj1m.cn

List(1, 2, 3).map(_ * 2)
来源：http://agh.zhixingplan.top

[T55] Scala：集合过滤
来源：http://vnc.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nek.gotoacloud.top

[T56] Scala：样例类
来源：http://moj.smart0.xyz

case class User(name: String, age: Int)
来源：http://uad.dianchejie.cn

[T57] Scala：模式匹配
来源：http://pww.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jcu.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://mzz.xingfuxueyuan.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://guk.bjfxy.top

[T59] Scala：循环
来源：http://zqr.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://nfu.jianghu66.top

[T60] Scala：折叠
来源：http://pwm.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bif.ybcxt.top

================================================================================
来源：http://mqy.vehdjk.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fvi.cdnleiting.top

================================================================================
来源：http://day.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://xlr.jqgfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://oai.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://esr.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tgp.sweek.top

[U03] Py：加载 .env 配置
来源：http://fce.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tgx.yuxming.cn

[U04] Py：变量调试打印
来源：http://tjl.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qjz.tanke756.top

[U05] Py：列表去重且保序
来源：http://dwk.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://vgj.zdbjq.cn

[U06] Py：合并两个字典
来源：http://rji.pycfn.com

{**a, **b}
来源：http://enm.shangyingyoupin.top

[U07] Py：反转字典键值
来源：http://ipn.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://hqr.dianchejie.cn

[U08] Py：展平二维列表
来源：http://npm.ybcxt.top

[y for x in nested for y in x]
来源：http://ayk.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://akg.jinqigufen.top

max(d, key=d.get)
来源：http://iuv.ehwqpu.com

[U10] Py：按值排序字典
来源：http://omk.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jlm.redwolf501.top

[U11] Py：生成器表达式
来源：http://hdt.jqgufenzy.top

(x * 2 for x in arr)
来源：http://cyw.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://cec.hcnkem.com

Counter(arr).most_common(3)
来源：http://keq.yj202588.top

[U13] Py：固定长度队列
来源：http://cqq.vqdsnc.cn

deque(maxlen=10)
来源：http://fik.ybcxt.top

[U14] Py：分组收集到列表
来源：http://aru.nanxuanxn.top

defaultdict(list)
来源：http://nbr.fzhhl.top

[U15] Py：高精度计时
来源：http://wjs.yongpay.top

t = time.perf_counter()
来源：http://hlc.ivvv.top

[U16] Py：命令行参数解析
来源：http://nnc.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ojg.aizwys.cn

[U17] Py：初始化日志
来源：http://rgb.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://brw.gogol.net.cn

[U18] Py：预编译正则
来源：http://xxl.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://kcv.wangdashe.top

[U19] Py：正则替换带回调
来源：http://vbk.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iik.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://jxc.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://lij.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://zoi.cdnleiting.top

@contextlib.contextmanager
来源：http://sbb.dianchejie.cn

[U22] Py：矩阵转置
来源：http://qwj.haohaochexian.top

list(zip(*m))
来源：http://ecp.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://cms.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fol.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://mxp.chenlongwang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jjv.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://xva.ehwqpu.com

csv.DictReader(f)
来源：http://ujt.tian-w.cn

[U26] Py：并发下载
来源：http://pal.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wco.fzhhl.top

[U27] Py：异步 HTTP
来源：http://uga.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://mpo.tianlin.xyz

[U28] Py：类型别名
来源：http://iwq.chenlongwang.top

UserId = int
来源：http://ioq.chenzaomai.com

[U29] Py：属性校验
来源：http://apv.sweek.top

@property 与 @x.setter 配合
来源：http://uet.xingfuxueyuan.xyz

[U30] Py：数据类
来源：http://lqc.ydjk.org.cn

@dataclass(slots=True)
来源：http://hpn.yj20258.top

[U31] Py：单测
来源：http://dxv.tanke756.top

python -m pytest -q
来源：http://itz.kuanghao11.cn

[U32] Py：代码格式化
来源：http://zzn.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://ary.feifeiyinyue.top

[U33] Py：打包发布
来源：http://qwi.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://wty.hnqzz.top

[U34] Py：判断编码
来源：http://qcc.xinyue.icu

chardet.detect(raw)
来源：http://idv.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://acl.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xde.hnqzz.top

[U36] Py：定时任务
来源：http://rom.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://gur.hcnkem.com

[U37] Py：读写 Excel
来源：http://vbu.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://kca.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://cye.jyoumei.cn

Path(__file__).resolve().parent
来源：http://rnj.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://vfn.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://fwe.tian-w.cn

[U40] Py：打印到标准错误
来源：http://vpg.bjfxy.top

print("err", file=sys.stderr)
来源：http://stc.jinqigufen.top

[U41] PHP：初始化 Composer 项目
来源：http://lge.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rbm.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://smp.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://byt.316326.xyz

[U43] PHP：声明命名空间
来源：http://vjk.haohaochexian.top

namespace App\Http;
来源：http://fau.cheryme.top

[U44] PHP：开启严格类型
来源：http://kvm.hammf.cn

declare(strict_types=1);
来源：http://nru.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://vfi.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wph.cqqwz.cn

[U46] PHP：可空类型
来源：http://zat.sxryk.cn

?string $name = null
来源：http://fry.nanxuanxn.top

[U47] PHP：联合类型
来源：http://sgg.xinyue.icu

int|string $id
来源：http://awg.hysaishi.cn

[U48] PHP：纯枚举
来源：http://noz.gzhubu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xff.yj20258888.top

[U49] PHP：只读属性
来源：http://tnr.zhixingplan.top

public readonly string $name
来源：http://gsx.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://ahi.mhx1999.top

public function __construct(private int $id) {}
来源：http://sue.hysaishi.cn

[U51] PHP：数组解构
来源：http://uxd.mhx1999.top

[$a, $b] = $arr;
来源：http://uga.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://xia.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://qcs.fengsongda.top

[U53] PHP：空合并运算符
来源：http://pfh.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://lpb.zycfv.cn

[U54] PHP：空安全调用
来源：http://nsz.ppjwa.cn

$obj?->method()
来源：http://ahh.cashguo.top

[U55] PHP：match 表达式
来源：http://ltl.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bqw.zdbjq.cn

[U56] PHP：命名参数
来源：http://gsw.9152youxi.cn

f(a: 1, b: 2)
来源：http://tid.jianghu66.top

[U57] PHP：字符串插值
来源：http://oyf.bjfxy.top

"值: {$a}"
来源：http://xyk.yj202588.top

[U58] PHP：数组三件套
来源：http://clu.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gvc.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://rpj.yanxiufei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qhd.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://cmg.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wdn.hesvh.cn


<!-- 参考信息 -->