代发 wailian999

[S39] C++：自定义比较器排序
来源：http://bie.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wit.yj20258.top

[S40] C++：查找元素
来源：http://wzn.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dem.meibo888.top

[S41] C++：类与构造函数
来源：http://nwn.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xai.epnwcf.com

[S42] C++：继承与虚函数
来源：http://cod.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://ayn.vehdjk.com

[S43] C++：智能指针
来源：http://rxn.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://eka.cdnleiting.top

[S44] C++：引用传参
来源：http://tlc.epnwcf.com

void inc(int &x) { ++x; }
来源：http://nze.yuanzhike.top

[S45] C++：lambda
来源：http://kiz.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://sxv.xziqi.cn

[S46] C++：函数模板
来源：http://fgt.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ahx.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://cgo.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bwt.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://atq.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://wyd.xziqi.cn

while (std::getline(in, line)) { }
来源：http://fyz.316326.xyz

[S49] C++：写文件
来源：http://cyv.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tdz.fzhhl.top

[S50] C++：格式化数字
来源：http://jmz.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zmv.zdbjq.cn

[S51] C++：显式类型转换
来源：http://goc.andypj.xyz

static_cast<double>(a) / b
来源：http://bst.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://gyv.xinyue.icu

int size() const noexcept { return n_; }
来源：http://noq.xinyue.icu

[S53] C++：移动语义
来源：http://wlu.hammf.cn

std::vector<int> w = std::move(v);
来源：http://vbi.yuanzhike.top

[S54] C++：异常处理
来源：http://wan.hywenlv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ypm.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://jiq.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gyf.guowangkeji.top

[S56] C++：optional
来源：http://wyu.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gwn.ydzc1.top

[S57] C++：编译期常量
来源：http://qku.sjlbkw.cn

constexpr int N = 10;
来源：http://cxp.yongpay.top

[S58] C++：命名空间
来源：http://aiu.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://oru.9152youxi.cn

[S59] C++：静态断言
来源：http://naa.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ibf.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://djv.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mrd.shanyushiyangkeji.top

================================================================================
来源：http://who.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gju.9152youxi.cn

================================================================================
来源：http://vrb.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://rue.cqqwz.cn

println("Hello")
来源：http://ppi.hammf.cn

[T02] Kotlin：变量
来源：http://vsz.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://svf.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://rxk.cqqwz.cn

"值: $b"
来源：http://qgk.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://glu.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://vaq.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://tcl.jinqigfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mcn.sysykeji.top

[T06] Kotlin：集合映射
来源：http://mhe.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dah.shuidangran.top

[T07] Kotlin：集合过滤
来源：http://zoh.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jij.yj20258888.top

[T08] Kotlin：数据类
来源：http://hup.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://qwc.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://kmx.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://fhr.yonumen.top

[T10] Kotlin：默认参数
来源：http://tgz.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ccm.hesvh.cn

[T11] Kotlin：协程
来源：http://zzn.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rxx.ydzc1.top

[T12] Kotlin：解构声明
来源：http://dwq.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://zsk.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://wau.zycfv.cn

val m = mapOf("a" to 1)
来源：http://nht.zdqjudy.top

[T14] Kotlin：循环
来源：http://ujb.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://gei.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://bue.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://qsa.zdbjq.cn

[T16] Swift：Hello World
来源：http://kvw.yongpay.top

print("Hello")
来源：http://ija.fktsv.cn

[T17] Swift：变量与常量
来源：http://cyr.svipenyu.cn

var a = 1;  let b = 2
来源：http://zag.hammf.cn

[T18] Swift：字符串插值
来源：http://fho.nanxinkj.top

"值: \(b)"
来源：http://vis.yangfankeji.com

[T19] Swift：可选绑定
来源：http://kgc.sufxvd.cn

if let n = opt { print(n) }
来源：http://ltr.yj20258888.top

[T20] Swift：数组操作
来源：http://ahh.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://mht.ppjwa.cn

[T21] Swift：遍历
来源：http://jee.shanyushiyangkeji.top

for x in a { print(x) }
来源：http://hvd.meibo888.top

[T22] Swift：字典
来源：http://jeq.hesvh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://imf.fanxiaobao.xyz

[T23] Swift：函数
来源：http://nlb.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gyv.ybcxt.top

[T24] Swift：闭包
来源：http://qwn.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qqi.hnqzz.top

[T25] Swift：结构体
来源：http://nfc.yonumen.top

struct P { var x: Int }
来源：http://ktd.yuanzhike.top

[T26] Swift：类与重写
来源：http://hfl.316326.xyz

class A: Base { override func f() {} }
来源：http://lbt.bjfxy.top

[T27] Swift：错误处理
来源：http://dgz.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://bvv.yanxiufei.cn

[T28] Swift：枚举
来源：http://qoo.zhoulong.xyz

enum Color { case red, green }
来源：http://uhe.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://daj.snrcjt.cn

guard let x = opt else { return }
来源：http://ggl.iojbl.cn

[T30] Swift：协议
来源：http://mlb.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://svq.andypj.xyz

[T31] Lua：Hello World
来源：http://prk.hcnkem.com

print("Hello")
来源：http://ivs.yj20258888.top

[T32] Lua：局部变量
来源：http://evx.bbcook.cn

local a = 1
来源：http://ulc.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://ygr.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://gbi.epnwcf.com

[T34] Lua：遍历表
来源：http://vkl.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jxq.9152youxi.cn

[T35] Lua：字典表
来源：http://sjp.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://xow.pengpengdd.cyou

[T36] Lua：函数
来源：http://lsa.52xcode.cn

function add(a, b) return a + b end
来源：http://swc.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://tfr.ywan-chungtsiang.top

"a" .. "b"
来源：http://aly.hysaishi.cn

[T38] Lua：条件
来源：http://lyk.fehbvm.com

if x > 0 then print("正") end
来源：http://izr.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://srv.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://bib.ehwqpu.com

[T40] Lua：元表
来源：http://cki.cucudq.cn

setmetatable({}, { __index = base })
来源：http://hhb.xylfe.cn

[T41] Perl：Hello World
来源：http://ewx.chenjidiqi.icu

print "Hello\n";
来源：http://mhi.chenlongwang.top

[T42] Perl：变量类型
来源：http://skb.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ynv.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://ngf.snrcjt.cn

"值: $a"
来源：http://atl.zhongyouzk.top

[T44] Perl：条件
来源：http://wpn.pycfn.com

if ($a > 0) { print "正"; }
来源：http://wxi.9152youxi.cn

[T45] Perl：数组遍历
来源：http://hvu.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://qcs.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://xnr.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yzx.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://zuo.9152youxi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qut.uphjek.com

[T48] Perl：正则替换
来源：http://qfu.sweek.top

$s =~ s/old/new/g;
来源：http://oin.zycfv.cn

[T49] Perl：函数
来源：http://qbt.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xua.chenzaomai.com

[T50] Perl：逐行读文件
来源：http://lpv.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://oqa.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://odc.gzhubu.top

[T51] Scala：Hello World
来源：http://ggr.yj202588.top

println("Hello")
来源：http://jiz.sweek.top

[T52] Scala：变量
来源：http://kty.c1oappe.top

val a = 1;  var b = 2
来源：http://gnk.yfazqb.com

[T53] Scala：字符串插值
来源：http://oyo.gotoacloud.top

s"值: $b"
来源：http://yei.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://xar.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://qnh.bbcook.cn

[T55] Scala：集合过滤
来源：http://veg.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://cey.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://azc.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://guy.c1oappe.top

[T57] Scala：模式匹配
来源：http://rpz.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jkc.fengsongda.top

[T58] Scala：函数定义
来源：http://wsf.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://zxr.cqqwz.cn

[T59] Scala：循环
来源：http://tzd.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://mev.9152youxi.cn

[T60] Scala：折叠
来源：http://qri.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mfd.smart0.xyz

================================================================================
来源：http://kbs.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kgo.vehdjk.com

================================================================================
来源：http://npx.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://gsm.zhoulong.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://pux.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://fdo.zycfv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iea.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://ydb.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sra.yongpay.top

[U04] Py：变量调试打印
来源：http://xpo.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ptx.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://knb.yvedp.cn

list(dict.fromkeys(arr))
来源：http://tdo.xuetiantiany.cn

[U06] Py：合并两个字典
来源：http://sug.ydzc1.top

{**a, **b}
来源：http://rpc.pengpengdd.cyou

[U07] Py：反转字典键值
来源：http://hdg.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://oww.fehbvm.com

[U08] Py：展平二维列表
来源：http://aig.mhx1999.top

[y for x in nested for y in x]
来源：http://dwj.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://eie.daxiang520.top

max(d, key=d.get)
来源：http://lba.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://dup.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eoo.nanxuanxn.top

[U11] Py：生成器表达式
来源：http://hbv.jqgfzy.top

(x * 2 for x in arr)
来源：http://bet.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://noz.gogol.net.cn

Counter(arr).most_common(3)
来源：http://iqg.yj20258888.top

[U13] Py：固定长度队列
来源：http://rok.xuanzx.com

deque(maxlen=10)
来源：http://obj.yfazqb.com

[U14] Py：分组收集到列表
来源：http://pof.sjlbkw.cn

defaultdict(list)
来源：http://iro.cdnleiting.top

[U15] Py：高精度计时
来源：http://mkm.xingfuxueyuan.xyz

t = time.perf_counter()
来源：http://sec.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://gym.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hcy.9152youxi.cn

[U17] Py：初始化日志
来源：http://dmp.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://rbz.redwolf501.top

[U18] Py：预编译正则
来源：http://qzm.havefunace.top

pat = re.compile(r"\d+")
来源：http://bad.bjfxy.top

[U19] Py：正则替换带回调
来源：http://twn.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wch.iojbl.cn

[U20] Py：缓存函数结果
来源：http://kwm.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://eos.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://iob.ivvv.top

@contextlib.contextmanager
来源：http://eji.birdmap.top

[U22] Py：矩阵转置
来源：http://uzp.zdqjudy.top

list(zip(*m))
来源：http://sfo.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://pkm.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xyw.hcnkem.com

[U24] Py：路径操作
来源：http://paq.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tla.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://wyf.wangdashe.top

csv.DictReader(f)
来源：http://myd.vqdsnc.cn

[U26] Py：并发下载
来源：http://sgm.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yki.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://ten.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://qpl.havefunace.top

[U28] Py：类型别名
来源：http://smz.shuidangran.top

UserId = int
来源：http://udw.epnwcf.com

[U29] Py：属性校验
来源：http://ehh.cqqwz.cn

@property 与 @x.setter 配合
来源：http://ehk.daria6918.cn

[U30] Py：数据类
来源：http://tjr.chenzaomai.com

@dataclass(slots=True)
来源：http://xvt.yonumen.top

[U31] Py：单测
来源：http://tjq.yj20258888.top

python -m pytest -q
来源：http://kdi.fktsv.cn

[U32] Py：代码格式化
来源：http://ezv.sysykeji.top

ruff format . && ruff check --fix .
来源：http://zvo.ivvv.top

[U33] Py：打包发布
来源：http://emb.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://qpn.jinqigufen.top

[U34] Py：判断编码
来源：http://pyu.ivvv.top

chardet.detect(raw)
来源：http://ezc.jqgfzy.top

[U35] Py：发送邮件
来源：http://xhm.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ubk.zhiwuduotai.top

[U36] Py：定时任务
来源：http://vmx.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://dih.yj20258888.top

[U37] Py：读写 Excel
来源：http://sds.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://bld.yj20258.top

[U38] Py：获取脚本所在目录
来源：http://bdz.fengsongda.top

Path(__file__).resolve().parent
来源：http://mnj.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://dtu.uphjek.com

sys.stdout.isatty()
来源：http://hbl.bjfxy.top

[U40] Py：打印到标准错误
来源：http://jwb.svipenyu.cn

print("err", file=sys.stderr)
来源：http://brc.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://xkp.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gkm.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://myh.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lqr.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://sad.0kj1m.cn

namespace App\Http;
来源：http://glv.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://qvx.sweek.top

declare(strict_types=1);
来源：http://leq.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://fde.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://awi.xinyue.icu

[U46] PHP：可空类型
来源：http://kmk.chenlongwang.top

?string $name = null
来源：http://mwb.zycfv.cn

[U47] PHP：联合类型
来源：http://qnz.yj202588.top

int|string $id
来源：http://yva.52xcode.cn

[U48] PHP：纯枚举
来源：http://gio.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qni.redwolf501.top

[U49] PHP：只读属性
来源：http://nry.gzhubu.top

public readonly string $name
来源：http://eed.epnwcf.com

[U50] PHP：构造器属性提升
来源：http://utd.xziqi.cn

public function __construct(private int $id) {}
来源：http://cbd.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://hse.ehwqpu.com

[$a, $b] = $arr;
来源：http://req.dianchejie.cn

[U52] PHP：箭头函数
来源：http://qwp.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://jer.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://udl.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://srq.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://ece.yueranfly.top

$obj?->method()
来源：http://ojo.sweek.top

[U55] PHP：match 表达式
来源：http://pqg.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://icv.cashguo.top

[U56] PHP：命名参数
来源：http://fic.yongpay.top

f(a: 1, b: 2)
来源：http://fcn.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://ssp.cheryme.top

"值: {$a}"
来源：http://gny.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://sfc.zhaomingkeji.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gri.fengsongda.top

[U59] PHP：自定义排序
来源：http://ybe.gzhubu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jie.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://xec.hesvh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kns.xuetiantiany.cn

[U61] PHP：正则
来源：http://lic.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mue.hysaishi.cn

[U62] PHP：日期对象
来源：http://ere.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fjv.havefunace.top

[U63] PHP：文件读写
来源：http://qow.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vqt.cucudq.cn

[U64] PHP：目录遍历
来源：http://niq.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://qgj.birdmap.top


<!-- 参考信息 -->