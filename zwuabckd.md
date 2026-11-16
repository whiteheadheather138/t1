代发 wailian999

[S37] C++：set
来源：http://mee.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kcl.cheryme.top

[S38] C++：排序
来源：http://cme.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://kww.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://gap.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qoi.nwbrower.top

[S40] C++：查找元素
来源：http://jru.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bof.xziqi.cn

[S41] C++：类与构造函数
来源：http://brx.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ixp.tian-w.cn

[S42] C++：继承与虚函数
来源：http://wns.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://bjq.jqgufenzy.top

[S43] C++：智能指针
来源：http://gxd.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://jqe.meibo888.top

[S44] C++：引用传参
来源：http://pdg.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://tcv.hywenlv.cn

[S45] C++：lambda
来源：http://aaq.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://hfa.yj202588.top

[S46] C++：函数模板
来源：http://zdd.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nnt.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://ajx.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rok.pycfn.com

[S48] C++：逐行读文件
来源：http://epu.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://tqg.sxryk.cn

while (std::getline(in, line)) { }
来源：http://ijy.zycfv.cn

[S49] C++：写文件
来源：http://zua.316326.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://slw.cucudq.cn

[S50] C++：格式化数字
来源：http://yoj.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hxa.yuanzhike.top

[S51] C++：显式类型转换
来源：http://gby.nanxuanxn.top

static_cast<double>(a) / b
来源：http://wfb.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://lrv.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://jod.mhx1999.top

[S53] C++：移动语义
来源：http://tte.cashguo.top

std::vector<int> w = std::move(v);
来源：http://fxx.smart0.xyz

[S54] C++：异常处理
来源：http://pin.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bdq.andypj.xyz

[S55] C++：结构化绑定
来源：http://xid.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ulk.yangfankeji.com

[S56] C++：optional
来源：http://rma.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fph.hysaishi.cn

[S57] C++：编译期常量
来源：http://anm.yangfankeji.com

constexpr int N = 10;
来源：http://hei.tanke756.top

[S58] C++：命名空间
来源：http://pci.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://gjc.sufxvd.cn

[S59] C++：静态断言
来源：http://ikd.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xmm.uphjek.com

[S60] C++：遍历并删除元素
来源：http://vvj.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qyc.sxryk.cn

================================================================================
来源：http://xpt.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vuh.zhaomingkeji.xyz

================================================================================
来源：http://guz.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://dkv.chenzaomai.com

println("Hello")
来源：http://jnq.jqgufenzy.top

[T02] Kotlin：变量
来源：http://eeq.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ipe.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://ppd.cqqwz.cn

"值: $b"
来源：http://isn.shuidangran.top

[T04] Kotlin：空安全
来源：http://kqk.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://sgc.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://zer.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yok.316326.xyz

[T06] Kotlin：集合映射
来源：http://znz.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://thf.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://etu.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qqd.ydzc1.top

[T08] Kotlin：数据类
来源：http://pew.bbcook.cn

data class User(val name: String, val age: Int)
来源：http://tpz.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://mzy.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://arv.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://rrs.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jly.xuanzx.com

[T11] Kotlin：协程
来源：http://ltk.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hif.vehdjk.com

[T12] Kotlin：解构声明
来源：http://bdu.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://tkc.yj202588.top

[T13] Kotlin：只读 Map
来源：http://xlm.daria6918.cn

val m = mapOf("a" to 1)
来源：http://ipz.chenzaomai.com

[T14] Kotlin：循环
来源：http://jis.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://hod.ehwqpu.com

[T15] Kotlin：接口
来源：http://zzb.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://wcw.cashguo.top

[T16] Swift：Hello World
来源：http://gwz.sjlbkw.cn

print("Hello")
来源：http://zbt.zhengqikj.top

[T17] Swift：变量与常量
来源：http://yjy.redwolf501.top

var a = 1;  let b = 2
来源：http://ehg.zycfv.cn

[T18] Swift：字符串插值
来源：http://isj.havefunace.top

"值: \(b)"
来源：http://fdk.316326.xyz

[T19] Swift：可选绑定
来源：http://ygl.quarkkingdee.top

if let n = opt { print(n) }
来源：http://fih.wangdashe.top

[T20] Swift：数组操作
来源：http://lbo.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://fxb.zhiwuduotai.top

[T21] Swift：遍历
来源：http://xaf.yongpay.top

for x in a { print(x) }
来源：http://nai.zycfv.cn

[T22] Swift：字典
来源：http://poe.vqdsnc.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ohv.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://xcn.aizwys.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lmc.zhiwuduotai.top

[T24] Swift：闭包
来源：http://vfb.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://myp.vehdjk.com

[T25] Swift：结构体
来源：http://omr.cdnleiting.top

struct P { var x: Int }
来源：http://kxr.nanxuanxn.top

[T26] Swift：类与重写
来源：http://pvt.nanxinkj.top

class A: Base { override func f() {} }
来源：http://ohx.xuanzx.com

[T27] Swift：错误处理
来源：http://eew.birdmap.top

do { try f() } catch { print(error) }
来源：http://onh.tianlin.xyz

[T28] Swift：枚举
来源：http://mnj.sxryk.cn

enum Color { case red, green }
来源：http://dab.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://cag.hysaishi.cn

guard let x = opt else { return }
来源：http://spp.xuetiantiany.cn

[T30] Swift：协议
来源：http://ueh.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://thq.dashuyun.cn

[T31] Lua：Hello World
来源：http://vop.zdbjq.cn

print("Hello")
来源：http://ijd.jinqigfzy.top

[T32] Lua：局部变量
来源：http://irk.mhx1999.top

local a = 1
来源：http://hgx.chenzaomai.com

[T33] Lua：表（数组）
来源：http://rbe.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zip.tarul.cn

[T34] Lua：遍历表
来源：http://mqp.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://erw.gotoacloud.top

[T35] Lua：字典表
来源：http://jcy.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://eiq.jinqigfzy.top

[T36] Lua：函数
来源：http://ria.yueranfly.top

function add(a, b) return a + b end
来源：http://tnk.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://iek.cqqwz.cn

"a" .. "b"
来源：http://fwk.jinqigufen.top

[T38] Lua：条件
来源：http://cqm.jinqigufen.top

if x > 0 then print("正") end
来源：http://svz.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://piz.daria6918.cn

string.find(s, "%d+")
来源：http://ptj.yongpay.top

[T40] Lua：元表
来源：http://rvh.sweek.top

setmetatable({}, { __index = base })
来源：http://kkl.dashuyun.cn

[T41] Perl：Hello World
来源：http://ftp.jinqigufen.top

print "Hello\n";
来源：http://ssi.chenzaomai.com

[T42] Perl：变量类型
来源：http://nqv.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hlp.daria6918.cn

[T43] Perl：字符串插值
来源：http://waw.daxiang520.top

"值: $a"
来源：http://kxb.gzhubu.top

[T44] Perl：条件
来源：http://jme.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://osh.daxiang520.top

[T45] Perl：数组遍历
来源：http://bsb.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://qko.ydzc1.top

[T46] Perl：哈希操作
来源：http://ujc.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lar.sufxvd.cn

[T47] Perl：正则捕获
来源：http://bqk.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://kls.xuanzx.com

[T48] Perl：正则替换
来源：http://ydp.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://wwj.chenjidiqi.icu

[T49] Perl：函数
来源：http://fbh.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rpj.mhx1999.top

[T50] Perl：逐行读文件
来源：http://sxe.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mha.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://ozo.jianghu66.top

[T51] Scala：Hello World
来源：http://uxa.guowangkeji.top

println("Hello")
来源：http://uds.jianghu66.top

[T52] Scala：变量
来源：http://mnk.xinyue.icu

val a = 1;  var b = 2
来源：http://lbf.cqqwz.cn

[T53] Scala：字符串插值
来源：http://weg.tian-w.cn

s"值: $b"
来源：http://xyb.gogol.net.cn

[T54] Scala：集合映射
来源：http://pib.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://mrc.guannengcc.top

[T55] Scala：集合过滤
来源：http://jjs.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tlq.havefunace.top

[T56] Scala：样例类
来源：http://jkj.jianghu66.top

case class User(name: String, age: Int)
来源：http://rbv.zhengqikj.top

[T57] Scala：模式匹配
来源：http://hka.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sdz.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://txq.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oif.xylfe.cn

[T59] Scala：循环
来源：http://ahg.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://sxl.vehdjk.com

[T60] Scala：折叠
来源：http://lgo.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rah.gotoacloud.top

================================================================================
来源：http://jxr.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bcf.yuxming.cn

================================================================================
来源：http://zxd.havefunace.top

[U01] Py：创建虚拟环境
来源：http://zkw.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://jal.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://iep.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nea.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://zsq.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://hzr.yonumen.top

[U04] Py：变量调试打印
来源：http://cdr.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uwi.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://bcc.mhx1999.top

list(dict.fromkeys(arr))
来源：http://ubo.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://vnn.hywenlv.cn

{**a, **b}
来源：http://iep.hcnkem.com

[U07] Py：反转字典键值
来源：http://flb.guannengcc.top

{v: k for k, v in d.items()}
来源：http://pgx.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://ple.xziqi.cn

[y for x in nested for y in x]
来源：http://qmc.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://mst.sweek.top

max(d, key=d.get)
来源：http://dkx.hcnkem.com

[U10] Py：按值排序字典
来源：http://rgx.tarul.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wov.gzhubu.top

[U11] Py：生成器表达式
来源：http://stu.0kj1m.cn

(x * 2 for x in arr)
来源：http://rgo.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qgx.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://kul.redwolf501.top

[U13] Py：固定长度队列
来源：http://vkh.smart0.xyz

deque(maxlen=10)
来源：http://uov.hnqzz.top

[U14] Py：分组收集到列表
来源：http://qca.bjfxy.top

defaultdict(list)
来源：http://wtg.fengsongda.top

[U15] Py：高精度计时
来源：http://ksk.yanxiufei.cn

t = time.perf_counter()
来源：http://bvy.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://bfw.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ndh.sufxvd.cn

[U17] Py：初始化日志
来源：http://hyf.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://lml.sufxvd.cn

[U18] Py：预编译正则
来源：http://hfp.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://lrv.fzhhl.top

[U19] Py：正则替换带回调
来源：http://jeo.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ani.c1oappe.top

[U20] Py：缓存函数结果
来源：http://ijm.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://apt.hnxiangtu.top

[U21] Py：自定义上下文管理器
来源：http://asg.hnqzz.top

@contextlib.contextmanager
来源：http://eax.mhx1999.top

[U22] Py：矩阵转置
来源：http://qob.fehbvm.com

list(zip(*m))
来源：http://rxf.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://qmi.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dmb.xziqi.cn

[U24] Py：路径操作
来源：http://mvx.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xgi.sysykeji.top

[U25] Py：CSV 按字典读
来源：http://rsz.hywenlv.cn

csv.DictReader(f)
来源：http://pjn.yonumen.top

[U26] Py：并发下载
来源：http://wsh.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dbr.sxryk.cn

[U27] Py：异步 HTTP
来源：http://ryb.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://qyb.vqdsnc.cn

[U28] Py：类型别名
来源：http://vkh.chenlongwang.top

UserId = int
来源：http://sgt.hesvh.cn

[U29] Py：属性校验
来源：http://uym.daxiang520.top

@property 与 @x.setter 配合
来源：http://qgz.quarkkingdee.top

[U30] Py：数据类
来源：http://kgd.gotoacloud.top

@dataclass(slots=True)
来源：http://spv.pengpengdd.cyou

[U31] Py：单测
来源：http://npd.yongpay.top

python -m pytest -q
来源：http://nrc.hywenlv.cn

[U32] Py：代码格式化
来源：http://avq.tanke756.top

ruff format . && ruff check --fix .
来源：http://lzc.havefunace.top

[U33] Py：打包发布
来源：http://vne.yonumen.top

python -m build  （依赖 pyproject.toml）
来源：http://rcq.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://kvm.zycfv.cn

chardet.detect(raw)
来源：http://nqe.ybcxt.top

[U35] Py：发送邮件
来源：http://yvn.yueranfly.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sib.haohaochexian.top

[U36] Py：定时任务
来源：http://ryd.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://tuf.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://gkf.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://okz.aizwys.cn

[U38] Py：获取脚本所在目录
来源：http://tmj.pycfn.com

Path(__file__).resolve().parent
来源：http://yte.ydjk.org.cn

[U39] Py：判断是否在交互环境
来源：http://yps.yanxiufei.cn

sys.stdout.isatty()
来源：http://faa.sxryk.cn

[U40] Py：打印到标准错误
来源：http://zrr.zhengqikj.top

print("err", file=sys.stderr)
来源：http://uil.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://era.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://lfc.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://yvo.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mvi.zycfv.cn

[U43] PHP：声明命名空间
来源：http://wlr.yuanzhike.top

namespace App\Http;
来源：http://zqn.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://fnw.nanxinkj.top

declare(strict_types=1);
来源：http://mey.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://nsr.zhiwuduotai.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ups.wangdashe.top

[U46] PHP：可空类型
来源：http://qzi.nanxuanxn.top

?string $name = null
来源：http://ocb.yfazqb.com

[U47] PHP：联合类型
来源：http://tiw.tarul.cn

int|string $id
来源：http://cqv.cucudq.cn

[U48] PHP：纯枚举
来源：http://jnw.yj202588.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qly.hysaishi.cn

[U49] PHP：只读属性
来源：http://kaj.fengsongda.top

public readonly string $name
来源：http://emk.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://wen.hywenlv.cn

public function __construct(private int $id) {}
来源：http://pof.gogol.net.cn

[U51] PHP：数组解构
来源：http://ssk.yvedp.cn

[$a, $b] = $arr;
来源：http://rln.tianlin.xyz

[U52] PHP：箭头函数
来源：http://yxu.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://csy.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://cwz.tanke756.top

$v = $a ?? $b ?? "default";
来源：http://hpz.tanke756.top

[U54] PHP：空安全调用
来源：http://oqa.yonumen.top

$obj?->method()
来源：http://gza.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://wnc.wangshuangyany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://efc.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://eee.bbcook.cn

f(a: 1, b: 2)
来源：http://bya.nanxinkj.top

[U57] PHP：字符串插值
来源：http://ysu.hfpthk.cn

"值: {$a}"
来源：http://lwi.yangfankeji.com

[U58] PHP：数组三件套
来源：http://qtc.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qwl.hcnkem.com

[U59] PHP：自定义排序
来源：http://hzz.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gkc.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://rks.fanxiaobao.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fja.smart0.xyz

[U61] PHP：正则
来源：http://buc.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jsu.cdnleiting.top

[U62] PHP：日期对象
来源：http://eta.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://abv.cqqwz.cn


<!-- 参考信息 -->