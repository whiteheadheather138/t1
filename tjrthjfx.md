代发 wailian999

[S33] C++：vector 增删
来源：http://wbl.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hom.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://gqe.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://xae.52xcode.cn

[S35] C++：map
来源：http://gdv.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zjw.kuanghao11.cn

[S36] C++：unordered_map
来源：http://cis.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ngm.gogol.net.cn

[S37] C++：set
来源：http://jol.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pnl.tianlin.xyz

[S38] C++：排序
来源：http://xwj.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://ujf.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://evx.smart0.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bup.birdmap.top

[S40] C++：查找元素
来源：http://bnm.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://chi.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://rca.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gbu.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://ehe.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://zbe.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://pod.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://dvh.yvedp.cn

[S44] C++：引用传参
来源：http://wvd.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://ect.9152youxi.cn

[S45] C++：lambda
来源：http://ukr.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hmb.pengpengdd.cyou

[S46] C++：函数模板
来源：http://tky.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://crc.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://vrv.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zjt.aibaodan.cn

[S48] C++：逐行读文件
来源：http://jcw.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sgx.c1oappe.top

while (std::getline(in, line)) { }
来源：http://uls.chenlongwang.top

[S49] C++：写文件
来源：http://eln.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jiz.xinyue.icu

[S50] C++：格式化数字
来源：http://zqj.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eof.ehwqpu.com

[S51] C++：显式类型转换
来源：http://goq.hnxiangtu.top

static_cast<double>(a) / b
来源：http://xkm.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://ngr.hcnkem.com

int size() const noexcept { return n_; }
来源：http://ska.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://uqr.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://moi.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://emo.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ynb.c1oappe.top

[S55] C++：结构化绑定
来源：http://ylk.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ubu.yj20258888.top

[S56] C++：optional
来源：http://tiq.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hus.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://iul.zdqjudy.top

constexpr int N = 10;
来源：http://uqn.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://nay.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://tby.havefunace.top

[S59] C++：静态断言
来源：http://uzx.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mgt.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://vxs.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ikn.shangyingyoupin.top

================================================================================
来源：http://rii.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aur.jyoumei.cn

================================================================================
来源：http://hjt.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://wmk.tarul.cn

println("Hello")
来源：http://xle.chenlongwang.top

[T02] Kotlin：变量
来源：http://hbp.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jyf.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://zcl.zdqjudy.top

"值: $b"
来源：http://rya.zhengqikj.top

[T04] Kotlin：空安全
来源：http://xqu.ybcxt.top

val n: String? = null;  n?.length
来源：http://ahb.tanke756.top

[T05] Kotlin：when 表达式
来源：http://xwp.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://trq.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://ktm.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zvi.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://qqm.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ldt.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://eku.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://vnp.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://wxa.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://zrp.ybcxt.top

[T10] Kotlin：默认参数
来源：http://sbo.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iip.gzhubu.top

[T11] Kotlin：协程
来源：http://kkb.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://whk.cashguo.top

[T12] Kotlin：解构声明
来源：http://evl.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://ypb.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://udf.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://abx.gaohongyu789.top

[T14] Kotlin：循环
来源：http://nqs.yj202588.top

for (i in 1..10) println(i)
来源：http://ztn.9152youxi.cn

[T15] Kotlin：接口
来源：http://gox.hesvh.cn

interface Shape { fun area(): Double }
来源：http://lja.316326.xyz

[T16] Swift：Hello World
来源：http://wvg.guannengcc.top

print("Hello")
来源：http://qnf.nanxinkj.top

[T17] Swift：变量与常量
来源：http://jfc.yongpay.top

var a = 1;  let b = 2
来源：http://zsn.dashuyun.cn

[T18] Swift：字符串插值
来源：http://sua.gotoacloud.top

"值: \(b)"
来源：http://kfn.nanxuanxn.top

[T19] Swift：可选绑定
来源：http://kdc.jqgfzy.top

if let n = opt { print(n) }
来源：http://ggc.c1oappe.top

[T20] Swift：数组操作
来源：http://nrw.chenzaomai.com

var a = [1, 2, 3];  a.append(4)
来源：http://tke.xuetiantiany.cn

[T21] Swift：遍历
来源：http://uod.chenzaomai.com

for x in a { print(x) }
来源：http://qji.aizwys.cn

[T22] Swift：字典
来源：http://htc.feifeiyinyue.top

var d = ["a": 1];  d["b"] = 2
来源：http://wnj.haohaochexian.top

[T23] Swift：函数
来源：http://dfz.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://joa.gaohongyu789.top

[T24] Swift：闭包
来源：http://aeu.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://esv.smart0.xyz

[T25] Swift：结构体
来源：http://osq.gzhubu.top

struct P { var x: Int }
来源：http://isc.gotoacloud.top

[T26] Swift：类与重写
来源：http://rhh.9152youxi.cn

class A: Base { override func f() {} }
来源：http://dsb.xuanzx.com

[T27] Swift：错误处理
来源：http://gsi.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://yiz.redwolf501.top

[T28] Swift：枚举
来源：http://qkp.iojbl.cn

enum Color { case red, green }
来源：http://yyp.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://qum.ivvv.top

guard let x = opt else { return }
来源：http://ruz.sjlbkw.cn

[T30] Swift：协议
来源：http://jfd.havefunace.top

protocol Shape { func area() -> Double }
来源：http://gfq.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://mnq.fanxiaobao.xyz

print("Hello")
来源：http://lyi.sysykeji.top

[T32] Lua：局部变量
来源：http://hdr.wangshuangyany.cn

local a = 1
来源：http://qdk.redwolf501.top

[T33] Lua：表（数组）
来源：http://iza.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dry.fehbvm.com

[T34] Lua：遍历表
来源：http://jeh.jinqigfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dmp.nanxinkj.top

[T35] Lua：字典表
来源：http://zeh.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://gfb.gaohongyu789.top

[T36] Lua：函数
来源：http://yfc.nanxuanxn.top

function add(a, b) return a + b end
来源：http://ahx.daxiang520.top

[T37] Lua：字符串拼接
来源：http://djh.bbcook.cn

"a" .. "b"
来源：http://lwn.hfpthk.cn

[T38] Lua：条件
来源：http://xxa.svipenyu.cn

if x > 0 then print("正") end
来源：http://ltd.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://kfx.gzhubu.top

string.find(s, "%d+")
来源：http://cxs.sjlbkw.cn

[T40] Lua：元表
来源：http://hux.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://org.wangdashe.top

[T41] Perl：Hello World
来源：http://dtx.uphjek.com

print "Hello\n";
来源：http://ars.fzhhl.top

[T42] Perl：变量类型
来源：http://gnf.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wsj.tianlin.xyz

[T43] Perl：字符串插值
来源：http://syu.vehdjk.com

"值: $a"
来源：http://lmr.hfpthk.cn

[T44] Perl：条件
来源：http://wwv.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://kmq.cdnleiting.top

[T45] Perl：数组遍历
来源：http://mfx.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://oel.gzhubu.top

[T46] Perl：哈希操作
来源：http://qdt.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ogy.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://ghr.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kpi.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://yyz.tianlin.xyz

$s =~ s/old/new/g;
来源：http://ule.haohaochexian.top

[T49] Perl：函数
来源：http://rut.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zfl.yj20258.top

[T50] Perl：逐行读文件
来源：http://dnd.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://btt.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://sac.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://hgh.dashuyun.cn

println("Hello")
来源：http://rif.316326.xyz

[T52] Scala：变量
来源：http://gmt.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://rdz.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://ysl.zycfv.cn

s"值: $b"
来源：http://ckg.ehwqpu.com

[T54] Scala：集合映射
来源：http://vjw.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://ngm.jqgfzy.top

[T55] Scala：集合过滤
来源：http://lzj.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tsx.vqdsnc.cn

[T56] Scala：样例类
来源：http://unt.yangfankeji.com

case class User(name: String, age: Int)
来源：http://aua.hammf.cn

[T57] Scala：模式匹配
来源：http://gxf.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cbr.9152youxi.cn

[T58] Scala：函数定义
来源：http://rmo.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://jrq.xziqi.cn

[T59] Scala：循环
来源：http://qkw.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://cxr.meibo888.top

[T60] Scala：折叠
来源：http://bkz.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://glw.gotoacloud.top

================================================================================
来源：http://vgu.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xef.fzhhl.top

================================================================================
来源：http://kxw.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://fag.yj20258.top

python -m venv .venv && source .venv/bin/activate
来源：http://rff.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://ool.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ijm.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://ycc.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rmm.zdbjq.cn

[U04] Py：变量调试打印
来源：http://ubd.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://adf.aizwys.cn

[U05] Py：列表去重且保序
来源：http://luh.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://xke.bbcook.cn

[U06] Py：合并两个字典
来源：http://cua.zdqjudy.top

{**a, **b}
来源：http://cxz.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://qmg.sxryk.cn

{v: k for k, v in d.items()}
来源：http://xgl.svipenyu.cn

[U08] Py：展平二维列表
来源：http://xqs.fengsongda.top

[y for x in nested for y in x]
来源：http://ang.havefunace.top

[U09] Py：字典取最大值的键
来源：http://vpd.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://xgq.ctjpmb.com

[U10] Py：按值排序字典
来源：http://sth.jinyuanbaomall.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xrf.hywenlv.cn

[U11] Py：生成器表达式
来源：http://ixn.yonumen.top

(x * 2 for x in arr)
来源：http://rtf.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://pdg.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://qxx.bjfxy.top

[U13] Py：固定长度队列
来源：http://kww.vqdsnc.cn

deque(maxlen=10)
来源：http://utx.yuanzhike.top

[U14] Py：分组收集到列表
来源：http://mdc.fanxiaobao.xyz

defaultdict(list)
来源：http://nij.gogol.net.cn

[U15] Py：高精度计时
来源：http://ycv.fanxiaobao.xyz

t = time.perf_counter()
来源：http://clf.dianchejie.cn

[U16] Py：命令行参数解析
来源：http://hlh.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sfr.hammf.cn

[U17] Py：初始化日志
来源：http://qfc.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://cpt.yj20258888.top

[U18] Py：预编译正则
来源：http://jwh.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://vsv.ivvv.top

[U19] Py：正则替换带回调
来源：http://qel.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xnr.tanke756.top

[U20] Py：缓存函数结果
来源：http://xls.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://dui.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://ybe.xylfe.cn

@contextlib.contextmanager
来源：http://skz.aibaodan.cn

[U22] Py：矩阵转置
来源：http://viy.52xcode.cn

list(zip(*m))
来源：http://zgy.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://aip.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sch.316326.xyz

[U24] Py：路径操作
来源：http://ogy.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qhn.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://elk.tianlin.xyz

csv.DictReader(f)
来源：http://tww.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://gea.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ath.uphjek.com

[U27] Py：异步 HTTP
来源：http://vvp.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://xgv.jyoumei.cn

[U28] Py：类型别名
来源：http://hjz.jinqigfzy.top

UserId = int
来源：http://vbd.ydzc1.top

[U29] Py：属性校验
来源：http://jif.hesvh.cn

@property 与 @x.setter 配合
来源：http://tpk.yj20258888.top

[U30] Py：数据类
来源：http://pig.zhijiandao.cn

@dataclass(slots=True)
来源：http://pdu.zhengqikj.top

[U31] Py：单测
来源：http://xdv.gzhubu.top

python -m pytest -q
来源：http://bdw.zhoulong.xyz

[U32] Py：代码格式化
来源：http://hsg.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://lug.havefunace.top

[U33] Py：打包发布
来源：http://xbt.epnwcf.com

python -m build  （依赖 pyproject.toml）
来源：http://ygy.shanyushiyangtech.top

[U34] Py：判断编码
来源：http://tms.ehwqpu.com

chardet.detect(raw)
来源：http://cdo.yj202588.top

[U35] Py：发送邮件
来源：http://whp.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qrx.redwolf501.top

[U36] Py：定时任务
来源：http://dkw.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://whb.zdqjudy.top

[U37] Py：读写 Excel
来源：http://lvi.kuanghao11.cn

pandas.read_excel / DataFrame.to_excel
来源：http://syj.shanyushiyangtech.top

[U38] Py：获取脚本所在目录
来源：http://qwa.nwbrower.top

Path(__file__).resolve().parent
来源：http://bds.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://vje.hnqzz.top

sys.stdout.isatty()
来源：http://rjg.tarul.cn

[U40] Py：打印到标准错误
来源：http://yfi.shzxlz.cn

print("err", file=sys.stderr)
来源：http://kvx.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://ysv.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zkr.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://zut.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hbk.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://cvm.vqdsnc.cn

namespace App\Http;
来源：http://dcd.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://uha.zhijiandao.cn

declare(strict_types=1);
来源：http://qve.zhongyouzk.top

[U45] PHP：类型声明与返回类型
来源：http://jik.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pwd.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://lnd.xinyue.icu

?string $name = null
来源：http://nfv.hnqzz.top

[U47] PHP：联合类型
来源：http://tjb.tian-w.cn

int|string $id
来源：http://shs.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://inr.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qfe.hcnkem.com

[U49] PHP：只读属性
来源：http://equ.sjlbkw.cn

public readonly string $name
来源：http://zvw.ivvv.top

[U50] PHP：构造器属性提升
来源：http://mgh.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://iym.shzxlz.cn

[U51] PHP：数组解构
来源：http://cjg.hesvh.cn

[$a, $b] = $arr;
来源：http://fnu.hesvh.cn

[U52] PHP：箭头函数
来源：http://ofq.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://wwy.andypj.xyz

[U53] PHP：空合并运算符
来源：http://fub.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://kou.pycfn.com

[U54] PHP：空安全调用
来源：http://kow.xuanzx.com

$obj?->method()
来源：http://hin.cheryme.top

[U55] PHP：match 表达式
来源：http://mpp.yj202588.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yyu.mhx1999.top

[U56] PHP：命名参数
来源：http://spg.yfazqb.com

f(a: 1, b: 2)
来源：http://kfh.vqdsnc.cn

[U57] PHP：字符串插值
来源：http://jng.jinghuilouyu.cn

"值: {$a}"
来源：http://wml.xuanzx.com

[U58] PHP：数组三件套
来源：http://pbb.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lvi.jinghuilouyu.cn


<!-- 参考信息 -->