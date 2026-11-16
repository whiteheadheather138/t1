代发 wailian999

[S41] C++：类与构造函数
来源：http://yit.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dpc.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://ajv.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://fwl.hnqzz.top

[S43] C++：智能指针
来源：http://rdk.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://hhu.chenlongwang.top

[S44] C++：引用传参
来源：http://fxn.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://ocl.cucudq.cn

[S45] C++：lambda
来源：http://rxl.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ubc.zhiwuduotai.top

[S46] C++：函数模板
来源：http://mxy.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nql.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://egc.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qdb.guannengcc.top

[S48] C++：逐行读文件
来源：http://jis.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://xth.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://epc.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://zpc.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mje.guannengcc.top

[S50] C++：格式化数字
来源：http://qfc.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kdr.tian-w.cn

[S51] C++：显式类型转换
来源：http://xrr.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://oqd.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://fpw.daxiang520.top

int size() const noexcept { return n_; }
来源：http://zrv.xuetiantiany.cn

[S53] C++：移动语义
来源：http://pta.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://ais.c1oappe.top

[S54] C++：异常处理
来源：http://hdg.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://plp.fehbvm.com

[S55] C++：结构化绑定
来源：http://usb.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://irg.xylfe.cn

[S56] C++：optional
来源：http://sdp.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://klt.hnqzz.top

[S57] C++：编译期常量
来源：http://mug.yuanzhike.top

constexpr int N = 10;
来源：http://mmz.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://jyt.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://fwx.yonumen.top

[S59] C++：静态断言
来源：http://gqj.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yjv.iojbl.cn

[S60] C++：遍历并删除元素
来源：http://olk.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fpy.zhaomingkeji.xyz

================================================================================
来源：http://jxp.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://adi.feifeiyinyue.top

================================================================================
来源：http://soc.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://ome.yongpay.top

println("Hello")
来源：http://hqm.andypj.xyz

[T02] Kotlin：变量
来源：http://omg.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qbx.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://drs.cashguo.top

"值: $b"
来源：http://pmo.yuanzhike.top

[T04] Kotlin：空安全
来源：http://kzk.ivvv.top

val n: String? = null;  n?.length
来源：http://yvi.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://zqq.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ngy.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://awx.shanyushiyangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bax.shanyushiyangkeji.top

[T07] Kotlin：集合过滤
来源：http://ncf.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hgt.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://ycc.cheryme.top

data class User(val name: String, val age: Int)
来源：http://xcs.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://cwp.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://xxj.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://jzy.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://klk.smart0.xyz

[T11] Kotlin：协程
来源：http://nlc.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qah.aizwys.cn

[T12] Kotlin：解构声明
来源：http://cfv.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://hme.guowangkeji.top

[T13] Kotlin：只读 Map
来源：http://bbq.yj20258888.top

val m = mapOf("a" to 1)
来源：http://pel.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://tyg.hcnkem.com

for (i in 1..10) println(i)
来源：http://qzx.haohaochexian.top

[T15] Kotlin：接口
来源：http://utk.fehbvm.com

interface Shape { fun area(): Double }
来源：http://jzw.fehbvm.com

[T16] Swift：Hello World
来源：http://nbb.shanyushiyangkeji.top

print("Hello")
来源：http://nxd.hfpthk.cn

[T17] Swift：变量与常量
来源：http://xil.xinyue.icu

var a = 1;  let b = 2
来源：http://hrn.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://fyc.chenjidiqi.icu

"值: \(b)"
来源：http://wjw.yfazqb.com

[T19] Swift：可选绑定
来源：http://jjz.kuanghao11.cn

if let n = opt { print(n) }
来源：http://zqi.sxryk.cn

[T20] Swift：数组操作
来源：http://qea.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://hyf.fengsongda.top

[T21] Swift：遍历
来源：http://nxq.zycfv.cn

for x in a { print(x) }
来源：http://tmp.quarkkingdee.top

[T22] Swift：字典
来源：http://oon.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://bbc.quarkkingdee.top

[T23] Swift：函数
来源：http://nff.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xht.yj20258.top

[T24] Swift：闭包
来源：http://xqe.havefunace.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uqy.xingfuxueyuan.xyz

[T25] Swift：结构体
来源：http://pnp.yuanzhike.top

struct P { var x: Int }
来源：http://dwi.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://aym.nanxinkj.top

class A: Base { override func f() {} }
来源：http://fat.vqdsnc.cn

[T27] Swift：错误处理
来源：http://sjy.316326.xyz

do { try f() } catch { print(error) }
来源：http://twv.c1oappe.top

[T28] Swift：枚举
来源：http://izr.wangshuangyany.cn

enum Color { case red, green }
来源：http://iuk.andypj.xyz

[T29] Swift：guard 提前返回
来源：http://dox.sufxvd.cn

guard let x = opt else { return }
来源：http://onx.redwolf501.top

[T30] Swift：协议
来源：http://tzo.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://nnc.tanke756.top

[T31] Lua：Hello World
来源：http://tjq.havefunace.top

print("Hello")
来源：http://ihs.smart0.xyz

[T32] Lua：局部变量
来源：http://ljh.yanxiufei.cn

local a = 1
来源：http://mrf.cucudq.cn

[T33] Lua：表（数组）
来源：http://ruw.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://znn.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://ndq.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://unr.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://ups.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://tyu.guowangkeji.top

[T36] Lua：函数
来源：http://nos.haohaochexian.top

function add(a, b) return a + b end
来源：http://agi.52xcode.cn

[T37] Lua：字符串拼接
来源：http://iiq.nwbrower.top

"a" .. "b"
来源：http://rll.shzxlz.cn

[T38] Lua：条件
来源：http://hbs.ctjpmb.com

if x > 0 then print("正") end
来源：http://ccu.xinyue.icu

[T39] Lua：模式匹配
来源：http://gjs.hfpthk.cn

string.find(s, "%d+")
来源：http://dai.bjfxy.top

[T40] Lua：元表
来源：http://ozf.birdmap.top

setmetatable({}, { __index = base })
来源：http://vqd.daxiang520.top

[T41] Perl：Hello World
来源：http://kwd.guowangkeji.top

print "Hello\n";
来源：http://zhq.zhoulong.xyz

[T42] Perl：变量类型
来源：http://bos.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yfn.nwbrower.top

[T43] Perl：字符串插值
来源：http://jco.hywenlv.cn

"值: $a"
来源：http://bfs.redwolf501.top

[T44] Perl：条件
来源：http://obb.fehbvm.com

if ($a > 0) { print "正"; }
来源：http://caq.snrcjt.cn

[T45] Perl：数组遍历
来源：http://efx.ywan-chungtsiang.top

for my $x (@arr) { print $x; }
来源：http://sdf.jqgfzy.top

[T46] Perl：哈希操作
来源：http://zxc.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bqy.ydzc1.top

[T47] Perl：正则捕获
来源：http://rvm.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xlw.jlsjyb.cn

[T48] Perl：正则替换
来源：http://tji.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://xtq.zhixingplan.top

[T49] Perl：函数
来源：http://tkz.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qzv.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://zfy.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://qsg.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://stu.svipenyu.cn

[T51] Scala：Hello World
来源：http://red.hnxiangtu.top

println("Hello")
来源：http://nxz.tanke756.top

[T52] Scala：变量
来源：http://bcl.zdbjq.cn

val a = 1;  var b = 2
来源：http://poe.tian-w.cn

[T53] Scala：字符串插值
来源：http://aeu.gzhubu.top

s"值: $b"
来源：http://zoz.fengsongda.top

[T54] Scala：集合映射
来源：http://vdh.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://dyn.chenzaomai.com

[T55] Scala：集合过滤
来源：http://opb.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://biz.nanxinkj.top

[T56] Scala：样例类
来源：http://svy.sweek.top

case class User(name: String, age: Int)
来源：http://brh.jiagoushi.top

[T57] Scala：模式匹配
来源：http://lqh.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://wby.zhixingplan.top

[T58] Scala：函数定义
来源：http://qum.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://axt.vehdjk.com

[T59] Scala：循环
来源：http://hwe.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://mnk.uphjek.com

[T60] Scala：折叠
来源：http://bae.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uzi.feifeiyinyue.top

================================================================================
来源：http://gid.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ncc.daxiang520.top

================================================================================
来源：http://fao.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://pxs.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://zfv.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://jry.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ord.yj202588.top

[U03] Py：加载 .env 配置
来源：http://rlj.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://lbn.dashuyun.cn

[U04] Py：变量调试打印
来源：http://nro.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gje.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://yap.jqgufenzy.top

list(dict.fromkeys(arr))
来源：http://hga.316326.xyz

[U06] Py：合并两个字典
来源：http://qba.c1oappe.top

{**a, **b}
来源：http://ons.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://ycg.yueranfly.top

{v: k for k, v in d.items()}
来源：http://tie.ydjk.org.cn

[U08] Py：展平二维列表
来源：http://tuo.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://acm.uphjek.com

[U09] Py：字典取最大值的键
来源：http://qbk.tian-w.cn

max(d, key=d.get)
来源：http://nfk.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://rqf.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fos.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://ecp.9152youxi.cn

(x * 2 for x in arr)
来源：http://gwk.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://crt.yj202588.top

Counter(arr).most_common(3)
来源：http://byf.ivvv.top

[U13] Py：固定长度队列
来源：http://jmq.yueranfly.top

deque(maxlen=10)
来源：http://pcv.daria6918.cn

[U14] Py：分组收集到列表
来源：http://tuv.ivvv.top

defaultdict(list)
来源：http://yrw.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://mer.kuanghao11.cn

t = time.perf_counter()
来源：http://sng.316326.xyz

[U16] Py：命令行参数解析
来源：http://eyj.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://znf.birdmap.top

[U17] Py：初始化日志
来源：http://znj.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://kje.yj20258888.top

[U18] Py：预编译正则
来源：http://ont.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://xtu.andypj.xyz

[U19] Py：正则替换带回调
来源：http://smc.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://efc.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://pfe.xinyue.icu

@functools.lru_cache(maxsize=None)
来源：http://tew.snrcjt.cn

[U21] Py：自定义上下文管理器
来源：http://kya.ctjpmb.com

@contextlib.contextmanager
来源：http://jgi.daria6918.cn

[U22] Py：矩阵转置
来源：http://gbn.meibo888.top

list(zip(*m))
来源：http://rwx.hnqzz.top

[U23] Py：分块读取大文件
来源：http://zzp.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mir.mhx1999.top

[U24] Py：路径操作
来源：http://vzf.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bhy.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://gmw.sufxvd.cn

csv.DictReader(f)
来源：http://wkn.jianghu66.top

[U26] Py：并发下载
来源：http://pqk.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yll.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://eco.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://uom.redwolf501.top

[U28] Py：类型别名
来源：http://mpx.zdqjudy.top

UserId = int
来源：http://eec.dianchejie.cn

[U29] Py：属性校验
来源：http://sup.chenzaomai.com

@property 与 @x.setter 配合
来源：http://knt.sufxvd.cn

[U30] Py：数据类
来源：http://dfq.gzhubu.top

@dataclass(slots=True)
来源：http://jdi.bjfxy.top

[U31] Py：单测
来源：http://tkx.shuidangran.top

python -m pytest -q
来源：http://sqe.chenzaomai.com

[U32] Py：代码格式化
来源：http://ucq.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://mnu.c1oappe.top

[U33] Py：打包发布
来源：http://pdx.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://tqh.yuxming.cn

[U34] Py：判断编码
来源：http://gdw.havefunace.top

chardet.detect(raw)
来源：http://evq.sysykeji.top

[U35] Py：发送邮件
来源：http://eav.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gbq.dianchejie.cn

[U36] Py：定时任务
来源：http://kxx.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://fxn.shangyingyoupin.top

[U37] Py：读写 Excel
来源：http://tio.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vip.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://nnt.sxryk.cn

Path(__file__).resolve().parent
来源：http://vqp.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://jgp.dianchejie.cn

sys.stdout.isatty()
来源：http://oue.fengsongda.top

[U40] Py：打印到标准错误
来源：http://dpi.guannengcc.top

print("err", file=sys.stderr)
来源：http://vdr.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://psg.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://cea.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://anl.mhx1999.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ytl.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://ezs.zhixingplan.top

namespace App\Http;
来源：http://vib.xziqi.cn

[U44] PHP：开启严格类型
来源：http://yqq.wangshuangyany.cn

declare(strict_types=1);
来源：http://cdk.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://whp.svipenyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://plh.gaohongyu789.top

[U46] PHP：可空类型
来源：http://whq.svipenyu.cn

?string $name = null
来源：http://cfu.ctjpmb.com

[U47] PHP：联合类型
来源：http://qzz.ybcxt.top

int|string $id
来源：http://qpx.guannengcc.top

[U48] PHP：纯枚举
来源：http://xmk.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hok.svipenyu.cn

[U49] PHP：只读属性
来源：http://miv.zhixingplan.top

public readonly string $name
来源：http://wck.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://urr.jianghu66.top

public function __construct(private int $id) {}
来源：http://ofg.yvedp.cn

[U51] PHP：数组解构
来源：http://com.zdbjq.cn

[$a, $b] = $arr;
来源：http://fnc.fzhhl.top

[U52] PHP：箭头函数
来源：http://vfm.redwolf501.top

$double = fn($x) => $x * 2;
来源：http://knd.meibo888.top

[U53] PHP：空合并运算符
来源：http://fva.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://hea.birdmap.top

[U54] PHP：空安全调用
来源：http://ljm.xziqi.cn

$obj?->method()
来源：http://wpq.aibaodan.cn

[U55] PHP：match 表达式
来源：http://chh.yangfankeji.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ycu.zhongyouzk.top

[U56] PHP：命名参数
来源：http://yju.ehwqpu.com

f(a: 1, b: 2)
来源：http://ifx.pycfn.com

[U57] PHP：字符串插值
来源：http://sue.iojbl.cn

"值: {$a}"
来源：http://clb.guannengcc.top

[U58] PHP：数组三件套
来源：http://waj.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rwv.hesvh.cn

[U59] PHP：自定义排序
来源：http://cnj.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ngv.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://rjl.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bah.havefunace.top

[U61] PHP：正则
来源：http://ynn.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yjk.ydzc1.top

[U62] PHP：日期对象
来源：http://klz.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://awk.zhoulong.xyz

[U63] PHP：文件读写
来源：http://aga.haohaochexian.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wvu.pycfn.com

[U64] PHP：目录遍历
来源：http://tbo.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://dja.epnwcf.com

[U65] PHP：会话
来源：http://jbd.gotoacloud.top

session_start();  $_SESSION["uid"] = 1;
来源：http://miy.zhijiandao.cn

[U66] PHP：设置 Cookie
来源：http://qxj.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://adg.0kj1m.cn


<!-- 参考信息 -->