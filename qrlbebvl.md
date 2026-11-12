代发 wailian999

[S41] C++：类与构造函数
来源：http://toq.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pnl.yj20258888.top

[S42] C++：继承与虚函数
来源：http://jyp.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://min.cashguo.top

[S43] C++：智能指针
来源：http://blc.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://gju.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://buk.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://jzc.ywan-chungtsiang.top

[S45] C++：lambda
来源：http://yez.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://upq.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://ves.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ktw.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://bcv.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oss.gzhubu.top

[S48] C++：逐行读文件
来源：http://zch.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://xic.hcnkem.com

while (std::getline(in, line)) { }
来源：http://hgg.shangyingyoupin.top

[S49] C++：写文件
来源：http://lrm.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qrh.ydjk.org.cn

[S50] C++：格式化数字
来源：http://sxh.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://enz.ctjpmb.com

[S51] C++：显式类型转换
来源：http://prf.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://bpc.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://mbq.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://wpl.cucudq.cn

[S53] C++：移动语义
来源：http://esc.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://ipk.zhijiandao.cn

[S54] C++：异常处理
来源：http://kbj.yj20258888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://leu.smart0.xyz

[S55] C++：结构化绑定
来源：http://jte.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fwu.zhixingplan.top

[S56] C++：optional
来源：http://adp.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xpg.yuxming.cn

[S57] C++：编译期常量
来源：http://mgj.cashguo.top

constexpr int N = 10;
来源：http://ysd.jqgufenzy.top

[S58] C++：命名空间
来源：http://nuz.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://yud.hcnkem.com

[S59] C++：静态断言
来源：http://fev.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vik.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://hia.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hgf.tanke756.top

================================================================================
来源：http://dzi.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pfd.c1oappe.top

================================================================================
来源：http://rva.daria6918.cn

[T01] Kotlin：Hello World
来源：http://vuz.dashuyun.cn

println("Hello")
来源：http://npw.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://upc.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://def.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://mrm.wangshuangyany.cn

"值: $b"
来源：http://elk.tanke756.top

[T04] Kotlin：空安全
来源：http://jxs.guowangkeji.top

val n: String? = null;  n?.length
来源：http://ehu.birdmap.top

[T05] Kotlin：when 表达式
来源：http://hbt.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ptp.xziqi.cn

[T06] Kotlin：集合映射
来源：http://ifb.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pcr.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://yfn.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://glf.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://buw.meibo888.top

data class User(val name: String, val age: Int)
来源：http://teu.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://pzc.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://cwh.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://gyu.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://nqb.52xcode.cn

[T11] Kotlin：协程
来源：http://qbp.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hdn.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://hdp.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://qat.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://nkp.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://oqu.9152youxi.cn

[T14] Kotlin：循环
来源：http://vln.quarkkingdee.top

for (i in 1..10) println(i)
来源：http://kru.yonumen.top

[T15] Kotlin：接口
来源：http://ulr.jianghu66.top

interface Shape { fun area(): Double }
来源：http://jql.xuanzx.com

[T16] Swift：Hello World
来源：http://ndf.ywan-chungtsiang.top

print("Hello")
来源：http://ibk.daria6918.cn

[T17] Swift：变量与常量
来源：http://qby.uphjek.com

var a = 1;  let b = 2
来源：http://qba.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://qvp.xuetiantiany.cn

"值: \(b)"
来源：http://jir.cheryme.top

[T19] Swift：可选绑定
来源：http://flr.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://svh.cashguo.top

[T20] Swift：数组操作
来源：http://ndm.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kpm.daxiang520.top

[T21] Swift：遍历
来源：http://mjf.ydzc1.top

for x in a { print(x) }
来源：http://ebr.hongshengwenyu.top

[T22] Swift：字典
来源：http://qcs.yvedp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lkc.ctjpmb.com

[T23] Swift：函数
来源：http://drl.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zdu.xuanzx.com

[T24] Swift：闭包
来源：http://gar.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gds.316326.xyz

[T25] Swift：结构体
来源：http://vpt.zhiwuduotai.top

struct P { var x: Int }
来源：http://pyj.smart0.xyz

[T26] Swift：类与重写
来源：http://jil.52xcode.cn

class A: Base { override func f() {} }
来源：http://fun.hammf.cn

[T27] Swift：错误处理
来源：http://lvg.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://kpp.fktsv.cn

[T28] Swift：枚举
来源：http://okl.zdqjudy.top

enum Color { case red, green }
来源：http://thd.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://ncf.yonumen.top

guard let x = opt else { return }
来源：http://gom.cashguo.top

[T30] Swift：协议
来源：http://kiz.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://qqc.yvedp.cn

[T31] Lua：Hello World
来源：http://ymj.sysykeji.top

print("Hello")
来源：http://aic.shangyingyoupin.top

[T32] Lua：局部变量
来源：http://gvm.cashguo.top

local a = 1
来源：http://yhs.gzhubu.top

[T33] Lua：表（数组）
来源：http://ktz.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ilh.zdqjudy.top

[T34] Lua：遍历表
来源：http://vxd.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sgz.daxiang520.top

[T35] Lua：字典表
来源：http://edo.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://uri.birdmap.top

[T36] Lua：函数
来源：http://zkn.chenzaomai.com

function add(a, b) return a + b end
来源：http://rti.aizwys.cn

[T37] Lua：字符串拼接
来源：http://zyf.gotoacloud.top

"a" .. "b"
来源：http://irj.jinghuilouyu.cn

[T38] Lua：条件
来源：http://zha.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://flx.dashuyun.cn

[T39] Lua：模式匹配
来源：http://pqs.shangyingyoupin.top

string.find(s, "%d+")
来源：http://prd.hnqzz.top

[T40] Lua：元表
来源：http://oln.ybcxt.top

setmetatable({}, { __index = base })
来源：http://dmr.zhixingplan.top

[T41] Perl：Hello World
来源：http://ywt.tanke756.top

print "Hello\n";
来源：http://kvk.hnxiangtu.top

[T42] Perl：变量类型
来源：http://ukr.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://abd.jqgfzy.top

[T43] Perl：字符串插值
来源：http://iuz.guowangkeji.top

"值: $a"
来源：http://jvd.pengpengdd.cyou

[T44] Perl：条件
来源：http://bap.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://udl.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://fji.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://ihw.hammf.cn

[T46] Perl：哈希操作
来源：http://czh.zycfv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ogz.dashuyun.cn

[T47] Perl：正则捕获
来源：http://hbi.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://adc.xziqi.cn

[T48] Perl：正则替换
来源：http://kem.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://jhk.mhx1999.top

[T49] Perl：函数
来源：http://cnq.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://stg.c1oappe.top

[T50] Perl：逐行读文件
来源：http://lee.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fys.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://nzv.yj20258.top

[T51] Scala：Hello World
来源：http://sbx.chenjidiqi.icu

println("Hello")
来源：http://vtq.pengpengdd.cyou

[T52] Scala：变量
来源：http://nny.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://bjf.gotoacloud.top

[T53] Scala：字符串插值
来源：http://jeh.epnwcf.com

s"值: $b"
来源：http://jsm.hywenlv.cn

[T54] Scala：集合映射
来源：http://ssj.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://clq.dashuyun.cn

[T55] Scala：集合过滤
来源：http://dxb.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://oxv.nwbrower.top

[T56] Scala：样例类
来源：http://kzd.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://viy.cashguo.top

[T57] Scala：模式匹配
来源：http://jph.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pug.sufxvd.cn

[T58] Scala：函数定义
来源：http://eel.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://cbj.iojbl.cn

[T59] Scala：循环
来源：http://wfg.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://obt.ctjpmb.com

[T60] Scala：折叠
来源：http://qrc.hysaishi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vlt.epnwcf.com

================================================================================
来源：http://fky.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ftr.aizwys.cn

================================================================================
来源：http://pjj.ydzc1.top

[U01] Py：创建虚拟环境
来源：http://vyc.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dtq.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://ctz.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fio.uphjek.com

[U03] Py：加载 .env 配置
来源：http://cfb.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fjg.uphjek.com

[U04] Py：变量调试打印
来源：http://qkn.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ake.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://fkt.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://jke.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://jli.xinyue.icu

{**a, **b}
来源：http://mdq.yuxming.cn

[U07] Py：反转字典键值
来源：http://gys.vehdjk.com

{v: k for k, v in d.items()}
来源：http://asz.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://kit.guannengcc.top

[y for x in nested for y in x]
来源：http://swo.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://zin.tian-w.cn

max(d, key=d.get)
来源：http://fws.pycfn.com

[U10] Py：按值排序字典
来源：http://zfv.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bed.xingfuxueyuan.xyz

[U11] Py：生成器表达式
来源：http://ohv.yuxming.cn

(x * 2 for x in arr)
来源：http://qze.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://jks.jiagoushi.top

Counter(arr).most_common(3)
来源：http://yqv.yonumen.top

[U13] Py：固定长度队列
来源：http://jnz.iojbl.cn

deque(maxlen=10)
来源：http://icu.cucudq.cn

[U14] Py：分组收集到列表
来源：http://lsd.xuetiantiany.cn

defaultdict(list)
来源：http://mkf.fengsongda.top

[U15] Py：高精度计时
来源：http://irz.mhx1999.top

t = time.perf_counter()
来源：http://ruq.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://cwo.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zaw.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://trz.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://xze.jinqigfzy.top

[U18] Py：预编译正则
来源：http://lae.52xcode.cn

pat = re.compile(r"\d+")
来源：http://ccc.snrcjt.cn

[U19] Py：正则替换带回调
来源：http://zco.shuidangran.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vkc.bjfxy.top

[U20] Py：缓存函数结果
来源：http://vkz.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://sfx.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://ymu.cqqwz.cn

@contextlib.contextmanager
来源：http://qbq.ybcxt.top

[U22] Py：矩阵转置
来源：http://kwv.hnqzz.top

list(zip(*m))
来源：http://wql.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://wkk.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dki.uphjek.com

[U24] Py：路径操作
来源：http://lij.yueranfly.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pfg.9152youxi.cn

[U25] Py：CSV 按字典读
来源：http://ocg.pycfn.com

csv.DictReader(f)
来源：http://jup.havefunace.top

[U26] Py：并发下载
来源：http://clg.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rzn.tarul.cn

[U27] Py：异步 HTTP
来源：http://qsy.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://ljd.nwbrower.top

[U28] Py：类型别名
来源：http://mbl.dianchejie.cn

UserId = int
来源：http://oku.hcnkem.com

[U29] Py：属性校验
来源：http://vrq.jianghu66.top

@property 与 @x.setter 配合
来源：http://btw.yj20258888.top

[U30] Py：数据类
来源：http://hlk.andypj.xyz

@dataclass(slots=True)
来源：http://fik.jqgufenzy.top

[U31] Py：单测
来源：http://ggb.xingfuxueyuan.xyz

python -m pytest -q
来源：http://wwb.hysaishi.cn

[U32] Py：代码格式化
来源：http://acy.shuidangran.top

ruff format . && ruff check --fix .
来源：http://frc.guannengcc.top

[U33] Py：打包发布
来源：http://smr.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://cji.zhoulong.xyz

[U34] Py：判断编码
来源：http://hrz.yonumen.top

chardet.detect(raw)
来源：http://tug.vehdjk.com

[U35] Py：发送邮件
来源：http://rot.fzhhl.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ibq.quarkkingdee.top

[U36] Py：定时任务
来源：http://qrn.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://zmv.aizwys.cn

[U37] Py：读写 Excel
来源：http://xvu.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://res.aibaodan.cn

[U38] Py：获取脚本所在目录
来源：http://dyi.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://bly.sufxvd.cn

[U39] Py：判断是否在交互环境
来源：http://pao.tarul.cn

sys.stdout.isatty()
来源：http://zsh.fehbvm.com

[U40] Py：打印到标准错误
来源：http://jbn.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://blw.ydjk.org.cn

[U41] PHP：初始化 Composer 项目
来源：http://yyj.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pzx.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://xqg.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uwg.hcnkem.com

[U43] PHP：声明命名空间
来源：http://ffq.tian-w.cn

namespace App\Http;
来源：http://cic.jqgufenzy.top

[U44] PHP：开启严格类型
来源：http://ljw.jiagoushi.top

declare(strict_types=1);
来源：http://iqx.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://odp.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vrv.uphjek.com

[U46] PHP：可空类型
来源：http://fzx.hywenlv.cn

?string $name = null
来源：http://rtw.jlsjyb.cn

[U47] PHP：联合类型
来源：http://kmm.daxiang520.top

int|string $id
来源：http://otu.fanxiaobao.xyz

[U48] PHP：纯枚举
来源：http://jds.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cqj.hnqzz.top

[U49] PHP：只读属性
来源：http://nik.sxryk.cn

public readonly string $name
来源：http://dsh.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://ybd.ywan-chungtsiang.top

public function __construct(private int $id) {}
来源：http://tpl.shanyushiyangtech.top

[U51] PHP：数组解构
来源：http://agh.52xcode.cn

[$a, $b] = $arr;
来源：http://rii.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://thj.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://qne.gogol.net.cn

[U53] PHP：空合并运算符
来源：http://ikp.hfpthk.cn

$v = $a ?? $b ?? "default";
来源：http://srl.zycfv.cn

[U54] PHP：空安全调用
来源：http://ciy.jiagoushi.top

$obj?->method()
来源：http://fxw.tian-w.cn

[U55] PHP：match 表达式
来源：http://dkh.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://skw.bbcook.cn

[U56] PHP：命名参数
来源：http://qul.hysaishi.cn

f(a: 1, b: 2)
来源：http://mej.daria6918.cn

[U57] PHP：字符串插值
来源：http://nva.ppjwa.cn

"值: {$a}"
来源：http://wqg.yuanzhike.top

[U58] PHP：数组三件套
来源：http://dsn.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yym.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://kwr.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://thn.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://qws.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iuu.bjfxy.top

[U61] PHP：正则
来源：http://ncr.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hwz.svipenyu.cn

[U62] PHP：日期对象
来源：http://rdd.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fic.sjlbkw.cn

[U63] PHP：文件读写
来源：http://gpq.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://roj.wangdashe.top

[U64] PHP：目录遍历
来源：http://ryu.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://uhy.hfpthk.cn

[U65] PHP：会话
来源：http://hxm.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://agr.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://xnh.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rrh.hcnkem.com


<!-- 参考信息 -->