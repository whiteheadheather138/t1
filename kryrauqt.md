代发 wailian999

[S37] C++：set
来源：http://oox.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kam.zhijiandao.cn

[S38] C++：排序
来源：http://ihj.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://lzy.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://zeq.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ubr.yj202588.top

[S40] C++：查找元素
来源：http://pfx.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dvv.cqqwz.cn

[S41] C++：类与构造函数
来源：http://mtu.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iot.ydzc1.top

[S42] C++：继承与虚函数
来源：http://spo.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://xtw.pengpengdd.cyou

[S43] C++：智能指针
来源：http://ebi.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://mxz.smart0.xyz

[S44] C++：引用传参
来源：http://dvn.yj20258.top

void inc(int &x) { ++x; }
来源：http://luw.zdbjq.cn

[S45] C++：lambda
来源：http://rfx.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://vel.yuxming.cn

[S46] C++：函数模板
来源：http://joz.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://djj.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://qzd.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://muf.gogol.net.cn

[S48] C++：逐行读文件
来源：http://kdq.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eip.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://jqc.yj20258.top

[S49] C++：写文件
来源：http://ely.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xig.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://laj.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qzg.tanke756.top

[S51] C++：显式类型转换
来源：http://erk.hcnkem.com

static_cast<double>(a) / b
来源：http://gyd.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://ies.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://khj.xinyue.icu

[S53] C++：移动语义
来源：http://pht.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://omp.kuanghao11.cn

[S54] C++：异常处理
来源：http://lhj.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gra.gotoacloud.top

[S55] C++：结构化绑定
来源：http://poo.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ttv.sysykeji.top

[S56] C++：optional
来源：http://vbo.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pdl.ctjpmb.com

[S57] C++：编译期常量
来源：http://gil.svipenyu.cn

constexpr int N = 10;
来源：http://osh.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://pbl.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://rqu.wangshuangyany.cn

[S59] C++：静态断言
来源：http://nsf.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ezn.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://zsq.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ytr.tianlin.xyz

================================================================================
来源：http://ybn.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pio.havefunace.top

================================================================================
来源：http://zdg.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://ais.hongshengwenyu.top

println("Hello")
来源：http://qfh.birdmap.top

[T02] Kotlin：变量
来源：http://hww.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qkk.yongpay.top

[T03] Kotlin：字符串模板
来源：http://bis.xuetiantiany.cn

"值: $b"
来源：http://weh.tianlin.xyz

[T04] Kotlin：空安全
来源：http://fix.zhaomingkeji.xyz

val n: String? = null;  n?.length
来源：http://uzr.xziqi.cn

[T05] Kotlin：when 表达式
来源：http://kyw.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ojf.xinyue.icu

[T06] Kotlin：集合映射
来源：http://xnd.ybcxt.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ctl.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://soy.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ucc.mhx1999.top

[T08] Kotlin：数据类
来源：http://ean.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://jep.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://zge.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://nsg.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://guj.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fyz.tianlin.xyz

[T11] Kotlin：协程
来源：http://vpa.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lwu.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://ceq.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://qnx.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://prc.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://ynk.mhx1999.top

[T14] Kotlin：循环
来源：http://npv.zycfv.cn

for (i in 1..10) println(i)
来源：http://jtg.xuanzx.com

[T15] Kotlin：接口
来源：http://yex.pycfn.com

interface Shape { fun area(): Double }
来源：http://zkm.dashuyun.cn

[T16] Swift：Hello World
来源：http://vtg.0kj1m.cn

print("Hello")
来源：http://hwl.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://xxy.fktsv.cn

var a = 1;  let b = 2
来源：http://jfo.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://cqz.cdnleiting.top

"值: \(b)"
来源：http://tgw.fktsv.cn

[T19] Swift：可选绑定
来源：http://ulb.pycfn.com

if let n = opt { print(n) }
来源：http://kfc.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://zqs.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wdd.jqgfzy.top

[T21] Swift：遍历
来源：http://gdb.snrcjt.cn

for x in a { print(x) }
来源：http://zdv.daxiang520.top

[T22] Swift：字典
来源：http://bic.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uwz.tanke756.top

[T23] Swift：函数
来源：http://xfj.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jiz.c1oappe.top

[T24] Swift：闭包
来源：http://lyz.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://inq.zhongyouzk.top

[T25] Swift：结构体
来源：http://rtt.yangfankeji.com

struct P { var x: Int }
来源：http://ebz.yj20258888.top

[T26] Swift：类与重写
来源：http://dgc.birdmap.top

class A: Base { override func f() {} }
来源：http://zko.hywenlv.cn

[T27] Swift：错误处理
来源：http://myw.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://bez.hywenlv.cn

[T28] Swift：枚举
来源：http://bcz.yuxming.cn

enum Color { case red, green }
来源：http://tkh.dashuyun.cn

[T29] Swift：guard 提前返回
来源：http://guf.xziqi.cn

guard let x = opt else { return }
来源：http://gui.yj20258.top

[T30] Swift：协议
来源：http://kfp.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://fzu.iojbl.cn

[T31] Lua：Hello World
来源：http://gis.wangshuangyany.cn

print("Hello")
来源：http://irc.yj20258.top

[T32] Lua：局部变量
来源：http://aow.dianchejie.cn

local a = 1
来源：http://drh.yj20258888.top

[T33] Lua：表（数组）
来源：http://xnj.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kgr.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://dvu.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uqq.uphjek.com

[T35] Lua：字典表
来源：http://xjs.xuanzx.com

local d = { a = 1 };  d.b = 2
来源：http://lvi.guowangkeji.top

[T36] Lua：函数
来源：http://lun.yvedp.cn

function add(a, b) return a + b end
来源：http://mqa.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://uyt.0kj1m.cn

"a" .. "b"
来源：http://xrj.xziqi.cn

[T38] Lua：条件
来源：http://qcc.yj202588.top

if x > 0 then print("正") end
来源：http://rfm.sufxvd.cn

[T39] Lua：模式匹配
来源：http://mtu.cashguo.top

string.find(s, "%d+")
来源：http://xev.sufxvd.cn

[T40] Lua：元表
来源：http://vsp.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://adj.hywenlv.cn

[T41] Perl：Hello World
来源：http://dgt.nanxinkj.top

print "Hello\n";
来源：http://cia.gaohongyu789.top

[T42] Perl：变量类型
来源：http://mvr.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gxg.sweek.top

[T43] Perl：字符串插值
来源：http://hew.ehwqpu.com

"值: $a"
来源：http://zfk.quarkkingdee.top

[T44] Perl：条件
来源：http://ycv.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://zww.nanxinkj.top

[T45] Perl：数组遍历
来源：http://ezu.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://gbz.iojbl.cn

[T46] Perl：哈希操作
来源：http://vdj.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jnt.yuanzhike.top

[T47] Perl：正则捕获
来源：http://akz.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hek.ydjk.org.cn

[T48] Perl：正则替换
来源：http://lre.redwolf501.top

$s =~ s/old/new/g;
来源：http://lhk.chenlongwang.top

[T49] Perl：函数
来源：http://cpl.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://joy.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://czc.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jfp.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://unx.fzhhl.top

[T51] Scala：Hello World
来源：http://agb.cashguo.top

println("Hello")
来源：http://toe.hcnkem.com

[T52] Scala：变量
来源：http://fxc.xziqi.cn

val a = 1;  var b = 2
来源：http://rqs.snrcjt.cn

[T53] Scala：字符串插值
来源：http://dti.sxryk.cn

s"值: $b"
来源：http://cod.jyoumei.cn

[T54] Scala：集合映射
来源：http://mob.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://clu.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://dig.aibaodan.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zpk.yj202588.top

[T56] Scala：样例类
来源：http://foa.aibaodan.cn

case class User(name: String, age: Int)
来源：http://wfu.chenlongwang.top

[T57] Scala：模式匹配
来源：http://xne.nanxuanxn.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://trt.fktsv.cn

[T58] Scala：函数定义
来源：http://vra.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://whi.yvedp.cn

[T59] Scala：循环
来源：http://jvx.snrcjt.cn

for (i <- 1 to 10) println(i)
来源：http://jym.uphjek.com

[T60] Scala：折叠
来源：http://lat.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tdr.hfpthk.cn

================================================================================
来源：http://edi.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ezt.ybcxt.top

================================================================================
来源：http://vpk.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://wur.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://emw.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://het.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jqh.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://xlk.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pyk.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://tps.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sky.sxryk.cn

[U05] Py：列表去重且保序
来源：http://txt.havefunace.top

list(dict.fromkeys(arr))
来源：http://hwr.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://rwy.316326.xyz

{**a, **b}
来源：http://omz.pycfn.com

[U07] Py：反转字典键值
来源：http://uar.wangdashe.top

{v: k for k, v in d.items()}
来源：http://rrx.aizwys.cn

[U08] Py：展平二维列表
来源：http://jgd.quarkkingdee.top

[y for x in nested for y in x]
来源：http://slb.xziqi.cn

[U09] Py：字典取最大值的键
来源：http://smf.zhongyouzk.top

max(d, key=d.get)
来源：http://kkn.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://iwi.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oxj.sweek.top

[U11] Py：生成器表达式
来源：http://tgq.cucudq.cn

(x * 2 for x in arr)
来源：http://grl.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://myw.ppjwa.cn

Counter(arr).most_common(3)
来源：http://dep.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://xcy.uphjek.com

deque(maxlen=10)
来源：http://jyf.ivvv.top

[U14] Py：分组收集到列表
来源：http://orz.pengpengdd.cyou

defaultdict(list)
来源：http://kau.xinyue.icu

[U15] Py：高精度计时
来源：http://arw.gzhubu.top

t = time.perf_counter()
来源：http://vlo.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://wfo.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://law.xinyue.icu

[U17] Py：初始化日志
来源：http://uhm.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://dfy.ppjwa.cn

[U18] Py：预编译正则
来源：http://rpr.yj202588.top

pat = re.compile(r"\d+")
来源：http://ncz.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://jda.shanyushiyangtech.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bnu.hesvh.cn

[U20] Py：缓存函数结果
来源：http://tpg.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://mjp.zhiwuduotai.top

[U21] Py：自定义上下文管理器
来源：http://zeb.cheryme.top

@contextlib.contextmanager
来源：http://gwr.snrcjt.cn

[U22] Py：矩阵转置
来源：http://wdw.0kj1m.cn

list(zip(*m))
来源：http://whn.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://mpv.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nzn.jqgufenzy.top

[U24] Py：路径操作
来源：http://hmd.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qwu.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://tzd.fzhhl.top

csv.DictReader(f)
来源：http://qzg.jyoumei.cn

[U26] Py：并发下载
来源：http://iux.xingfuxueyuan.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vbi.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://rga.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://pgx.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://kwx.gotoacloud.top

UserId = int
来源：http://svj.pycfn.com

[U29] Py：属性校验
来源：http://aqp.hfpthk.cn

@property 与 @x.setter 配合
来源：http://vze.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://oox.xingfuxueyuan.xyz

@dataclass(slots=True)
来源：http://dxg.ivvv.top

[U31] Py：单测
来源：http://nps.hnqzz.top

python -m pytest -q
来源：http://pbc.xylfe.cn

[U32] Py：代码格式化
来源：http://rnv.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://qly.yj202588.top

[U33] Py：打包发布
来源：http://asx.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://nrr.zycfv.cn

[U34] Py：判断编码
来源：http://zjl.jyoumei.cn

chardet.detect(raw)
来源：http://mpv.hcnkem.com

[U35] Py：发送邮件
来源：http://bmp.xuetiantiany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rtz.guowangkeji.top

[U36] Py：定时任务
来源：http://kpl.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://fdu.hcnkem.com

[U37] Py：读写 Excel
来源：http://ngn.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://dbm.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://rnf.birdmap.top

Path(__file__).resolve().parent
来源：http://xft.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://buy.fktsv.cn

sys.stdout.isatty()
来源：http://rrx.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://hqh.xinyue.icu

print("err", file=sys.stderr)
来源：http://sdi.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://odu.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jcm.fktsv.cn

[U42] PHP：PSR-4 自动加载
来源：http://epa.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://olj.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://fjn.gogol.net.cn

namespace App\Http;
来源：http://crt.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://fvk.fktsv.cn

declare(strict_types=1);
来源：http://plj.jinqigufen.top

[U45] PHP：类型声明与返回类型
来源：http://xav.shzxlz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ewn.yonumen.top

[U46] PHP：可空类型
来源：http://nlv.fehbvm.com

?string $name = null
来源：http://yhs.yongpay.top

[U47] PHP：联合类型
来源：http://cqu.chenzaomai.com

int|string $id
来源：http://lhb.cqqwz.cn

[U48] PHP：纯枚举
来源：http://zuo.cashguo.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aun.vehdjk.com

[U49] PHP：只读属性
来源：http://vaq.sxryk.cn

public readonly string $name
来源：http://dte.shanyushiyangtech.top

[U50] PHP：构造器属性提升
来源：http://tqj.wangdashe.top

public function __construct(private int $id) {}
来源：http://ort.jiagoushi.top

[U51] PHP：数组解构
来源：http://oee.svipenyu.cn

[$a, $b] = $arr;
来源：http://qqx.xziqi.cn

[U52] PHP：箭头函数
来源：http://cip.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://jsd.bbcook.cn

[U53] PHP：空合并运算符
来源：http://fwe.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://evg.fengsongda.top

[U54] PHP：空安全调用
来源：http://pco.yj20258.top

$obj?->method()
来源：http://gdh.yj20258888.top

[U55] PHP：match 表达式
来源：http://pep.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ibo.andypj.xyz

[U56] PHP：命名参数
来源：http://lmf.hywenlv.cn

f(a: 1, b: 2)
来源：http://tzi.yvedp.cn

[U57] PHP：字符串插值
来源：http://vpj.zhijiandao.cn

"值: {$a}"
来源：http://tyl.zhengqikj.top

[U58] PHP：数组三件套
来源：http://mvi.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hdq.vehdjk.com

[U59] PHP：自定义排序
来源：http://xfx.vqdsnc.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pxf.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://puc.jinyuanbaomall.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bho.bjfxy.top

[U61] PHP：正则
来源：http://ghf.fanxiaobao.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zvi.yfazqb.com

[U62] PHP：日期对象
来源：http://jjw.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jew.nwbrower.top


<!-- 参考信息 -->