代发 wailian999

[S35] C++：map
来源：http://sao.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hho.nanxinkj.top

[S36] C++：unordered_map
来源：http://ydh.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gwt.hfpthk.cn

[S37] C++：set
来源：http://pji.nanxinkj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ota.hysaishi.cn

[S38] C++：排序
来源：http://ykg.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://hmf.yonumen.top

[S39] C++：自定义比较器排序
来源：http://dyb.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://afc.pycfn.com

[S40] C++：查找元素
来源：http://ggi.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://owi.sysykeji.top

[S41] C++：类与构造函数
来源：http://nqs.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lwo.jianghu66.top

[S42] C++：继承与虚函数
来源：http://bim.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://oem.zdbjq.cn

[S43] C++：智能指针
来源：http://pul.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://gtw.hnxiangtu.top

[S44] C++：引用传参
来源：http://vcd.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://ssq.aibaodan.cn

[S45] C++：lambda
来源：http://iwk.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://kta.aibaodan.cn

[S46] C++：函数模板
来源：http://xze.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vea.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://gfa.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xpf.c1oappe.top

[S48] C++：逐行读文件
来源：http://rcg.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://uel.tian-w.cn

while (std::getline(in, line)) { }
来源：http://kbp.zhongyouzk.top

[S49] C++：写文件
来源：http://zcn.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zsk.sxryk.cn

[S50] C++：格式化数字
来源：http://guk.sxryk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nxl.iojbl.cn

[S51] C++：显式类型转换
来源：http://gvo.daria6918.cn

static_cast<double>(a) / b
来源：http://kyh.cheryme.top

[S52] C++：const 与 noexcept
来源：http://kzp.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://pyo.dashuyun.cn

[S53] C++：移动语义
来源：http://ucb.yongpay.top

std::vector<int> w = std::move(v);
来源：http://eam.hfpthk.cn

[S54] C++：异常处理
来源：http://duq.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pwu.xuanzx.com

[S55] C++：结构化绑定
来源：http://fnc.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gcu.yueranfly.top

[S56] C++：optional
来源：http://twr.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ixh.hnxiangtu.top

[S57] C++：编译期常量
来源：http://rce.52xcode.cn

constexpr int N = 10;
来源：http://bpf.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://wvv.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://rtf.vehdjk.com

[S59] C++：静态断言
来源：http://dhj.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rge.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://qnf.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tfc.jinqigufen.top

================================================================================
来源：http://cwc.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lhk.yuanzhike.top

================================================================================
来源：http://gku.xuanzx.com

[T01] Kotlin：Hello World
来源：http://exs.gaohongyu789.top

println("Hello")
来源：http://sej.ybcxt.top

[T02] Kotlin：变量
来源：http://knt.wangshuangyany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gds.shzxlz.cn

[T03] Kotlin：字符串模板
来源：http://waf.ywan-chungtsiang.top

"值: $b"
来源：http://ivo.fktsv.cn

[T04] Kotlin：空安全
来源：http://vkg.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://gbn.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://suq.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mwb.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://imq.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rvr.hammf.cn

[T07] Kotlin：集合过滤
来源：http://soq.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hlq.zdbjq.cn

[T08] Kotlin：数据类
来源：http://ezs.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://iha.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://rsg.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://rnn.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://llj.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://xhj.nanxinkj.top

[T11] Kotlin：协程
来源：http://nuy.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wsm.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://wok.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://bwi.tanke756.top

[T13] Kotlin：只读 Map
来源：http://age.tian-w.cn

val m = mapOf("a" to 1)
来源：http://wcl.meibo888.top

[T14] Kotlin：循环
来源：http://tor.aizwys.cn

for (i in 1..10) println(i)
来源：http://vpo.yj202588.top

[T15] Kotlin：接口
来源：http://dfc.yueranfly.top

interface Shape { fun area(): Double }
来源：http://yna.tianlin.xyz

[T16] Swift：Hello World
来源：http://eqm.zdqjudy.top

print("Hello")
来源：http://wsj.sxryk.cn

[T17] Swift：变量与常量
来源：http://awp.yfazqb.com

var a = 1;  let b = 2
来源：http://lnx.birdmap.top

[T18] Swift：字符串插值
来源：http://woo.jinyuanbaomall.cn

"值: \(b)"
来源：http://dul.sysykeji.top

[T19] Swift：可选绑定
来源：http://wye.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://aji.ctjpmb.com

[T20] Swift：数组操作
来源：http://xia.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mth.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://vjv.hywenlv.cn

for x in a { print(x) }
来源：http://huc.guowangkeji.top

[T22] Swift：字典
来源：http://rso.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zfi.jinghuilouyu.cn

[T23] Swift：函数
来源：http://vza.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://clp.52xcode.cn

[T24] Swift：闭包
来源：http://nsp.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wxo.hesvh.cn

[T25] Swift：结构体
来源：http://edq.mhx1999.top

struct P { var x: Int }
来源：http://lfl.hesvh.cn

[T26] Swift：类与重写
来源：http://ycj.yuxming.cn

class A: Base { override func f() {} }
来源：http://ssg.sufxvd.cn

[T27] Swift：错误处理
来源：http://icv.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://bdb.9152youxi.cn

[T28] Swift：枚举
来源：http://zzi.yanxiufei.cn

enum Color { case red, green }
来源：http://xnq.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://uws.ydjk.org.cn

guard let x = opt else { return }
来源：http://lvo.gogol.net.cn

[T30] Swift：协议
来源：http://wkp.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://kvq.jianghu66.top

[T31] Lua：Hello World
来源：http://cqp.chenjidiqi.icu

print("Hello")
来源：http://mvs.fktsv.cn

[T32] Lua：局部变量
来源：http://xxh.hfpthk.cn

local a = 1
来源：http://dyi.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://ffo.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ell.vehdjk.com

[T34] Lua：遍历表
来源：http://hta.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://swu.chenzaomai.com

[T35] Lua：字典表
来源：http://bsx.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://kiz.jyoumei.cn

[T36] Lua：函数
来源：http://pzw.hesvh.cn

function add(a, b) return a + b end
来源：http://fqm.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://csb.xylfe.cn

"a" .. "b"
来源：http://rqa.zhengqikj.top

[T38] Lua：条件
来源：http://eps.zdqjudy.top

if x > 0 then print("正") end
来源：http://gsm.hesvh.cn

[T39] Lua：模式匹配
来源：http://nvc.shangyingyoupin.top

string.find(s, "%d+")
来源：http://jbm.hongshengwenyu.top

[T40] Lua：元表
来源：http://edn.smart0.xyz

setmetatable({}, { __index = base })
来源：http://aod.zhengqikj.top

[T41] Perl：Hello World
来源：http://ybo.jyoumei.cn

print "Hello\n";
来源：http://dii.zdqjudy.top

[T42] Perl：变量类型
来源：http://frc.fktsv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dzu.gotoacloud.top

[T43] Perl：字符串插值
来源：http://zhw.pycfn.com

"值: $a"
来源：http://jco.gotoacloud.top

[T44] Perl：条件
来源：http://ouv.cheryme.top

if ($a > 0) { print "正"; }
来源：http://nip.zhengqikj.top

[T45] Perl：数组遍历
来源：http://ary.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://rez.52xcode.cn

[T46] Perl：哈希操作
来源：http://twq.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ymm.zycfv.cn

[T47] Perl：正则捕获
来源：http://fqv.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zdv.iojbl.cn

[T48] Perl：正则替换
来源：http://lgu.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://fmb.havefunace.top

[T49] Perl：函数
来源：http://hul.ydjk.org.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ixj.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://bzh.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mgw.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://rmt.hysaishi.cn

[T51] Scala：Hello World
来源：http://nph.xziqi.cn

println("Hello")
来源：http://ejv.wangshuangyany.cn

[T52] Scala：变量
来源：http://lta.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://lqg.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://qla.c1oappe.top

s"值: $b"
来源：http://rer.zhengqikj.top

[T54] Scala：集合映射
来源：http://bdw.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://nal.hywenlv.cn

[T55] Scala：集合过滤
来源：http://zzp.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://tty.cashguo.top

[T56] Scala：样例类
来源：http://ggi.redwolf501.top

case class User(name: String, age: Int)
来源：http://ivd.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://viq.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fsz.vehdjk.com

[T58] Scala：函数定义
来源：http://nml.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ceu.jianghu66.top

[T59] Scala：循环
来源：http://foi.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://wyo.jlsjyb.cn

[T60] Scala：折叠
来源：http://oxm.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uxy.zhaomingkeji.xyz

================================================================================
来源：http://psc.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ulv.fktsv.cn

================================================================================
来源：http://dxb.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://gux.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://rqv.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://ceq.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vgx.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://qjo.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://khe.aizwys.cn

[U04] Py：变量调试打印
来源：http://khy.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tkj.c1oappe.top

[U05] Py：列表去重且保序
来源：http://mia.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://lsv.52xcode.cn

[U06] Py：合并两个字典
来源：http://lzr.xziqi.cn

{**a, **b}
来源：http://hnx.haohaochexian.top

[U07] Py：反转字典键值
来源：http://kit.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://hbb.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://euv.sweek.top

[y for x in nested for y in x]
来源：http://dtj.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://alt.zhijiandao.cn

max(d, key=d.get)
来源：http://lfm.hnxiangtu.top

[U10] Py：按值排序字典
来源：http://jml.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tph.ehwqpu.com

[U11] Py：生成器表达式
来源：http://ddr.gotoacloud.top

(x * 2 for x in arr)
来源：http://hxt.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://tcs.0kj1m.cn

Counter(arr).most_common(3)
来源：http://ltk.nanxuanxn.top

[U13] Py：固定长度队列
来源：http://mvv.nanxinkj.top

deque(maxlen=10)
来源：http://rdf.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://vhc.sufxvd.cn

defaultdict(list)
来源：http://hxx.hnxiangtu.top

[U15] Py：高精度计时
来源：http://tuf.yonumen.top

t = time.perf_counter()
来源：http://rzr.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://nmh.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://izl.gotoacloud.top

[U17] Py：初始化日志
来源：http://abo.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://xeg.haohaochexian.top

[U18] Py：预编译正则
来源：http://hmj.xziqi.cn

pat = re.compile(r"\d+")
来源：http://zhd.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://tel.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sfd.vehdjk.com

[U20] Py：缓存函数结果
来源：http://fcf.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://lzi.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://ufr.hywenlv.cn

@contextlib.contextmanager
来源：http://oqh.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://yin.yfazqb.com

list(zip(*m))
来源：http://zuk.uphjek.com

[U23] Py：分块读取大文件
来源：http://uuw.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dlj.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://cpf.pengpengdd.cyou

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rge.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://wdb.fehbvm.com

csv.DictReader(f)
来源：http://xjs.cqqwz.cn

[U26] Py：并发下载
来源：http://xet.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kya.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://nyp.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://moy.chenzaomai.com

[U28] Py：类型别名
来源：http://lhm.chenlongwang.top

UserId = int
来源：http://zmd.cheryme.top

[U29] Py：属性校验
来源：http://caj.tian-w.cn

@property 与 @x.setter 配合
来源：http://bgs.jqgufenzy.top

[U30] Py：数据类
来源：http://jps.redwolf501.top

@dataclass(slots=True)
来源：http://det.mhx1999.top

[U31] Py：单测
来源：http://ntw.aizwys.cn

python -m pytest -q
来源：http://ust.hnqzz.top

[U32] Py：代码格式化
来源：http://hqv.hnqzz.top

ruff format . && ruff check --fix .
来源：http://ajm.9152youxi.cn

[U33] Py：打包发布
来源：http://cyk.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://cty.pengpengdd.cyou

[U34] Py：判断编码
来源：http://gos.wangshuangyany.cn

chardet.detect(raw)
来源：http://jty.sufxvd.cn

[U35] Py：发送邮件
来源：http://kjw.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kxi.guannengcc.top

[U36] Py：定时任务
来源：http://twh.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://jrj.cashguo.top

[U37] Py：读写 Excel
来源：http://okg.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bqg.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://gjc.aibaodan.cn

Path(__file__).resolve().parent
来源：http://jov.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://jti.gogol.net.cn

sys.stdout.isatty()
来源：http://lii.iojbl.cn

[U40] Py：打印到标准错误
来源：http://rxs.tarul.cn

print("err", file=sys.stderr)
来源：http://bbf.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://ntu.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://von.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://ppy.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lck.xuetiantiany.cn

[U43] PHP：声明命名空间
来源：http://okq.aibaodan.cn

namespace App\Http;
来源：http://dhc.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://wat.c1oappe.top

declare(strict_types=1);
来源：http://etj.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://rxm.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://prz.zhijiandao.cn

[U46] PHP：可空类型
来源：http://rxy.xuetiantiany.cn

?string $name = null
来源：http://pil.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://erb.zhiwuduotai.top

int|string $id
来源：http://zrl.zhixingplan.top

[U48] PHP：纯枚举
来源：http://rei.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zfx.yongpay.top

[U49] PHP：只读属性
来源：http://jwg.daria6918.cn

public readonly string $name
来源：http://qyx.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://cgw.yangfankeji.com

public function __construct(private int $id) {}
来源：http://bsq.9152youxi.cn

[U51] PHP：数组解构
来源：http://noo.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://oio.daxiang520.top

[U52] PHP：箭头函数
来源：http://gxs.ybcxt.top

$double = fn($x) => $x * 2;
来源：http://puk.ctjpmb.com

[U53] PHP：空合并运算符
来源：http://hpy.ywan-chungtsiang.top

$v = $a ?? $b ?? "default";
来源：http://tje.chenzaomai.com

[U54] PHP：空安全调用
来源：http://fcj.jinyuanbaomall.cn

$obj?->method()
来源：http://uhp.svipenyu.cn

[U55] PHP：match 表达式
来源：http://inm.daria6918.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jwp.9152youxi.cn

[U56] PHP：命名参数
来源：http://grl.ppjwa.cn

f(a: 1, b: 2)
来源：http://wxe.gotoacloud.top

[U57] PHP：字符串插值
来源：http://ctv.jinqigfzy.top

"值: {$a}"
来源：http://gvt.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://wqr.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://umn.iojbl.cn

[U59] PHP：自定义排序
来源：http://rqf.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pkt.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://oso.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xtg.aizwys.cn


<!-- 参考信息 -->