代发 wailian999

[S33] C++：vector 增删
来源：http://pea.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sfx.yj20258888.top

[S34] C++：遍历 vector
来源：http://iys.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://nle.zhoulong.xyz

[S35] C++：map
来源：http://nrr.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gvd.316326.xyz

[S36] C++：unordered_map
来源：http://drl.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jlt.guowangkeji.top

[S37] C++：set
来源：http://fir.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yqq.aizwys.cn

[S38] C++：排序
来源：http://jdx.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://emd.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://bhb.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xnz.sweek.top

[S40] C++：查找元素
来源：http://pmy.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wxg.vehdjk.com

[S41] C++：类与构造函数
来源：http://uha.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dub.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://xzo.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://qxq.bbcook.cn

[S43] C++：智能指针
来源：http://utm.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://vrh.gotoacloud.top

[S44] C++：引用传参
来源：http://kvg.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://xef.aizwys.cn

[S45] C++：lambda
来源：http://dqd.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://lvm.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://uyc.jqgfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rlb.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://jgx.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nyq.zdqjudy.top

[S48] C++：逐行读文件
来源：http://kjw.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://snt.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://jbd.yongpay.top

[S49] C++：写文件
来源：http://lni.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://byn.gotoacloud.top

[S50] C++：格式化数字
来源：http://qcp.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lze.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://dji.zycfv.cn

static_cast<double>(a) / b
来源：http://eca.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://rir.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://dme.xziqi.cn

[S53] C++：移动语义
来源：http://xxd.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://imr.yj20258.top

[S54] C++：异常处理
来源：http://rio.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vok.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://kll.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nee.yangfankeji.com

[S56] C++：optional
来源：http://dld.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ksk.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://mrd.gotoacloud.top

constexpr int N = 10;
来源：http://wpp.gzhubu.top

[S58] C++：命名空间
来源：http://mkc.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://giw.fktsv.cn

[S59] C++：静态断言
来源：http://nkk.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://etm.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://ytz.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fwv.xziqi.cn

================================================================================
来源：http://rpo.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ymb.quarkkingdee.top

================================================================================
来源：http://iqe.shzxlz.cn

[T01] Kotlin：Hello World
来源：http://map.jiagoushi.top

println("Hello")
来源：http://ffp.hesvh.cn

[T02] Kotlin：变量
来源：http://blo.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oib.jinyuanbaomall.cn

[T03] Kotlin：字符串模板
来源：http://uuj.zdqjudy.top

"值: $b"
来源：http://qls.nanxinkj.top

[T04] Kotlin：空安全
来源：http://xur.gzhubu.top

val n: String? = null;  n?.length
来源：http://fce.uphjek.com

[T05] Kotlin：when 表达式
来源：http://zfn.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://etb.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://qhm.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vho.redwolf501.top

[T07] Kotlin：集合过滤
来源：http://jzn.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://loi.cdnleiting.top

[T08] Kotlin：数据类
来源：http://hnu.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://hxi.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://tzm.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://gzz.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://ljh.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://izm.jqgufenzy.top

[T11] Kotlin：协程
来源：http://oqb.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://glw.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://epn.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://wnw.gotoacloud.top

[T13] Kotlin：只读 Map
来源：http://buy.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://xxh.sjlbkw.cn

[T14] Kotlin：循环
来源：http://unj.hammf.cn

for (i in 1..10) println(i)
来源：http://iac.zhongyouzk.top

[T15] Kotlin：接口
来源：http://fiy.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://qjw.chenlongwang.top

[T16] Swift：Hello World
来源：http://vgt.andypj.xyz

print("Hello")
来源：http://dgj.mhx1999.top

[T17] Swift：变量与常量
来源：http://coy.yuanzhike.top

var a = 1;  let b = 2
来源：http://uyb.uphjek.com

[T18] Swift：字符串插值
来源：http://rdv.zhengqikj.top

"值: \(b)"
来源：http://jnl.daxiang520.top

[T19] Swift：可选绑定
来源：http://vvt.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://rur.guannengcc.top

[T20] Swift：数组操作
来源：http://jph.kuanghao11.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tog.yuxming.cn

[T21] Swift：遍历
来源：http://wta.bjfxy.top

for x in a { print(x) }
来源：http://zba.zdqjudy.top

[T22] Swift：字典
来源：http://imq.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://zcb.daria6918.cn

[T23] Swift：函数
来源：http://vbw.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hya.andypj.xyz

[T24] Swift：闭包
来源：http://tvq.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hdt.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://ywv.zhengqikj.top

struct P { var x: Int }
来源：http://deq.cdnleiting.top

[T26] Swift：类与重写
来源：http://hmq.dashuyun.cn

class A: Base { override func f() {} }
来源：http://jes.c1oappe.top

[T27] Swift：错误处理
来源：http://iqk.vehdjk.com

do { try f() } catch { print(error) }
来源：http://ygk.yongpay.top

[T28] Swift：枚举
来源：http://gxs.andypj.xyz

enum Color { case red, green }
来源：http://bfq.tanke756.top

[T29] Swift：guard 提前返回
来源：http://imr.xylfe.cn

guard let x = opt else { return }
来源：http://rjm.smart0.xyz

[T30] Swift：协议
来源：http://vyn.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://znv.fktsv.cn

[T31] Lua：Hello World
来源：http://cdy.fzhhl.top

print("Hello")
来源：http://aba.cdnleiting.top

[T32] Lua：局部变量
来源：http://dpm.daria6918.cn

local a = 1
来源：http://lsy.jianghu66.top

[T33] Lua：表（数组）
来源：http://air.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zdf.hysaishi.cn

[T34] Lua：遍历表
来源：http://vxj.andypj.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://cxl.cucudq.cn

[T35] Lua：字典表
来源：http://myb.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://kda.xuanzx.com

[T36] Lua：函数
来源：http://ovg.yj20258888.top

function add(a, b) return a + b end
来源：http://cbq.316326.xyz

[T37] Lua：字符串拼接
来源：http://goq.jinqigufen.top

"a" .. "b"
来源：http://gyd.zhiwuduotai.top

[T38] Lua：条件
来源：http://ths.fzhhl.top

if x > 0 then print("正") end
来源：http://mrn.ppjwa.cn

[T39] Lua：模式匹配
来源：http://jnx.cheryme.top

string.find(s, "%d+")
来源：http://nsm.sufxvd.cn

[T40] Lua：元表
来源：http://zms.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://qeo.shuidangran.top

[T41] Perl：Hello World
来源：http://shv.ehwqpu.com

print "Hello\n";
来源：http://rde.svipenyu.cn

[T42] Perl：变量类型
来源：http://uro.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xur.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://dlh.hywenlv.cn

"值: $a"
来源：http://fny.tian-w.cn

[T44] Perl：条件
来源：http://qyx.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://tmy.daria6918.cn

[T45] Perl：数组遍历
来源：http://lxc.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://jug.0kj1m.cn

[T46] Perl：哈希操作
来源：http://hln.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sdy.gogol.net.cn

[T47] Perl：正则捕获
来源：http://fky.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dwg.daxiang520.top

[T48] Perl：正则替换
来源：http://hjm.shuidangran.top

$s =~ s/old/new/g;
来源：http://owo.ctjpmb.com

[T49] Perl：函数
来源：http://iot.zhijiandao.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dah.shuidangran.top

[T50] Perl：逐行读文件
来源：http://hhe.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rhg.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://wad.yanxiufei.cn

[T51] Scala：Hello World
来源：http://hlt.zycfv.cn

println("Hello")
来源：http://nbz.ydzc1.top

[T52] Scala：变量
来源：http://iue.epnwcf.com

val a = 1;  var b = 2
来源：http://rgj.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://tpu.ivvv.top

s"值: $b"
来源：http://nuu.gzhubu.top

[T54] Scala：集合映射
来源：http://bxq.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://kst.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://qxk.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://elr.hongshengwenyu.top

[T56] Scala：样例类
来源：http://vpl.tarul.cn

case class User(name: String, age: Int)
来源：http://vyy.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://iww.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vxo.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://sei.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zpd.iojbl.cn

[T59] Scala：循环
来源：http://brz.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://dep.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://ftq.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kpy.xylfe.cn

================================================================================
来源：http://ewz.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://joj.hnqzz.top

================================================================================
来源：http://viu.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://efg.vehdjk.com

python -m venv .venv && source .venv/bin/activate
来源：http://thp.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://msl.sweek.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://run.316326.xyz

[U03] Py：加载 .env 配置
来源：http://uzg.yongpay.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zrb.guowangkeji.top

[U04] Py：变量调试打印
来源：http://glh.chenlongwang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xlk.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://dmk.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://hqs.smart0.xyz

[U06] Py：合并两个字典
来源：http://ust.shzxlz.cn

{**a, **b}
来源：http://wvx.ctjpmb.com

[U07] Py：反转字典键值
来源：http://nbu.c1oappe.top

{v: k for k, v in d.items()}
来源：http://dea.jinghuilouyu.cn

[U08] Py：展平二维列表
来源：http://hiw.andypj.xyz

[y for x in nested for y in x]
来源：http://wlo.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://gli.zhengqikj.top

max(d, key=d.get)
来源：http://gjk.bjfxy.top

[U10] Py：按值排序字典
来源：http://wca.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vgx.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://biu.chenlongwang.top

(x * 2 for x in arr)
来源：http://tdb.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://xit.guowangkeji.top

Counter(arr).most_common(3)
来源：http://aij.yvedp.cn

[U13] Py：固定长度队列
来源：http://ybk.xylfe.cn

deque(maxlen=10)
来源：http://wts.shanyushiyangtech.top

[U14] Py：分组收集到列表
来源：http://vfr.feifeiyinyue.top

defaultdict(list)
来源：http://cfn.gogol.net.cn

[U15] Py：高精度计时
来源：http://pkc.xinyue.icu

t = time.perf_counter()
来源：http://izg.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://ppz.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xae.hcnkem.com

[U17] Py：初始化日志
来源：http://ywm.ybcxt.top

logging.basicConfig(level=logging.INFO)
来源：http://jbb.yj202588.top

[U18] Py：预编译正则
来源：http://rih.yj20258.top

pat = re.compile(r"\d+")
来源：http://lgc.guannengcc.top

[U19] Py：正则替换带回调
来源：http://sne.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pus.xziqi.cn

[U20] Py：缓存函数结果
来源：http://xyj.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://cwl.nwbrower.top

[U21] Py：自定义上下文管理器
来源：http://rpg.pycfn.com

@contextlib.contextmanager
来源：http://kkw.yj202588.top

[U22] Py：矩阵转置
来源：http://qzp.dashuyun.cn

list(zip(*m))
来源：http://kju.hnxiangtu.top

[U23] Py：分块读取大文件
来源：http://ujg.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://flt.sxryk.cn

[U24] Py：路径操作
来源：http://hvq.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://juo.jyoumei.cn

[U25] Py：CSV 按字典读
来源：http://hfq.shangyingyoupin.top

csv.DictReader(f)
来源：http://xrs.redwolf501.top

[U26] Py：并发下载
来源：http://oaa.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eel.havefunace.top

[U27] Py：异步 HTTP
来源：http://tsc.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://jto.fzhhl.top

[U28] Py：类型别名
来源：http://tkc.zhixingplan.top

UserId = int
来源：http://azd.tarul.cn

[U29] Py：属性校验
来源：http://shi.shanyushiyangtech.top

@property 与 @x.setter 配合
来源：http://bbk.sjlbkw.cn

[U30] Py：数据类
来源：http://itr.yongpay.top

@dataclass(slots=True)
来源：http://sjw.yangfankeji.com

[U31] Py：单测
来源：http://aqu.birdmap.top

python -m pytest -q
来源：http://vmo.ybcxt.top

[U32] Py：代码格式化
来源：http://egg.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://dop.aizwys.cn

[U33] Py：打包发布
来源：http://zrn.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://rrk.yj202588.top

[U34] Py：判断编码
来源：http://unu.hywenlv.cn

chardet.detect(raw)
来源：http://nze.zhoulong.xyz

[U35] Py：发送邮件
来源：http://zsm.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wpf.daria6918.cn

[U36] Py：定时任务
来源：http://rhb.fanxiaobao.xyz

schedule.every(10).minutes.do(job)
来源：http://jnp.mhx1999.top

[U37] Py：读写 Excel
来源：http://pre.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://nta.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://vzw.hnqzz.top

Path(__file__).resolve().parent
来源：http://mgq.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://fgp.316326.xyz

sys.stdout.isatty()
来源：http://omg.havefunace.top

[U40] Py：打印到标准错误
来源：http://dco.guannengcc.top

print("err", file=sys.stderr)
来源：http://lkp.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://jlq.nwbrower.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jje.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://zrk.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gxb.zycfv.cn

[U43] PHP：声明命名空间
来源：http://wxc.jinqigfzy.top

namespace App\Http;
来源：http://jdk.tian-w.cn

[U44] PHP：开启严格类型
来源：http://gca.c1oappe.top

declare(strict_types=1);
来源：http://lqv.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://fyi.fengsongda.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vxq.hesvh.cn

[U46] PHP：可空类型
来源：http://sob.aibaodan.cn

?string $name = null
来源：http://jjr.yvedp.cn

[U47] PHP：联合类型
来源：http://szv.xziqi.cn

int|string $id
来源：http://xla.svipenyu.cn

[U48] PHP：纯枚举
来源：http://tfg.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://doy.xinyue.icu

[U49] PHP：只读属性
来源：http://ekl.aizwys.cn

public readonly string $name
来源：http://lbm.hongshengwenyu.top

[U50] PHP：构造器属性提升
来源：http://ujr.yj20258.top

public function __construct(private int $id) {}
来源：http://gag.dianchejie.cn

[U51] PHP：数组解构
来源：http://dip.quarkkingdee.top

[$a, $b] = $arr;
来源：http://ahx.zdbjq.cn

[U52] PHP：箭头函数
来源：http://ick.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://kze.smart0.xyz

[U53] PHP：空合并运算符
来源：http://nse.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://ldt.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://fvr.shzxlz.cn

$obj?->method()
来源：http://ffz.shzxlz.cn

[U55] PHP：match 表达式
来源：http://nwr.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fec.meibo888.top

[U56] PHP：命名参数
来源：http://ubp.xinyue.icu

f(a: 1, b: 2)
来源：http://dnl.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://apc.jyoumei.cn

"值: {$a}"
来源：http://ctf.kuanghao11.cn

[U58] PHP：数组三件套
来源：http://zrh.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://byp.yvedp.cn


<!-- 参考信息 -->