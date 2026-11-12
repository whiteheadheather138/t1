代发 wailian999

[S35] C++：map
来源：http://pom.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zbh.gotoacloud.top

[S36] C++：unordered_map
来源：http://pqm.guannengcc.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nqm.xinyue.icu

[S37] C++：set
来源：http://lyq.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oba.daxiang520.top

[S38] C++：排序
来源：http://cgn.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://pth.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://nqz.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zxa.shuidangran.top

[S40] C++：查找元素
来源：http://bof.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ixd.xylfe.cn

[S41] C++：类与构造函数
来源：http://ehg.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hjs.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://aqz.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://mvm.yanxiufei.cn

[S43] C++：智能指针
来源：http://tzi.haohaochexian.top

auto p = std::make_unique<int>(5);
来源：http://hhq.feifeiyinyue.top

[S44] C++：引用传参
来源：http://nqz.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://khl.vehdjk.com

[S45] C++：lambda
来源：http://ngf.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fvt.daria6918.cn

[S46] C++：函数模板
来源：http://ejj.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ptl.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://xnb.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lko.yuxming.cn

[S48] C++：逐行读文件
来源：http://gfz.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lhv.52xcode.cn

while (std::getline(in, line)) { }
来源：http://zrc.zhixingplan.top

[S49] C++：写文件
来源：http://inl.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kvv.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://bvs.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bfe.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://lhy.xuanzx.com

static_cast<double>(a) / b
来源：http://bdp.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://fda.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://qfz.zhijiandao.cn

[S53] C++：移动语义
来源：http://ymj.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://rin.ydzc1.top

[S54] C++：异常处理
来源：http://iqk.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://agy.jinqigufen.top

[S55] C++：结构化绑定
来源：http://mpp.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iif.daria6918.cn

[S56] C++：optional
来源：http://gsw.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://exh.meibo888.top

[S57] C++：编译期常量
来源：http://vcr.nanxinkj.top

constexpr int N = 10;
来源：http://zun.zhixingplan.top

[S58] C++：命名空间
来源：http://nmv.meibo888.top

namespace ns { int f() { return 1; } }
来源：http://lue.dashuyun.cn

[S59] C++：静态断言
来源：http://dbm.nwbrower.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://joj.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://snc.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pss.zdqjudy.top

================================================================================
来源：http://gsw.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ekb.fanxiaobao.xyz

================================================================================
来源：http://gdt.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://hyz.pengpengdd.cyou

println("Hello")
来源：http://wmi.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://ktc.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lrb.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://yqj.ydzc1.top

"值: $b"
来源：http://dlo.fzhhl.top

[T04] Kotlin：空安全
来源：http://xjk.yj20258.top

val n: String? = null;  n?.length
来源：http://rve.meibo888.top

[T05] Kotlin：when 表达式
来源：http://ocy.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aul.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://dxv.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nuc.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://nnw.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xeh.yongpay.top

[T08] Kotlin：数据类
来源：http://hxm.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://doh.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://hov.meibo888.top

fun String.exclaim() = this + "!"
来源：http://wsn.fktsv.cn

[T10] Kotlin：默认参数
来源：http://nrh.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bup.iojbl.cn

[T11] Kotlin：协程
来源：http://rxq.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pmp.guannengcc.top

[T12] Kotlin：解构声明
来源：http://trd.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://wau.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://low.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://cjx.dashuyun.cn

[T14] Kotlin：循环
来源：http://lzz.tanke756.top

for (i in 1..10) println(i)
来源：http://ixz.epnwcf.com

[T15] Kotlin：接口
来源：http://sfh.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://rsw.hnqzz.top

[T16] Swift：Hello World
来源：http://csa.tianlin.xyz

print("Hello")
来源：http://vfp.tian-w.cn

[T17] Swift：变量与常量
来源：http://mho.cdnleiting.top

var a = 1;  let b = 2
来源：http://enh.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://kud.fzhhl.top

"值: \(b)"
来源：http://ypw.ivvv.top

[T19] Swift：可选绑定
来源：http://oni.sysykeji.top

if let n = opt { print(n) }
来源：http://pzc.havefunace.top

[T20] Swift：数组操作
来源：http://wwb.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://qre.andypj.xyz

[T21] Swift：遍历
来源：http://mej.shanyushiyangkeji.top

for x in a { print(x) }
来源：http://wet.wangdashe.top

[T22] Swift：字典
来源：http://sci.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://cna.jyoumei.cn

[T23] Swift：函数
来源：http://zfe.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nlo.yongpay.top

[T24] Swift：闭包
来源：http://ewc.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bgb.ppjwa.cn

[T25] Swift：结构体
来源：http://nnr.cheryme.top

struct P { var x: Int }
来源：http://ucg.shuidangran.top

[T26] Swift：类与重写
来源：http://ujg.shangyingyoupin.top

class A: Base { override func f() {} }
来源：http://vfm.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://ebo.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://ews.vqdsnc.cn

[T28] Swift：枚举
来源：http://pgy.aizwys.cn

enum Color { case red, green }
来源：http://kyw.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://ezq.havefunace.top

guard let x = opt else { return }
来源：http://qiy.yonumen.top

[T30] Swift：协议
来源：http://ulu.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://dzb.hysaishi.cn

[T31] Lua：Hello World
来源：http://zde.guannengcc.top

print("Hello")
来源：http://vzh.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://ovr.meibo888.top

local a = 1
来源：http://avi.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://kah.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://yny.zhengqikj.top

[T34] Lua：遍历表
来源：http://qop.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dlq.cucudq.cn

[T35] Lua：字典表
来源：http://yhs.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://kak.ywan-chungtsiang.top

[T36] Lua：函数
来源：http://mzx.hcnkem.com

function add(a, b) return a + b end
来源：http://lpt.yuxming.cn

[T37] Lua：字符串拼接
来源：http://lqe.shangyingyoupin.top

"a" .. "b"
来源：http://dpj.zycfv.cn

[T38] Lua：条件
来源：http://rtz.yuanzhike.top

if x > 0 then print("正") end
来源：http://jnc.chenzaomai.com

[T39] Lua：模式匹配
来源：http://ddp.gotoacloud.top

string.find(s, "%d+")
来源：http://qxx.sweek.top

[T40] Lua：元表
来源：http://bgz.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://ocl.yonumen.top

[T41] Perl：Hello World
来源：http://mgp.aizwys.cn

print "Hello\n";
来源：http://gag.birdmap.top

[T42] Perl：变量类型
来源：http://tnf.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jst.shuidangran.top

[T43] Perl：字符串插值
来源：http://lai.vehdjk.com

"值: $a"
来源：http://ktf.yonumen.top

[T44] Perl：条件
来源：http://hdt.yfazqb.com

if ($a > 0) { print "正"; }
来源：http://gfa.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://kzh.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://qdf.yuanzhike.top

[T46] Perl：哈希操作
来源：http://ahs.hammf.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sti.xziqi.cn

[T47] Perl：正则捕获
来源：http://cmw.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://eax.yj20258888.top

[T48] Perl：正则替换
来源：http://vhd.zhixingplan.top

$s =~ s/old/new/g;
来源：http://wiu.yanxiufei.cn

[T49] Perl：函数
来源：http://qra.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://inw.yfazqb.com

[T50] Perl：逐行读文件
来源：http://qpw.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rbt.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://dlf.aibaodan.cn

[T51] Scala：Hello World
来源：http://czp.hnqzz.top

println("Hello")
来源：http://cqm.bjfxy.top

[T52] Scala：变量
来源：http://fxq.pycfn.com

val a = 1;  var b = 2
来源：http://nut.ppjwa.cn

[T53] Scala：字符串插值
来源：http://epd.jinqigufen.top

s"值: $b"
来源：http://lnk.tian-w.cn

[T54] Scala：集合映射
来源：http://jiz.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://lyx.cqqwz.cn

[T55] Scala：集合过滤
来源：http://yqh.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://csl.bjfxy.top

[T56] Scala：样例类
来源：http://kho.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://qog.316326.xyz

[T57] Scala：模式匹配
来源：http://cnn.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jot.snrcjt.cn

[T58] Scala：函数定义
来源：http://xjb.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://kie.fehbvm.com

[T59] Scala：循环
来源：http://tgv.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://qyn.zhengqikj.top

[T60] Scala：折叠
来源：http://lzf.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cep.hywenlv.cn

================================================================================
来源：http://xhx.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ygb.jianghu66.top

================================================================================
来源：http://qav.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://rmb.ydzc1.top

python -m venv .venv && source .venv/bin/activate
来源：http://lcl.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://oly.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zdi.shzxlz.cn

[U03] Py：加载 .env 配置
来源：http://sxa.hcnkem.com

from dotenv import load_dotenv; load_dotenv()
来源：http://gih.hongshengwenyu.top

[U04] Py：变量调试打印
来源：http://cll.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://acz.dashuyun.cn

[U05] Py：列表去重且保序
来源：http://uch.hesvh.cn

list(dict.fromkeys(arr))
来源：http://wxg.zhijiandao.cn

[U06] Py：合并两个字典
来源：http://ylm.gaohongyu789.top

{**a, **b}
来源：http://saz.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://kyj.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://zml.zycfv.cn

[U08] Py：展平二维列表
来源：http://wsi.0kj1m.cn

[y for x in nested for y in x]
来源：http://ieh.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://cvj.ppjwa.cn

max(d, key=d.get)
来源：http://ecv.xuetiantiany.cn

[U10] Py：按值排序字典
来源：http://eya.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fkl.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://nhs.jianghu66.top

(x * 2 for x in arr)
来源：http://etb.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ifb.zdbjq.cn

Counter(arr).most_common(3)
来源：http://iqq.zycfv.cn

[U13] Py：固定长度队列
来源：http://ddg.hfpthk.cn

deque(maxlen=10)
来源：http://zaa.yuanzhike.top

[U14] Py：分组收集到列表
来源：http://tdh.fehbvm.com

defaultdict(list)
来源：http://ktt.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://nwd.meibo888.top

t = time.perf_counter()
来源：http://lfv.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://uhh.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ycs.pycfn.com

[U17] Py：初始化日志
来源：http://vla.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://iza.sweek.top

[U18] Py：预编译正则
来源：http://dic.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://ovr.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://cim.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lzf.yvedp.cn

[U20] Py：缓存函数结果
来源：http://pmf.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://agb.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://tbb.mhx1999.top

@contextlib.contextmanager
来源：http://sap.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://pzo.bbcook.cn

list(zip(*m))
来源：http://miy.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://muk.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sef.quarkkingdee.top

[U24] Py：路径操作
来源：http://ndl.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rnz.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://olp.fzhhl.top

csv.DictReader(f)
来源：http://swb.yj20258888.top

[U26] Py：并发下载
来源：http://khl.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ujx.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://idi.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://hne.yuxming.cn

[U28] Py：类型别名
来源：http://ubf.bbcook.cn

UserId = int
来源：http://lht.birdmap.top

[U29] Py：属性校验
来源：http://rhp.yj20258.top

@property 与 @x.setter 配合
来源：http://dnq.gogol.net.cn

[U30] Py：数据类
来源：http://nly.svipenyu.cn

@dataclass(slots=True)
来源：http://tnm.ydjk.org.cn

[U31] Py：单测
来源：http://ynz.xingfuxueyuan.xyz

python -m pytest -q
来源：http://had.shanyushiyangtech.top

[U32] Py：代码格式化
来源：http://jos.yj202588.top

ruff format . && ruff check --fix .
来源：http://fpg.shzxlz.cn

[U33] Py：打包发布
来源：http://mlg.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://zft.shzxlz.cn

[U34] Py：判断编码
来源：http://hxk.yanxiufei.cn

chardet.detect(raw)
来源：http://xoa.fzhhl.top

[U35] Py：发送邮件
来源：http://nlr.shangyingyoupin.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mld.kuanghao11.cn

[U36] Py：定时任务
来源：http://cjj.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://fil.meibo888.top

[U37] Py：读写 Excel
来源：http://cse.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://rdi.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://ucy.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://ang.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://bvl.fktsv.cn

sys.stdout.isatty()
来源：http://vjf.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://oox.sweek.top

print("err", file=sys.stderr)
来源：http://ykc.zhongyouzk.top

[U41] PHP：初始化 Composer 项目
来源：http://zqw.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ryk.tian-w.cn

[U42] PHP：PSR-4 自动加载
来源：http://yis.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ffn.sxryk.cn

[U43] PHP：声明命名空间
来源：http://ipc.ehwqpu.com

namespace App\Http;
来源：http://xvx.cdnleiting.top

[U44] PHP：开启严格类型
来源：http://yks.ybcxt.top

declare(strict_types=1);
来源：http://nvb.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://vaq.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wul.sufxvd.cn

[U46] PHP：可空类型
来源：http://dwi.chenzaomai.com

?string $name = null
来源：http://dlx.0kj1m.cn

[U47] PHP：联合类型
来源：http://jkm.nwbrower.top

int|string $id
来源：http://bwz.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://zkw.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mvx.ehwqpu.com

[U49] PHP：只读属性
来源：http://ydr.jinqigfzy.top

public readonly string $name
来源：http://ymv.cucudq.cn

[U50] PHP：构造器属性提升
来源：http://iwp.shzxlz.cn

public function __construct(private int $id) {}
来源：http://slv.tianlin.xyz

[U51] PHP：数组解构
来源：http://yom.0kj1m.cn

[$a, $b] = $arr;
来源：http://nyr.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://rqq.cdnleiting.top

$double = fn($x) => $x * 2;
来源：http://swq.hcnkem.com

[U53] PHP：空合并运算符
来源：http://ldq.ydjk.org.cn

$v = $a ?? $b ?? "default";
来源：http://zmz.hfpthk.cn

[U54] PHP：空安全调用
来源：http://bjd.ivvv.top

$obj?->method()
来源：http://shk.jinqigufen.top

[U55] PHP：match 表达式
来源：http://krk.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gmc.hnqzz.top

[U56] PHP：命名参数
来源：http://lca.fengsongda.top

f(a: 1, b: 2)
来源：http://ctd.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://yod.fengsongda.top

"值: {$a}"
来源：http://pgg.tianlin.xyz

[U58] PHP：数组三件套
来源：http://kkv.jinghuilouyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://njs.yueranfly.top

[U59] PHP：自定义排序
来源：http://qdr.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ihp.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://uzg.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oah.daria6918.cn


<!-- 参考信息 -->