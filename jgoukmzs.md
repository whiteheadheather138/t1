代发 wailian999

[S35] C++：map
来源：http://sde.cheryme.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hlv.yueranfly.top

[S36] C++：unordered_map
来源：http://mwm.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vil.gaohongyu789.top

[S37] C++：set
来源：http://zgq.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jjj.tarul.cn

[S38] C++：排序
来源：http://kxr.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://vnk.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://hus.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://faf.hysaishi.cn

[S40] C++：查找元素
来源：http://psh.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eoh.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://nap.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cbr.bjfxy.top

[S42] C++：继承与虚函数
来源：http://fgg.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://cgy.ybcxt.top

[S43] C++：智能指针
来源：http://ydf.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://ceb.yueranfly.top

[S44] C++：引用传参
来源：http://akk.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://zhi.vehdjk.com

[S45] C++：lambda
来源：http://jaz.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://irh.tian-w.cn

[S46] C++：函数模板
来源：http://rjm.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bcm.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://nrc.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lnu.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://fxw.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://ruq.52xcode.cn

while (std::getline(in, line)) { }
来源：http://dch.ydzc1.top

[S49] C++：写文件
来源：http://jiy.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uca.wangdashe.top

[S50] C++：格式化数字
来源：http://ryl.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gpz.jiagoushi.top

[S51] C++：显式类型转换
来源：http://slu.jlsjyb.cn

static_cast<double>(a) / b
来源：http://unl.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://ehf.bjfxy.top

int size() const noexcept { return n_; }
来源：http://yqc.feifeiyinyue.top

[S53] C++：移动语义
来源：http://vjn.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://uwp.xuanzx.com

[S54] C++：异常处理
来源：http://zvm.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jdw.haohaochexian.top

[S55] C++：结构化绑定
来源：http://msd.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xdb.fanxiaobao.xyz

[S56] C++：optional
来源：http://chv.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://itl.zycfv.cn

[S57] C++：编译期常量
来源：http://yjv.jinqigfzy.top

constexpr int N = 10;
来源：http://fur.yfazqb.com

[S58] C++：命名空间
来源：http://ruy.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://zpj.pengpengdd.cyou

[S59] C++：静态断言
来源：http://wmy.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dqn.yongpay.top

[S60] C++：遍历并删除元素
来源：http://fiw.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bok.ctjpmb.com

================================================================================
来源：http://pvx.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://avs.cucudq.cn

================================================================================
来源：http://hif.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://qmh.sjlbkw.cn

println("Hello")
来源：http://ume.sweek.top

[T02] Kotlin：变量
来源：http://uci.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xwi.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://cbr.hywenlv.cn

"值: $b"
来源：http://wns.hongshengwenyu.top

[T04] Kotlin：空安全
来源：http://hqj.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://oym.meibo888.top

[T05] Kotlin：when 表达式
来源：http://xba.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lmc.fengsongda.top

[T06] Kotlin：集合映射
来源：http://yen.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qdz.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://tze.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tfj.tianlin.xyz

[T08] Kotlin：数据类
来源：http://usm.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://ihl.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://eua.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://pib.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://pcj.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://aor.hammf.cn

[T11] Kotlin：协程
来源：http://exo.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vif.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://col.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://klh.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://txg.pycfn.com

val m = mapOf("a" to 1)
来源：http://wrp.ivvv.top

[T14] Kotlin：循环
来源：http://cxm.pengpengdd.cyou

for (i in 1..10) println(i)
来源：http://gyg.316326.xyz

[T15] Kotlin：接口
来源：http://zmy.uphjek.com

interface Shape { fun area(): Double }
来源：http://mlo.zhengqikj.top

[T16] Swift：Hello World
来源：http://bjn.jinyuanbaomall.cn

print("Hello")
来源：http://yzo.ydzc1.top

[T17] Swift：变量与常量
来源：http://ytf.zhongyouzk.top

var a = 1;  let b = 2
来源：http://qgg.jqgfzy.top

[T18] Swift：字符串插值
来源：http://ywv.hywenlv.cn

"值: \(b)"
来源：http://hik.chenzaomai.com

[T19] Swift：可选绑定
来源：http://wir.ybcxt.top

if let n = opt { print(n) }
来源：http://muf.jlsjyb.cn

[T20] Swift：数组操作
来源：http://zde.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ncj.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://ion.shangyingyoupin.top

for x in a { print(x) }
来源：http://gkh.ppjwa.cn

[T22] Swift：字典
来源：http://ccr.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vbf.hammf.cn

[T23] Swift：函数
来源：http://slo.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uki.tanke756.top

[T24] Swift：闭包
来源：http://vfl.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iwd.yuxming.cn

[T25] Swift：结构体
来源：http://rjq.vqdsnc.cn

struct P { var x: Int }
来源：http://aen.sjlbkw.cn

[T26] Swift：类与重写
来源：http://nga.yangfankeji.com

class A: Base { override func f() {} }
来源：http://smx.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://nhz.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://rks.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://mli.wangdashe.top

enum Color { case red, green }
来源：http://rpb.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://eln.shangyingyoupin.top

guard let x = opt else { return }
来源：http://eal.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://cxv.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://fyg.birdmap.top

[T31] Lua：Hello World
来源：http://jey.gogol.net.cn

print("Hello")
来源：http://qgw.yuxming.cn

[T32] Lua：局部变量
来源：http://dnb.zhoulong.xyz

local a = 1
来源：http://tmc.xylfe.cn

[T33] Lua：表（数组）
来源：http://tll.kuanghao11.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://keo.sweek.top

[T34] Lua：遍历表
来源：http://fwo.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://alt.jinqigfzy.top

[T35] Lua：字典表
来源：http://eld.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://upv.jiagoushi.top

[T36] Lua：函数
来源：http://pcj.xuanzx.com

function add(a, b) return a + b end
来源：http://zrw.ywan-chungtsiang.top

[T37] Lua：字符串拼接
来源：http://yjy.pycfn.com

"a" .. "b"
来源：http://ssu.zhijiandao.cn

[T38] Lua：条件
来源：http://iob.sweek.top

if x > 0 then print("正") end
来源：http://snt.havefunace.top

[T39] Lua：模式匹配
来源：http://avq.aizwys.cn

string.find(s, "%d+")
来源：http://wbo.tian-w.cn

[T40] Lua：元表
来源：http://zsn.wangdashe.top

setmetatable({}, { __index = base })
来源：http://wis.xziqi.cn

[T41] Perl：Hello World
来源：http://xii.jlsjyb.cn

print "Hello\n";
来源：http://wmb.dashuyun.cn

[T42] Perl：变量类型
来源：http://vfv.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yhm.bbcook.cn

[T43] Perl：字符串插值
来源：http://ygs.yj20258888.top

"值: $a"
来源：http://jam.hongshengwenyu.top

[T44] Perl：条件
来源：http://udh.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://hlj.xinyue.icu

[T45] Perl：数组遍历
来源：http://qwv.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://dpc.c1oappe.top

[T46] Perl：哈希操作
来源：http://iwe.quarkkingdee.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lfs.guannengcc.top

[T47] Perl：正则捕获
来源：http://ene.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lhv.smart0.xyz

[T48] Perl：正则替换
来源：http://lmg.hnqzz.top

$s =~ s/old/new/g;
来源：http://uzf.kuanghao11.cn

[T49] Perl：函数
来源：http://pjl.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://had.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://yyf.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lhs.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://kvl.sjlbkw.cn

[T51] Scala：Hello World
来源：http://dxa.sysykeji.top

println("Hello")
来源：http://gxx.chenlongwang.top

[T52] Scala：变量
来源：http://hpv.gotoacloud.top

val a = 1;  var b = 2
来源：http://wou.guannengcc.top

[T53] Scala：字符串插值
来源：http://qjg.yfazqb.com

s"值: $b"
来源：http://fuy.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://fqr.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://asg.sweek.top

[T55] Scala：集合过滤
来源：http://lnr.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://igb.xuetiantiany.cn

[T56] Scala：样例类
来源：http://zhg.jqgfzy.top

case class User(name: String, age: Int)
来源：http://tji.guowangkeji.top

[T57] Scala：模式匹配
来源：http://aom.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dou.hesvh.cn

[T58] Scala：函数定义
来源：http://kml.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iql.cashguo.top

[T59] Scala：循环
来源：http://hox.fktsv.cn

for (i <- 1 to 10) println(i)
来源：http://bde.epnwcf.com

[T60] Scala：折叠
来源：http://dcy.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://axn.sysykeji.top

================================================================================
来源：http://nzu.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dwg.zdqjudy.top

================================================================================
来源：http://szf.yvedp.cn

[U01] Py：创建虚拟环境
来源：http://ynj.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://wxr.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://pph.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bwb.guannengcc.top

[U03] Py：加载 .env 配置
来源：http://gdt.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ipt.cashguo.top

[U04] Py：变量调试打印
来源：http://gfv.feifeiyinyue.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://inp.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://rbn.hesvh.cn

list(dict.fromkeys(arr))
来源：http://jrt.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://iuv.zhaomingkeji.xyz

{**a, **b}
来源：http://mpv.hfpthk.cn

[U07] Py：反转字典键值
来源：http://mjf.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://klo.yonumen.top

[U08] Py：展平二维列表
来源：http://van.jianghu66.top

[y for x in nested for y in x]
来源：http://fvi.aizwys.cn

[U09] Py：字典取最大值的键
来源：http://fak.xuetiantiany.cn

max(d, key=d.get)
来源：http://wyw.tarul.cn

[U10] Py：按值排序字典
来源：http://aci.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://chv.dashuyun.cn

[U11] Py：生成器表达式
来源：http://dji.dashuyun.cn

(x * 2 for x in arr)
来源：http://opd.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://png.smart0.xyz

Counter(arr).most_common(3)
来源：http://orl.yonumen.top

[U13] Py：固定长度队列
来源：http://cuv.bjfxy.top

deque(maxlen=10)
来源：http://myw.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://dkk.tanke756.top

defaultdict(list)
来源：http://wdw.bjfxy.top

[U15] Py：高精度计时
来源：http://otk.epnwcf.com

t = time.perf_counter()
来源：http://csk.bjfxy.top

[U16] Py：命令行参数解析
来源：http://eqj.shanyushiyangtech.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uwd.hcnkem.com

[U17] Py：初始化日志
来源：http://ldh.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://ase.jinghuilouyu.cn

[U18] Py：预编译正则
来源：http://tgu.meibo888.top

pat = re.compile(r"\d+")
来源：http://zlz.xuetiantiany.cn

[U19] Py：正则替换带回调
来源：http://mpv.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://afg.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://xml.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://vuc.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://ynb.xinyue.icu

@contextlib.contextmanager
来源：http://jou.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://wkp.zdbjq.cn

list(zip(*m))
来源：http://rmn.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://hqc.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://euq.svipenyu.cn

[U24] Py：路径操作
来源：http://gze.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qnf.316326.xyz

[U25] Py：CSV 按字典读
来源：http://mke.guannengcc.top

csv.DictReader(f)
来源：http://hfg.sxryk.cn

[U26] Py：并发下载
来源：http://akl.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xbc.hnxiangtu.top

[U27] Py：异步 HTTP
来源：http://sdb.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ntp.ehwqpu.com

[U28] Py：类型别名
来源：http://fnz.gzhubu.top

UserId = int
来源：http://orq.havefunace.top

[U29] Py：属性校验
来源：http://bri.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://idi.daxiang520.top

[U30] Py：数据类
来源：http://mel.pengpengdd.cyou

@dataclass(slots=True)
来源：http://vgk.xuetiantiany.cn

[U31] Py：单测
来源：http://qra.nanxinkj.top

python -m pytest -q
来源：http://ghd.zdbjq.cn

[U32] Py：代码格式化
来源：http://lcc.sweek.top

ruff format . && ruff check --fix .
来源：http://vsn.kuanghao11.cn

[U33] Py：打包发布
来源：http://itq.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://bej.hnxiangtu.top

[U34] Py：判断编码
来源：http://wqx.birdmap.top

chardet.detect(raw)
来源：http://xow.epnwcf.com

[U35] Py：发送邮件
来源：http://xcf.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bhk.ivvv.top

[U36] Py：定时任务
来源：http://pga.zdqjudy.top

schedule.every(10).minutes.do(job)
来源：http://kwd.hfpthk.cn

[U37] Py：读写 Excel
来源：http://jar.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://zal.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://ukw.andypj.xyz

Path(__file__).resolve().parent
来源：http://zym.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://vzl.fktsv.cn

sys.stdout.isatty()
来源：http://nqb.smart0.xyz

[U40] Py：打印到标准错误
来源：http://xqf.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://mif.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://dqa.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wul.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://tvj.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sjg.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://uej.xylfe.cn

namespace App\Http;
来源：http://wlh.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://esa.uphjek.com

declare(strict_types=1);
来源：http://aom.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://cik.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uow.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://kra.shanyushiyangkeji.top

?string $name = null
来源：http://gcw.wangdashe.top

[U47] PHP：联合类型
来源：http://dqb.chenlongwang.top

int|string $id
来源：http://rso.jinqigufen.top

[U48] PHP：纯枚举
来源：http://xve.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blq.hywenlv.cn

[U49] PHP：只读属性
来源：http://ayf.epnwcf.com

public readonly string $name
来源：http://aoo.zhongyouzk.top

[U50] PHP：构造器属性提升
来源：http://yig.pycfn.com

public function __construct(private int $id) {}
来源：http://efj.yuxming.cn

[U51] PHP：数组解构
来源：http://nvr.bjfxy.top

[$a, $b] = $arr;
来源：http://hvg.chenlongwang.top

[U52] PHP：箭头函数
来源：http://slp.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://nzf.xziqi.cn

[U53] PHP：空合并运算符
来源：http://cnw.yuanzhike.top

$v = $a ?? $b ?? "default";
来源：http://loe.hammf.cn

[U54] PHP：空安全调用
来源：http://pss.feifeiyinyue.top

$obj?->method()
来源：http://img.ybcxt.top

[U55] PHP：match 表达式
来源：http://vui.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qxr.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://qlq.xziqi.cn

f(a: 1, b: 2)
来源：http://fzo.yuanzhike.top

[U57] PHP：字符串插值
来源：http://sda.svipenyu.cn

"值: {$a}"
来源：http://mzd.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://rgk.fzhhl.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mvn.mhx1999.top

[U59] PHP：自定义排序
来源：http://gzb.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jub.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://wdl.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ojd.guowangkeji.top


<!-- 参考信息 -->