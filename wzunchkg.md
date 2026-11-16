代发 wailian999

[S37] C++：set
来源：http://txu.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rco.jqgfzy.top

[S38] C++：排序
来源：http://bvl.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://act.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://zxs.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yam.gaohongyu789.top

[S40] C++：查找元素
来源：http://owk.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qrn.hfpthk.cn

[S41] C++：类与构造函数
来源：http://npa.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mnu.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://ofp.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://vqf.sweek.top

[S43] C++：智能指针
来源：http://wrp.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://vnf.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://rlz.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://exs.ydjk.org.cn

[S45] C++：lambda
来源：http://azr.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://xxv.xuanzx.com

[S46] C++：函数模板
来源：http://fps.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hyx.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://rif.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xvz.xziqi.cn

[S48] C++：逐行读文件
来源：http://pul.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://dbm.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://gcj.gaohongyu789.top

[S49] C++：写文件
来源：http://cki.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ags.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://oqo.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eiz.xziqi.cn

[S51] C++：显式类型转换
来源：http://lae.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://mvw.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://uiz.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://oum.ctjpmb.com

[S53] C++：移动语义
来源：http://osp.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://gfh.nwbrower.top

[S54] C++：异常处理
来源：http://tkl.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://azw.yfazqb.com

[S55] C++：结构化绑定
来源：http://zis.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ajb.yangfankeji.com

[S56] C++：optional
来源：http://fcw.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lcg.vehdjk.com

[S57] C++：编译期常量
来源：http://ofs.yueranfly.top

constexpr int N = 10;
来源：http://rxz.chenzaomai.com

[S58] C++：命名空间
来源：http://ifb.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://xml.jiagoushi.top

[S59] C++：静态断言
来源：http://ntn.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ais.havefunace.top

[S60] C++：遍历并删除元素
来源：http://whn.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wrv.zycfv.cn

================================================================================
来源：http://tnj.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://orp.zdqjudy.top

================================================================================
来源：http://kso.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://tlz.yj202588.top

println("Hello")
来源：http://ztc.yonumen.top

[T02] Kotlin：变量
来源：http://lhg.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zmk.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://cod.tarul.cn

"值: $b"
来源：http://ofe.meibo888.top

[T04] Kotlin：空安全
来源：http://osk.guannengcc.top

val n: String? = null;  n?.length
来源：http://two.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://kuo.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tfv.316326.xyz

[T06] Kotlin：集合映射
来源：http://bpr.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qdf.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://fsi.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gol.ivvv.top

[T08] Kotlin：数据类
来源：http://shq.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://qye.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://fjh.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://mnx.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://pfl.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oez.ydzc1.top

[T11] Kotlin：协程
来源：http://gcu.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tua.redwolf501.top

[T12] Kotlin：解构声明
来源：http://ovk.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://noh.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://fvg.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://xnl.52xcode.cn

[T14] Kotlin：循环
来源：http://uyc.xuanzx.com

for (i in 1..10) println(i)
来源：http://eed.nwbrower.top

[T15] Kotlin：接口
来源：http://nxm.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://tma.cdnleiting.top

[T16] Swift：Hello World
来源：http://vqt.yanxiufei.cn

print("Hello")
来源：http://xqi.birdmap.top

[T17] Swift：变量与常量
来源：http://pqr.meibo888.top

var a = 1;  let b = 2
来源：http://fuu.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://nlm.52xcode.cn

"值: \(b)"
来源：http://oos.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://dts.jiagoushi.top

if let n = opt { print(n) }
来源：http://exb.gotoacloud.top

[T20] Swift：数组操作
来源：http://ysr.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://xet.jianghu66.top

[T21] Swift：遍历
来源：http://jmo.yonumen.top

for x in a { print(x) }
来源：http://bkt.yonumen.top

[T22] Swift：字典
来源：http://yju.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://tvy.iojbl.cn

[T23] Swift：函数
来源：http://gvx.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ftg.smart0.xyz

[T24] Swift：闭包
来源：http://rrc.jlsjyb.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cld.chenlongwang.top

[T25] Swift：结构体
来源：http://luc.gzhubu.top

struct P { var x: Int }
来源：http://eat.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://ztr.ivvv.top

class A: Base { override func f() {} }
来源：http://dzl.ivvv.top

[T27] Swift：错误处理
来源：http://geg.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://onr.hcnkem.com

[T28] Swift：枚举
来源：http://qtu.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://mfg.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://wdg.ivvv.top

guard let x = opt else { return }
来源：http://wpj.hnqzz.top

[T30] Swift：协议
来源：http://vqp.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://lvm.chenlongwang.top

[T31] Lua：Hello World
来源：http://yvm.cucudq.cn

print("Hello")
来源：http://lnc.hcnkem.com

[T32] Lua：局部变量
来源：http://mzv.iojbl.cn

local a = 1
来源：http://xfp.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://ica.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://raa.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://xpn.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hnh.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://emf.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://skn.gaohongyu789.top

[T36] Lua：函数
来源：http://vzy.c1oappe.top

function add(a, b) return a + b end
来源：http://ieh.andypj.xyz

[T37] Lua：字符串拼接
来源：http://yxi.fanxiaobao.xyz

"a" .. "b"
来源：http://aiu.birdmap.top

[T38] Lua：条件
来源：http://xvw.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://nni.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://qzv.c1oappe.top

string.find(s, "%d+")
来源：http://nmb.yj20258888.top

[T40] Lua：元表
来源：http://aqa.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://cql.yuanzhike.top

[T41] Perl：Hello World
来源：http://gtk.ywan-chungtsiang.top

print "Hello\n";
来源：http://hqu.andypj.xyz

[T42] Perl：变量类型
来源：http://qzp.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://egb.tanke756.top

[T43] Perl：字符串插值
来源：http://eib.bbcook.cn

"值: $a"
来源：http://uvc.sysykeji.top

[T44] Perl：条件
来源：http://dgp.nanxinkj.top

if ($a > 0) { print "正"; }
来源：http://nfu.ydzc1.top

[T45] Perl：数组遍历
来源：http://ght.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://tpj.wangdashe.top

[T46] Perl：哈希操作
来源：http://agn.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nvi.hysaishi.cn

[T47] Perl：正则捕获
来源：http://wlm.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ejd.zhoulong.xyz

[T48] Perl：正则替换
来源：http://dlg.uphjek.com

$s =~ s/old/new/g;
来源：http://oqo.cheryme.top

[T49] Perl：函数
来源：http://dea.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rma.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://fms.hfpthk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xnd.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://oyx.yanxiufei.cn

[T51] Scala：Hello World
来源：http://bha.havefunace.top

println("Hello")
来源：http://llp.jqgfzy.top

[T52] Scala：变量
来源：http://xgb.redwolf501.top

val a = 1;  var b = 2
来源：http://sqx.xziqi.cn

[T53] Scala：字符串插值
来源：http://vea.gogol.net.cn

s"值: $b"
来源：http://mob.guowangkeji.top

[T54] Scala：集合映射
来源：http://zel.hammf.cn

List(1, 2, 3).map(_ * 2)
来源：http://brn.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://zrp.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://rvl.yongpay.top

[T56] Scala：样例类
来源：http://cxu.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://kew.redwolf501.top

[T57] Scala：模式匹配
来源：http://dcs.0kj1m.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rna.yongpay.top

[T58] Scala：函数定义
来源：http://lnr.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bqu.xinyue.icu

[T59] Scala：循环
来源：http://wtz.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://tse.shuidangran.top

[T60] Scala：折叠
来源：http://lxb.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rss.hnqzz.top

================================================================================
来源：http://dmz.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gev.yongpay.top

================================================================================
来源：http://aqt.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://syt.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://axi.redwolf501.top

[U02] Py：导出 / 安装依赖
来源：http://utt.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fjo.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://peg.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xlh.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://uyw.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ind.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://sdt.chenlongwang.top

list(dict.fromkeys(arr))
来源：http://emf.cheryme.top

[U06] Py：合并两个字典
来源：http://xct.gogol.net.cn

{**a, **b}
来源：http://uin.epnwcf.com

[U07] Py：反转字典键值
来源：http://acy.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://bjw.wangdashe.top

[U08] Py：展平二维列表
来源：http://yoi.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://byb.nanxinkj.top

[U09] Py：字典取最大值的键
来源：http://ipn.zycfv.cn

max(d, key=d.get)
来源：http://arq.wangdashe.top

[U10] Py：按值排序字典
来源：http://ssl.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fsn.cashguo.top

[U11] Py：生成器表达式
来源：http://hlp.sweek.top

(x * 2 for x in arr)
来源：http://jgy.shzxlz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://olu.ehwqpu.com

Counter(arr).most_common(3)
来源：http://rny.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://uwn.zhengqikj.top

deque(maxlen=10)
来源：http://rix.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://nto.pycfn.com

defaultdict(list)
来源：http://xeh.yj20258.top

[U15] Py：高精度计时
来源：http://qmh.sysykeji.top

t = time.perf_counter()
来源：http://fao.yfazqb.com

[U16] Py：命令行参数解析
来源：http://fhs.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ldz.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://ciw.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://sdy.daria6918.cn

[U18] Py：预编译正则
来源：http://qvy.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://nek.hesvh.cn

[U19] Py：正则替换带回调
来源：http://zyo.pengpengdd.cyou

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://epw.yj20258888.top

[U20] Py：缓存函数结果
来源：http://jtt.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://dqa.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://smg.dashuyun.cn

@contextlib.contextmanager
来源：http://eqb.jianghu66.top

[U22] Py：矩阵转置
来源：http://cgl.fehbvm.com

list(zip(*m))
来源：http://seg.aizwys.cn

[U23] Py：分块读取大文件
来源：http://cae.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pgc.hcnkem.com

[U24] Py：路径操作
来源：http://ndd.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zla.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://cnx.316326.xyz

csv.DictReader(f)
来源：http://isv.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://ztp.cheryme.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rfg.tian-w.cn

[U27] Py：异步 HTTP
来源：http://sji.cheryme.top

aiohttp.ClientSession() 配合 async with
来源：http://wav.chenjidiqi.icu

[U28] Py：类型别名
来源：http://xds.wangshuangyany.cn

UserId = int
来源：http://ywy.hnxiangtu.top

[U29] Py：属性校验
来源：http://msg.nwbrower.top

@property 与 @x.setter 配合
来源：http://eri.shanyushiyangtech.top

[U30] Py：数据类
来源：http://ngq.ydjk.org.cn

@dataclass(slots=True)
来源：http://ibu.ctjpmb.com

[U31] Py：单测
来源：http://pjz.sjlbkw.cn

python -m pytest -q
来源：http://euz.jlsjyb.cn

[U32] Py：代码格式化
来源：http://uke.yongpay.top

ruff format . && ruff check --fix .
来源：http://ejb.zhengqikj.top

[U33] Py：打包发布
来源：http://bmy.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://kcj.bjfxy.top

[U34] Py：判断编码
来源：http://esn.vehdjk.com

chardet.detect(raw)
来源：http://kja.yonumen.top

[U35] Py：发送邮件
来源：http://uam.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zqx.gogol.net.cn

[U36] Py：定时任务
来源：http://hfk.tarul.cn

schedule.every(10).minutes.do(job)
来源：http://tja.c1oappe.top

[U37] Py：读写 Excel
来源：http://ucl.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nkh.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://mpx.fktsv.cn

Path(__file__).resolve().parent
来源：http://ncu.0kj1m.cn

[U39] Py：判断是否在交互环境
来源：http://cgz.gogol.net.cn

sys.stdout.isatty()
来源：http://grq.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://imc.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://zph.ehwqpu.com

[U41] PHP：初始化 Composer 项目
来源：http://vur.hcnkem.com

composer init;  composer require guzzlehttp/guzzle
来源：http://pok.uphjek.com

[U42] PHP：PSR-4 自动加载
来源：http://rwo.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qyl.xylfe.cn

[U43] PHP：声明命名空间
来源：http://cii.chenlongwang.top

namespace App\Http;
来源：http://beo.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://mrh.9152youxi.cn

declare(strict_types=1);
来源：http://mbu.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://jrq.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aoe.sysykeji.top

[U46] PHP：可空类型
来源：http://vke.xinyue.icu

?string $name = null
来源：http://klj.hesvh.cn

[U47] PHP：联合类型
来源：http://nkj.quarkkingdee.top

int|string $id
来源：http://hdt.zhixingplan.top

[U48] PHP：纯枚举
来源：http://zex.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pvq.vehdjk.com

[U49] PHP：只读属性
来源：http://ntk.jinqigufen.top

public readonly string $name
来源：http://ipb.cheryme.top

[U50] PHP：构造器属性提升
来源：http://rfd.guannengcc.top

public function __construct(private int $id) {}
来源：http://wls.jqgufenzy.top

[U51] PHP：数组解构
来源：http://hpz.sxryk.cn

[$a, $b] = $arr;
来源：http://eeb.sweek.top

[U52] PHP：箭头函数
来源：http://lgk.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://ugb.tarul.cn

[U53] PHP：空合并运算符
来源：http://xzo.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://tvi.ydjk.org.cn

[U54] PHP：空安全调用
来源：http://ljf.yj20258888.top

$obj?->method()
来源：http://dfi.dianchejie.cn

[U55] PHP：match 表达式
来源：http://iwy.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yvw.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://ijq.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://pfu.bbcook.cn

[U57] PHP：字符串插值
来源：http://daf.fzhhl.top

"值: {$a}"
来源：http://sdq.snrcjt.cn

[U58] PHP：数组三件套
来源：http://vao.ybcxt.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pye.yueranfly.top

[U59] PHP：自定义排序
来源：http://cre.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vns.shzxlz.cn

[U60] PHP：JSON 编解码
来源：http://ftb.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mco.shuidangran.top

[U61] PHP：正则
来源：http://guv.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xia.tian-w.cn

[U62] PHP：日期对象
来源：http://rrt.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mdd.hongshengwenyu.top


<!-- 参考信息 -->