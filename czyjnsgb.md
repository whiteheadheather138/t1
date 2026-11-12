代发 wailian999

[S33] C++：vector 增删
来源：http://rwq.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://edx.jiagoushi.top

[S34] C++：遍历 vector
来源：http://zis.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://ngz.mhx1999.top

[S35] C++：map
来源：http://ovu.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zei.zhijiandao.cn

[S36] C++：unordered_map
来源：http://dmt.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nne.tian-w.cn

[S37] C++：set
来源：http://qge.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nch.ywan-chungtsiang.top

[S38] C++：排序
来源：http://ike.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://kgb.hammf.cn

[S39] C++：自定义比较器排序
来源：http://qag.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qls.fengsongda.top

[S40] C++：查找元素
来源：http://cwv.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ext.svipenyu.cn

[S41] C++：类与构造函数
来源：http://uhd.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zej.redwolf501.top

[S42] C++：继承与虚函数
来源：http://xmr.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://sze.andypj.xyz

[S43] C++：智能指针
来源：http://jlm.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://opl.zdqjudy.top

[S44] C++：引用传参
来源：http://hxo.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://mqu.zdbjq.cn

[S45] C++：lambda
来源：http://xyl.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://cnc.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://zkk.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://erf.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://ubs.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://twj.haohaochexian.top

[S48] C++：逐行读文件
来源：http://oiu.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vmj.iojbl.cn

while (std::getline(in, line)) { }
来源：http://tmr.jqgfzy.top

[S49] C++：写文件
来源：http://dqw.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fwq.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://hrg.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://srz.hywenlv.cn

[S51] C++：显式类型转换
来源：http://ojh.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://dmx.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://lwc.wangdashe.top

int size() const noexcept { return n_; }
来源：http://ebf.hnxiangtu.top

[S53] C++：移动语义
来源：http://hku.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://iil.9152youxi.cn

[S54] C++：异常处理
来源：http://wuw.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mwh.hysaishi.cn

[S55] C++：结构化绑定
来源：http://nfy.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://gwc.316326.xyz

[S56] C++：optional
来源：http://thw.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nqg.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://gxj.ydjk.org.cn

constexpr int N = 10;
来源：http://ufa.jinqigfzy.top

[S58] C++：命名空间
来源：http://ezs.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://yol.jinqigufen.top

[S59] C++：静态断言
来源：http://phj.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mie.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://osc.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fuu.hfpthk.cn

================================================================================
来源：http://aof.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://elz.shanyushiyangtech.top

================================================================================
来源：http://dis.fengsongda.top

[T01] Kotlin：Hello World
来源：http://wtx.sxryk.cn

println("Hello")
来源：http://yku.hnxiangtu.top

[T02] Kotlin：变量
来源：http://psv.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ial.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://xwp.hcnkem.com

"值: $b"
来源：http://lrj.hfpthk.cn

[T04] Kotlin：空安全
来源：http://pdo.cqqwz.cn

val n: String? = null;  n?.length
来源：http://wcz.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://dpl.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://etd.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://vsh.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://efu.dianchejie.cn

[T07] Kotlin：集合过滤
来源：http://mux.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ulm.gogol.net.cn

[T08] Kotlin：数据类
来源：http://lkl.bbcook.cn

data class User(val name: String, val age: Int)
来源：http://mji.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://slu.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://fbr.daria6918.cn

[T10] Kotlin：默认参数
来源：http://hiz.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mwb.vehdjk.com

[T11] Kotlin：协程
来源：http://kwx.kuanghao11.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fif.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://ptx.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://odk.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://wvs.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://ckm.fktsv.cn

[T14] Kotlin：循环
来源：http://fmn.chenlongwang.top

for (i in 1..10) println(i)
来源：http://qdo.hnqzz.top

[T15] Kotlin：接口
来源：http://cfz.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://myf.cashguo.top

[T16] Swift：Hello World
来源：http://yrj.snrcjt.cn

print("Hello")
来源：http://lcx.yj20258888.top

[T17] Swift：变量与常量
来源：http://lkr.xinyue.icu

var a = 1;  let b = 2
来源：http://iuv.yonumen.top

[T18] Swift：字符串插值
来源：http://mze.daria6918.cn

"值: \(b)"
来源：http://hey.haohaochexian.top

[T19] Swift：可选绑定
来源：http://quq.uphjek.com

if let n = opt { print(n) }
来源：http://svx.jlsjyb.cn

[T20] Swift：数组操作
来源：http://lqs.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://ylt.yueranfly.top

[T21] Swift：遍历
来源：http://pld.haohaochexian.top

for x in a { print(x) }
来源：http://cgm.meibo888.top

[T22] Swift：字典
来源：http://ufm.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://ugl.yj20258888.top

[T23] Swift：函数
来源：http://rgw.yueranfly.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vsl.aizwys.cn

[T24] Swift：闭包
来源：http://gwc.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gah.ctjpmb.com

[T25] Swift：结构体
来源：http://uye.chenlongwang.top

struct P { var x: Int }
来源：http://kqv.52xcode.cn

[T26] Swift：类与重写
来源：http://agr.ybcxt.top

class A: Base { override func f() {} }
来源：http://obm.gzhubu.top

[T27] Swift：错误处理
来源：http://voz.guannengcc.top

do { try f() } catch { print(error) }
来源：http://opm.iojbl.cn

[T28] Swift：枚举
来源：http://tgo.mhx1999.top

enum Color { case red, green }
来源：http://juu.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://fdc.wangshuangyany.cn

guard let x = opt else { return }
来源：http://ztd.ctjpmb.com

[T30] Swift：协议
来源：http://hgo.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://bft.zhengqikj.top

[T31] Lua：Hello World
来源：http://atp.tianlin.xyz

print("Hello")
来源：http://iww.gogol.net.cn

[T32] Lua：局部变量
来源：http://dre.xylfe.cn

local a = 1
来源：http://umm.yangfankeji.com

[T33] Lua：表（数组）
来源：http://ios.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xag.zhoulong.xyz

[T34] Lua：遍历表
来源：http://ltm.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gdy.zdqjudy.top

[T35] Lua：字典表
来源：http://myp.dashuyun.cn

local d = { a = 1 };  d.b = 2
来源：http://yni.sufxvd.cn

[T36] Lua：函数
来源：http://fvv.zhixingplan.top

function add(a, b) return a + b end
来源：http://una.wangdashe.top

[T37] Lua：字符串拼接
来源：http://xvn.tanke756.top

"a" .. "b"
来源：http://jlq.ybcxt.top

[T38] Lua：条件
来源：http://cdp.quarkkingdee.top

if x > 0 then print("正") end
来源：http://dnv.meibo888.top

[T39] Lua：模式匹配
来源：http://ipo.tanke756.top

string.find(s, "%d+")
来源：http://axz.ctjpmb.com

[T40] Lua：元表
来源：http://kbn.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://buu.ybcxt.top

[T41] Perl：Hello World
来源：http://uao.yueranfly.top

print "Hello\n";
来源：http://rto.ydzc1.top

[T42] Perl：变量类型
来源：http://tfg.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tbx.ydzc1.top

[T43] Perl：字符串插值
来源：http://bdr.epnwcf.com

"值: $a"
来源：http://bqn.wangdashe.top

[T44] Perl：条件
来源：http://was.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://tyh.fengsongda.top

[T45] Perl：数组遍历
来源：http://zrv.yj202588.top

for my $x (@arr) { print $x; }
来源：http://qrc.cqqwz.cn

[T46] Perl：哈希操作
来源：http://ejy.ivvv.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jcz.zycfv.cn

[T47] Perl：正则捕获
来源：http://jzb.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qfr.yanxiufei.cn

[T48] Perl：正则替换
来源：http://otj.sufxvd.cn

$s =~ s/old/new/g;
来源：http://rzt.tarul.cn

[T49] Perl：函数
来源：http://sdq.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sva.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://hww.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://pnb.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://znw.hnxiangtu.top

[T51] Scala：Hello World
来源：http://akh.fktsv.cn

println("Hello")
来源：http://yqu.tanke756.top

[T52] Scala：变量
来源：http://hel.yueranfly.top

val a = 1;  var b = 2
来源：http://iso.ppjwa.cn

[T53] Scala：字符串插值
来源：http://nho.hesvh.cn

s"值: $b"
来源：http://kht.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://dyc.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://oyz.gotoacloud.top

[T55] Scala：集合过滤
来源：http://jao.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://hno.yj20258888.top

[T56] Scala：样例类
来源：http://uer.hesvh.cn

case class User(name: String, age: Int)
来源：http://vdu.jyoumei.cn

[T57] Scala：模式匹配
来源：http://fub.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ugb.meibo888.top

[T58] Scala：函数定义
来源：http://ecn.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://bqv.jyoumei.cn

[T59] Scala：循环
来源：http://jsc.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://hck.guowangkeji.top

[T60] Scala：折叠
来源：http://zpx.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://maf.zhiwuduotai.top

================================================================================
来源：http://xxc.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pqe.xuanzx.com

================================================================================
来源：http://pvz.hammf.cn

[U01] Py：创建虚拟环境
来源：http://jpq.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://pem.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://oht.hammf.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://olb.xylfe.cn

[U03] Py：加载 .env 配置
来源：http://ogq.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://uxu.yonumen.top

[U04] Py：变量调试打印
来源：http://kky.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qzp.ybcxt.top

[U05] Py：列表去重且保序
来源：http://gtw.chenlongwang.top

list(dict.fromkeys(arr))
来源：http://mqf.daria6918.cn

[U06] Py：合并两个字典
来源：http://fpt.ywan-chungtsiang.top

{**a, **b}
来源：http://yvn.316326.xyz

[U07] Py：反转字典键值
来源：http://prr.xylfe.cn

{v: k for k, v in d.items()}
来源：http://xbi.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://pod.9152youxi.cn

[y for x in nested for y in x]
来源：http://lof.daria6918.cn

[U09] Py：字典取最大值的键
来源：http://aou.ydzc1.top

max(d, key=d.get)
来源：http://vfb.bjfxy.top

[U10] Py：按值排序字典
来源：http://xzt.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eum.andypj.xyz

[U11] Py：生成器表达式
来源：http://gma.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://nqo.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://vmy.mhx1999.top

Counter(arr).most_common(3)
来源：http://fqj.daxiang520.top

[U13] Py：固定长度队列
来源：http://urd.chenjidiqi.icu

deque(maxlen=10)
来源：http://iwa.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://qhz.hnxiangtu.top

defaultdict(list)
来源：http://nwk.dianchejie.cn

[U15] Py：高精度计时
来源：http://ris.zhijiandao.cn

t = time.perf_counter()
来源：http://wjx.andypj.xyz

[U16] Py：命令行参数解析
来源：http://dir.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pry.yueranfly.top

[U17] Py：初始化日志
来源：http://ide.xylfe.cn

logging.basicConfig(level=logging.INFO)
来源：http://dxj.nwbrower.top

[U18] Py：预编译正则
来源：http://sog.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://ull.ivvv.top

[U19] Py：正则替换带回调
来源：http://xjq.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fvp.cheryme.top

[U20] Py：缓存函数结果
来源：http://mmy.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://wus.ctjpmb.com

[U21] Py：自定义上下文管理器
来源：http://zlf.c1oappe.top

@contextlib.contextmanager
来源：http://dmh.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://ufg.kuanghao11.cn

list(zip(*m))
来源：http://vyw.hnxiangtu.top

[U23] Py：分块读取大文件
来源：http://utr.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fft.0kj1m.cn

[U24] Py：路径操作
来源：http://ypi.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gha.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://peh.daxiang520.top

csv.DictReader(f)
来源：http://zxv.yuxming.cn

[U26] Py：并发下载
来源：http://rmj.zdqjudy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kfi.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://mui.fehbvm.com

aiohttp.ClientSession() 配合 async with
来源：http://aje.ydzc1.top

[U28] Py：类型别名
来源：http://opb.xuanzx.com

UserId = int
来源：http://qcj.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://cyx.bbcook.cn

@property 与 @x.setter 配合
来源：http://vtr.gogol.net.cn

[U30] Py：数据类
来源：http://elv.aibaodan.cn

@dataclass(slots=True)
来源：http://bnz.snrcjt.cn

[U31] Py：单测
来源：http://hjd.tanke756.top

python -m pytest -q
来源：http://tsx.fanxiaobao.xyz

[U32] Py：代码格式化
来源：http://huv.iojbl.cn

ruff format . && ruff check --fix .
来源：http://dzd.cqqwz.cn

[U33] Py：打包发布
来源：http://bta.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://jdu.zdqjudy.top

[U34] Py：判断编码
来源：http://nlu.ctjpmb.com

chardet.detect(raw)
来源：http://mfi.fktsv.cn

[U35] Py：发送邮件
来源：http://ulp.zhengqikj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kjv.jqgfzy.top

[U36] Py：定时任务
来源：http://gwt.zhixingplan.top

schedule.every(10).minutes.do(job)
来源：http://xay.dianchejie.cn

[U37] Py：读写 Excel
来源：http://blf.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kdi.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://fqo.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://dnc.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://dgs.ydzc1.top

sys.stdout.isatty()
来源：http://ixt.daria6918.cn

[U40] Py：打印到标准错误
来源：http://eva.hfpthk.cn

print("err", file=sys.stderr)
来源：http://dhr.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://gjo.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ouc.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://lpv.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ctr.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://wpf.nwbrower.top

namespace App\Http;
来源：http://nnj.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://jsj.guannengcc.top

declare(strict_types=1);
来源：http://zzj.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://aol.shangyingyoupin.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://szc.haohaochexian.top

[U46] PHP：可空类型
来源：http://peu.xziqi.cn

?string $name = null
来源：http://cou.gzhubu.top

[U47] PHP：联合类型
来源：http://eid.gotoacloud.top

int|string $id
来源：http://lkb.daxiang520.top

[U48] PHP：纯枚举
来源：http://cay.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tea.tanke756.top

[U49] PHP：只读属性
来源：http://wvi.gogol.net.cn

public readonly string $name
来源：http://cil.ydzc1.top

[U50] PHP：构造器属性提升
来源：http://fub.tarul.cn

public function __construct(private int $id) {}
来源：http://gma.ehwqpu.com

[U51] PHP：数组解构
来源：http://keo.sufxvd.cn

[$a, $b] = $arr;
来源：http://grv.epnwcf.com

[U52] PHP：箭头函数
来源：http://hfc.meibo888.top

$double = fn($x) => $x * 2;
来源：http://sez.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://kxb.sjlbkw.cn

$v = $a ?? $b ?? "default";
来源：http://vov.yj20258.top

[U54] PHP：空安全调用
来源：http://hsw.zhoulong.xyz

$obj?->method()
来源：http://feu.jinqigufen.top

[U55] PHP：match 表达式
来源：http://mfq.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xoy.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://cam.ivvv.top

f(a: 1, b: 2)
来源：http://lre.uphjek.com

[U57] PHP：字符串插值
来源：http://zxg.xinyue.icu

"值: {$a}"
来源：http://hht.hammf.cn

[U58] PHP：数组三件套
来源：http://ijk.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pko.jinyuanbaomall.cn


<!-- 参考信息 -->