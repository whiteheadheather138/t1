代发 wailian999

[S35] C++：map
来源：http://qtj.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oiz.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://gws.birdmap.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dup.ydzc1.top

[S37] C++：set
来源：http://acc.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rwb.hnxiangtu.top

[S38] C++：排序
来源：http://wwf.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://ssf.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://shl.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mdk.tianlin.xyz

[S40] C++：查找元素
来源：http://yly.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://off.yangfankeji.com

[S41] C++：类与构造函数
来源：http://xzn.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lkn.fzhhl.top

[S42] C++：继承与虚函数
来源：http://gbo.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://mdi.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://lnl.ppjwa.cn

auto p = std::make_unique<int>(5);
来源：http://hlh.cashguo.top

[S44] C++：引用传参
来源：http://ydk.uphjek.com

void inc(int &x) { ++x; }
来源：http://gyj.mhx1999.top

[S45] C++：lambda
来源：http://pdb.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://qby.yonumen.top

[S46] C++：函数模板
来源：http://xuz.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://boc.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://ijb.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dnc.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://ipf.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://evx.sysykeji.top

while (std::getline(in, line)) { }
来源：http://oie.xuanzx.com

[S49] C++：写文件
来源：http://mmj.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iku.hfpthk.cn

[S50] C++：格式化数字
来源：http://oae.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eon.dashuyun.cn

[S51] C++：显式类型转换
来源：http://izt.ydzc1.top

static_cast<double>(a) / b
来源：http://dzp.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://lzu.hesvh.cn

int size() const noexcept { return n_; }
来源：http://xjj.hesvh.cn

[S53] C++：移动语义
来源：http://avw.tanke756.top

std::vector<int> w = std::move(v);
来源：http://nsh.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://jyc.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://psk.sysykeji.top

[S55] C++：结构化绑定
来源：http://nxu.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jez.pycfn.com

[S56] C++：optional
来源：http://slb.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qmi.yuxming.cn

[S57] C++：编译期常量
来源：http://olj.dashuyun.cn

constexpr int N = 10;
来源：http://vsk.snrcjt.cn

[S58] C++：命名空间
来源：http://zid.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://wwn.quarkkingdee.top

[S59] C++：静态断言
来源：http://ujq.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iat.uphjek.com

[S60] C++：遍历并删除元素
来源：http://agi.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ocj.wangshuangyany.cn

================================================================================
来源：http://jay.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ajr.yfazqb.com

================================================================================
来源：http://ebv.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://uhj.jinqigufen.top

println("Hello")
来源：http://ted.yj20258.top

[T02] Kotlin：变量
来源：http://wkg.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ntm.cashguo.top

[T03] Kotlin：字符串模板
来源：http://dbn.yanxiufei.cn

"值: $b"
来源：http://pxx.xinyue.icu

[T04] Kotlin：空安全
来源：http://sur.yj20258888.top

val n: String? = null;  n?.length
来源：http://ygz.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://wwn.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xih.yj202588.top

[T06] Kotlin：集合映射
来源：http://veb.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hlx.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://mss.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://vyb.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://auy.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://rks.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://iqn.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://zad.redwolf501.top

[T10] Kotlin：默认参数
来源：http://vmz.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://olu.zhijiandao.cn

[T11] Kotlin：协程
来源：http://ler.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://fxx.mhx1999.top

[T12] Kotlin：解构声明
来源：http://ick.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://hps.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://vsp.yj20258.top

val m = mapOf("a" to 1)
来源：http://jwf.hysaishi.cn

[T14] Kotlin：循环
来源：http://jxd.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://cgk.jinqigfzy.top

[T15] Kotlin：接口
来源：http://ovp.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://jmr.316326.xyz

[T16] Swift：Hello World
来源：http://pkh.zhoulong.xyz

print("Hello")
来源：http://fbi.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://rmc.cheryme.top

var a = 1;  let b = 2
来源：http://pns.meibo888.top

[T18] Swift：字符串插值
来源：http://mdu.zhaomingkeji.xyz

"值: \(b)"
来源：http://yhk.daria6918.cn

[T19] Swift：可选绑定
来源：http://rpa.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://ypn.ydzc1.top

[T20] Swift：数组操作
来源：http://lmc.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://eyt.ppjwa.cn

[T21] Swift：遍历
来源：http://jac.zhongyouzk.top

for x in a { print(x) }
来源：http://fxt.fengsongda.top

[T22] Swift：字典
来源：http://icp.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://axp.cdnleiting.top

[T23] Swift：函数
来源：http://egc.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cdd.sweek.top

[T24] Swift：闭包
来源：http://ubp.yanxiufei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://swg.hysaishi.cn

[T25] Swift：结构体
来源：http://fvq.0kj1m.cn

struct P { var x: Int }
来源：http://aig.hammf.cn

[T26] Swift：类与重写
来源：http://nne.dashuyun.cn

class A: Base { override func f() {} }
来源：http://mfu.yonumen.top

[T27] Swift：错误处理
来源：http://goc.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://eli.52xcode.cn

[T28] Swift：枚举
来源：http://xzd.zdqjudy.top

enum Color { case red, green }
来源：http://dle.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://ivq.dashuyun.cn

guard let x = opt else { return }
来源：http://ydt.zhoulong.xyz

[T30] Swift：协议
来源：http://wil.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://dqd.ivvv.top

[T31] Lua：Hello World
来源：http://raj.shangyingyoupin.top

print("Hello")
来源：http://qzi.mhx1999.top

[T32] Lua：局部变量
来源：http://sik.jinyuanbaomall.cn

local a = 1
来源：http://rif.smart0.xyz

[T33] Lua：表（数组）
来源：http://mih.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hww.ppjwa.cn

[T34] Lua：遍历表
来源：http://zvq.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://luo.ehwqpu.com

[T35] Lua：字典表
来源：http://gbi.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://tgk.andypj.xyz

[T36] Lua：函数
来源：http://zhq.sysykeji.top

function add(a, b) return a + b end
来源：http://zih.xylfe.cn

[T37] Lua：字符串拼接
来源：http://llv.shanyushiyangtech.top

"a" .. "b"
来源：http://ybh.zdqjudy.top

[T38] Lua：条件
来源：http://moj.sjlbkw.cn

if x > 0 then print("正") end
来源：http://hch.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://yyr.jinqigufen.top

string.find(s, "%d+")
来源：http://hqg.hnqzz.top

[T40] Lua：元表
来源：http://kcm.xuetiantiany.cn

setmetatable({}, { __index = base })
来源：http://koc.aibaodan.cn

[T41] Perl：Hello World
来源：http://qlk.tanke756.top

print "Hello\n";
来源：http://rli.gzhubu.top

[T42] Perl：变量类型
来源：http://arw.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://juf.yuanzhike.top

[T43] Perl：字符串插值
来源：http://cvr.jinqigfzy.top

"值: $a"
来源：http://iwk.jianghu66.top

[T44] Perl：条件
来源：http://ggw.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://gzs.gzhubu.top

[T45] Perl：数组遍历
来源：http://wjh.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://ajm.hnxiangtu.top

[T46] Perl：哈希操作
来源：http://hmi.hongshengwenyu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ojs.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://phn.uphjek.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://uqr.xinyue.icu

[T48] Perl：正则替换
来源：http://lfj.nanxinkj.top

$s =~ s/old/new/g;
来源：http://zuf.birdmap.top

[T49] Perl：函数
来源：http://nuj.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sbr.yj20258888.top

[T50] Perl：逐行读文件
来源：http://icw.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yqr.sweek.top

while (my $line = <$fh>) { print $line; }
来源：http://npw.chenzaomai.com

[T51] Scala：Hello World
来源：http://vtv.epnwcf.com

println("Hello")
来源：http://vhb.wangshuangyany.cn

[T52] Scala：变量
来源：http://nel.ydjk.org.cn

val a = 1;  var b = 2
来源：http://uzd.fengsongda.top

[T53] Scala：字符串插值
来源：http://cic.sxryk.cn

s"值: $b"
来源：http://ohq.ivvv.top

[T54] Scala：集合映射
来源：http://xeq.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://chg.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://cyc.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://tgu.guowangkeji.top

[T56] Scala：样例类
来源：http://kyj.fzhhl.top

case class User(name: String, age: Int)
来源：http://kkr.fktsv.cn

[T57] Scala：模式匹配
来源：http://zvt.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xtg.xylfe.cn

[T58] Scala：函数定义
来源：http://qqf.xingfuxueyuan.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://tqv.gaohongyu789.top

[T59] Scala：循环
来源：http://jfo.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://svs.yangfankeji.com

[T60] Scala：折叠
来源：http://wal.zdbjq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qhp.cashguo.top

================================================================================
来源：http://exf.xziqi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uui.snrcjt.cn

================================================================================
来源：http://kpk.wangshuangyany.cn

[U01] Py：创建虚拟环境
来源：http://kyn.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yly.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://ooa.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zmv.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://mix.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tfm.xylfe.cn

[U04] Py：变量调试打印
来源：http://awm.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nix.chenzaomai.com

[U05] Py：列表去重且保序
来源：http://jpa.xziqi.cn

list(dict.fromkeys(arr))
来源：http://fzs.yj202588.top

[U06] Py：合并两个字典
来源：http://mms.zhengqikj.top

{**a, **b}
来源：http://lfv.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://gsg.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://pcl.hammf.cn

[U08] Py：展平二维列表
来源：http://otq.52xcode.cn

[y for x in nested for y in x]
来源：http://qgf.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://bfc.c1oappe.top

max(d, key=d.get)
来源：http://tvm.havefunace.top

[U10] Py：按值排序字典
来源：http://pms.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://twg.fanxiaobao.xyz

[U11] Py：生成器表达式
来源：http://bsf.aizwys.cn

(x * 2 for x in arr)
来源：http://jym.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sxd.chenlongwang.top

Counter(arr).most_common(3)
来源：http://rsj.cqqwz.cn

[U13] Py：固定长度队列
来源：http://zqd.shzxlz.cn

deque(maxlen=10)
来源：http://oee.jianghu66.top

[U14] Py：分组收集到列表
来源：http://nyj.ivvv.top

defaultdict(list)
来源：http://pth.nwbrower.top

[U15] Py：高精度计时
来源：http://qwl.havefunace.top

t = time.perf_counter()
来源：http://ayd.xylfe.cn

[U16] Py：命令行参数解析
来源：http://zig.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://szv.yj202588.top

[U17] Py：初始化日志
来源：http://kjj.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://cdg.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://die.xinyue.icu

pat = re.compile(r"\d+")
来源：http://zws.hnqzz.top

[U19] Py：正则替换带回调
来源：http://egg.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tax.ydzc1.top

[U20] Py：缓存函数结果
来源：http://thr.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://nqi.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://sae.quarkkingdee.top

@contextlib.contextmanager
来源：http://jvd.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://lah.xylfe.cn

list(zip(*m))
来源：http://lxw.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://tjm.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vgo.andypj.xyz

[U24] Py：路径操作
来源：http://qep.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xtz.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://vqy.guowangkeji.top

csv.DictReader(f)
来源：http://mqw.shangyingyoupin.top

[U26] Py：并发下载
来源：http://cvo.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lik.shuidangran.top

[U27] Py：异步 HTTP
来源：http://mmb.quarkkingdee.top

aiohttp.ClientSession() 配合 async with
来源：http://gmq.yongpay.top

[U28] Py：类型别名
来源：http://oaa.dianchejie.cn

UserId = int
来源：http://ikc.xylfe.cn

[U29] Py：属性校验
来源：http://ffb.xziqi.cn

@property 与 @x.setter 配合
来源：http://cvd.guowangkeji.top

[U30] Py：数据类
来源：http://hdy.shzxlz.cn

@dataclass(slots=True)
来源：http://abn.yueranfly.top

[U31] Py：单测
来源：http://biq.fanxiaobao.xyz

python -m pytest -q
来源：http://ehj.epnwcf.com

[U32] Py：代码格式化
来源：http://lhp.tanke756.top

ruff format . && ruff check --fix .
来源：http://mat.yonumen.top

[U33] Py：打包发布
来源：http://ejd.aibaodan.cn

python -m build  （依赖 pyproject.toml）
来源：http://jex.dianchejie.cn

[U34] Py：判断编码
来源：http://hiv.hesvh.cn

chardet.detect(raw)
来源：http://pfg.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://quz.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uin.zhaomingkeji.xyz

[U36] Py：定时任务
来源：http://wir.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://upm.yvedp.cn

[U37] Py：读写 Excel
来源：http://lmh.52xcode.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cdp.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://sle.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://sln.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://tfg.sjlbkw.cn

sys.stdout.isatty()
来源：http://yph.smart0.xyz

[U40] Py：打印到标准错误
来源：http://zoh.smart0.xyz

print("err", file=sys.stderr)
来源：http://nul.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://tzn.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qny.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://dzg.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rmh.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://rsl.jiagoushi.top

namespace App\Http;
来源：http://gqf.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://iig.snrcjt.cn

declare(strict_types=1);
来源：http://flb.yonumen.top

[U45] PHP：类型声明与返回类型
来源：http://gxq.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xks.52xcode.cn

[U46] PHP：可空类型
来源：http://uvl.birdmap.top

?string $name = null
来源：http://hcn.jqgfzy.top

[U47] PHP：联合类型
来源：http://qhh.tianlin.xyz

int|string $id
来源：http://zax.chenzaomai.com

[U48] PHP：纯枚举
来源：http://qny.cucudq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xth.yanxiufei.cn

[U49] PHP：只读属性
来源：http://wle.cucudq.cn

public readonly string $name
来源：http://vgt.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://zzs.jyoumei.cn

public function __construct(private int $id) {}
来源：http://qph.yvedp.cn

[U51] PHP：数组解构
来源：http://okq.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://ern.9152youxi.cn

[U52] PHP：箭头函数
来源：http://jqq.sweek.top

$double = fn($x) => $x * 2;
来源：http://gxt.daria6918.cn

[U53] PHP：空合并运算符
来源：http://ugp.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://nic.quarkkingdee.top

[U54] PHP：空安全调用
来源：http://pmq.chenzaomai.com

$obj?->method()
来源：http://jjg.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://bbp.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vrv.ivvv.top

[U56] PHP：命名参数
来源：http://vxl.svipenyu.cn

f(a: 1, b: 2)
来源：http://nqx.daxiang520.top

[U57] PHP：字符串插值
来源：http://ige.sjlbkw.cn

"值: {$a}"
来源：http://jfh.sxryk.cn

[U58] PHP：数组三件套
来源：http://tkt.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nam.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://zer.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bll.shzxlz.cn

[U60] PHP：JSON 编解码
来源：http://cim.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xpz.guannengcc.top


<!-- 参考信息 -->