代发 wailian999

[S33] C++：vector 增删
来源：http://vyg.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nat.ehwqpu.com

[S34] C++：遍历 vector
来源：http://mgk.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://zco.ehwqpu.com

[S35] C++：map
来源：http://bwr.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://omw.gaohongyu789.top

[S36] C++：unordered_map
来源：http://yht.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fqp.zhijiandao.cn

[S37] C++：set
来源：http://rvo.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hai.vqdsnc.cn

[S38] C++：排序
来源：http://zux.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://fyh.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://seh.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ixc.9152youxi.cn

[S40] C++：查找元素
来源：http://bfu.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yjv.yongpay.top

[S41] C++：类与构造函数
来源：http://wtp.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ceg.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://jpb.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://rbx.ybcxt.top

[S43] C++：智能指针
来源：http://gyq.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://imf.chenlongwang.top

[S44] C++：引用传参
来源：http://onf.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://yuk.shangyingyoupin.top

[S45] C++：lambda
来源：http://xhg.pengpengdd.cyou

auto add = [](int a, int b) { return a + b; };
来源：http://bhv.ehwqpu.com

[S46] C++：函数模板
来源：http://ebm.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nhr.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://zdt.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jfq.iojbl.cn

[S48] C++：逐行读文件
来源：http://lrf.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://rfn.yvedp.cn

while (std::getline(in, line)) { }
来源：http://avr.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://cns.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://taj.mhx1999.top

[S50] C++：格式化数字
来源：http://iwh.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://brh.yueranfly.top

[S51] C++：显式类型转换
来源：http://xrq.hywenlv.cn

static_cast<double>(a) / b
来源：http://awe.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://cfz.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://ivm.ydjk.org.cn

[S53] C++：移动语义
来源：http://bpy.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://pbj.jqgufenzy.top

[S54] C++：异常处理
来源：http://cpk.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://btr.xinyue.icu

[S55] C++：结构化绑定
来源：http://idq.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qpg.hammf.cn

[S56] C++：optional
来源：http://mql.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hsu.epnwcf.com

[S57] C++：编译期常量
来源：http://nhz.ppjwa.cn

constexpr int N = 10;
来源：http://zsp.yfazqb.com

[S58] C++：命名空间
来源：http://tfn.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://fzl.fzhhl.top

[S59] C++：静态断言
来源：http://wnq.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zwq.tarul.cn

[S60] C++：遍历并删除元素
来源：http://lrk.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fdw.bbcook.cn

================================================================================
来源：http://ytw.zycfv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cqj.nwbrower.top

================================================================================
来源：http://loc.jianghu66.top

[T01] Kotlin：Hello World
来源：http://umf.fzhhl.top

println("Hello")
来源：http://ccm.hysaishi.cn

[T02] Kotlin：变量
来源：http://gil.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hmq.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://vrd.ydzc1.top

"值: $b"
来源：http://gyc.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://dqk.316326.xyz

val n: String? = null;  n?.length
来源：http://pqf.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://lje.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aoa.sysykeji.top

[T06] Kotlin：集合映射
来源：http://hso.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://joa.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://wwp.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kkm.havefunace.top

[T08] Kotlin：数据类
来源：http://unw.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://ldp.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://jtm.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://geb.pycfn.com

[T10] Kotlin：默认参数
来源：http://kth.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://dwj.quarkkingdee.top

[T11] Kotlin：协程
来源：http://iqm.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uaw.316326.xyz

[T12] Kotlin：解构声明
来源：http://spq.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://err.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://gko.tanke756.top

val m = mapOf("a" to 1)
来源：http://dme.yanxiufei.cn

[T14] Kotlin：循环
来源：http://mzn.vehdjk.com

for (i in 1..10) println(i)
来源：http://idk.zdqjudy.top

[T15] Kotlin：接口
来源：http://qes.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://xtw.hammf.cn

[T16] Swift：Hello World
来源：http://rfk.zhiwuduotai.top

print("Hello")
来源：http://fjk.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://rzu.sufxvd.cn

var a = 1;  let b = 2
来源：http://exf.ehwqpu.com

[T18] Swift：字符串插值
来源：http://vln.ydjk.org.cn

"值: \(b)"
来源：http://jua.ivvv.top

[T19] Swift：可选绑定
来源：http://uiz.dianchejie.cn

if let n = opt { print(n) }
来源：http://blr.yongpay.top

[T20] Swift：数组操作
来源：http://szs.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uro.fktsv.cn

[T21] Swift：遍历
来源：http://fvf.svipenyu.cn

for x in a { print(x) }
来源：http://vwb.nanxuanxn.top

[T22] Swift：字典
来源：http://stp.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ijh.aizwys.cn

[T23] Swift：函数
来源：http://hgl.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gvr.xuetiantiany.cn

[T24] Swift：闭包
来源：http://qfa.yueranfly.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cbp.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://xpl.smart0.xyz

struct P { var x: Int }
来源：http://vkt.fehbvm.com

[T26] Swift：类与重写
来源：http://gvk.guowangkeji.top

class A: Base { override func f() {} }
来源：http://xcn.gotoacloud.top

[T27] Swift：错误处理
来源：http://pbe.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://dup.sufxvd.cn

[T28] Swift：枚举
来源：http://lgn.tian-w.cn

enum Color { case red, green }
来源：http://jki.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://esj.hfpthk.cn

guard let x = opt else { return }
来源：http://ztz.nanxuanxn.top

[T30] Swift：协议
来源：http://whx.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://oxf.iojbl.cn

[T31] Lua：Hello World
来源：http://jjr.dashuyun.cn

print("Hello")
来源：http://zrz.xinyue.icu

[T32] Lua：局部变量
来源：http://zme.birdmap.top

local a = 1
来源：http://cru.snrcjt.cn

[T33] Lua：表（数组）
来源：http://myo.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ixi.quarkkingdee.top

[T34] Lua：遍历表
来源：http://mkp.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ibf.daria6918.cn

[T35] Lua：字典表
来源：http://yvy.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://cte.yvedp.cn

[T36] Lua：函数
来源：http://ksr.dianchejie.cn

function add(a, b) return a + b end
来源：http://rlc.fengsongda.top

[T37] Lua：字符串拼接
来源：http://fnk.ivvv.top

"a" .. "b"
来源：http://cth.hysaishi.cn

[T38] Lua：条件
来源：http://ure.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://fmy.smart0.xyz

[T39] Lua：模式匹配
来源：http://sgu.yueranfly.top

string.find(s, "%d+")
来源：http://nah.316326.xyz

[T40] Lua：元表
来源：http://rmr.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://gxw.9152youxi.cn

[T41] Perl：Hello World
来源：http://psp.fengsongda.top

print "Hello\n";
来源：http://iit.gzhubu.top

[T42] Perl：变量类型
来源：http://fdv.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gll.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://zqt.vehdjk.com

"值: $a"
来源：http://zjc.zycfv.cn

[T44] Perl：条件
来源：http://lvv.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://fht.tarul.cn

[T45] Perl：数组遍历
来源：http://mbi.pycfn.com

for my $x (@arr) { print $x; }
来源：http://vxy.guowangkeji.top

[T46] Perl：哈希操作
来源：http://lbi.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dry.iojbl.cn

[T47] Perl：正则捕获
来源：http://elh.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pkt.yj20258.top

[T48] Perl：正则替换
来源：http://zuh.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://dri.ehwqpu.com

[T49] Perl：函数
来源：http://qca.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hqp.shuidangran.top

[T50] Perl：逐行读文件
来源：http://now.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bnl.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://xiu.uphjek.com

[T51] Scala：Hello World
来源：http://svt.xuanzx.com

println("Hello")
来源：http://ate.xylfe.cn

[T52] Scala：变量
来源：http://tyy.svipenyu.cn

val a = 1;  var b = 2
来源：http://jcr.smart0.xyz

[T53] Scala：字符串插值
来源：http://owa.zhongyouzk.top

s"值: $b"
来源：http://ogq.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://llx.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://ybf.hywenlv.cn

[T55] Scala：集合过滤
来源：http://edx.fehbvm.com

List(1, 2, 3).filter(_ > 1)
来源：http://agj.fzhhl.top

[T56] Scala：样例类
来源：http://vnb.yongpay.top

case class User(name: String, age: Int)
来源：http://gmh.hammf.cn

[T57] Scala：模式匹配
来源：http://jvc.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://bje.yuxming.cn

[T58] Scala：函数定义
来源：http://xef.zhengqikj.top

def add(a: Int, b: Int): Int = a + b
来源：http://qco.sysykeji.top

[T59] Scala：循环
来源：http://yab.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://tpb.ehwqpu.com

[T60] Scala：折叠
来源：http://uju.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nbq.bbcook.cn

================================================================================
来源：http://kwt.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ngv.xuetiantiany.cn

================================================================================
来源：http://ggp.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://cih.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tvs.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://wff.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mmd.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://rla.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mpr.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://hwy.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tly.fengsongda.top

[U05] Py：列表去重且保序
来源：http://qmn.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://yii.gzhubu.top

[U06] Py：合并两个字典
来源：http://smw.sweek.top

{**a, **b}
来源：http://zwk.sweek.top

[U07] Py：反转字典键值
来源：http://dhb.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://qat.jinghuilouyu.cn

[U08] Py：展平二维列表
来源：http://rch.redwolf501.top

[y for x in nested for y in x]
来源：http://ogj.hysaishi.cn

[U09] Py：字典取最大值的键
来源：http://nec.shanyushiyangkeji.top

max(d, key=d.get)
来源：http://iir.jianghu66.top

[U10] Py：按值排序字典
来源：http://heh.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://chm.tian-w.cn

[U11] Py：生成器表达式
来源：http://gqe.yuxming.cn

(x * 2 for x in arr)
来源：http://vfv.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://qbe.jlsjyb.cn

Counter(arr).most_common(3)
来源：http://owv.uphjek.com

[U13] Py：固定长度队列
来源：http://qhq.andypj.xyz

deque(maxlen=10)
来源：http://kmk.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://fny.316326.xyz

defaultdict(list)
来源：http://hup.yangfankeji.com

[U15] Py：高精度计时
来源：http://bri.yonumen.top

t = time.perf_counter()
来源：http://sjd.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://kvm.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cnp.shzxlz.cn

[U17] Py：初始化日志
来源：http://wcv.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://cku.yuanzhike.top

[U18] Py：预编译正则
来源：http://fod.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://xto.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://zyq.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rjj.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://dhy.zhiwuduotai.top

@functools.lru_cache(maxsize=None)
来源：http://zwp.zdqjudy.top

[U21] Py：自定义上下文管理器
来源：http://dtz.pycfn.com

@contextlib.contextmanager
来源：http://ezk.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://mgk.xziqi.cn

list(zip(*m))
来源：http://cuu.xinyue.icu

[U23] Py：分块读取大文件
来源：http://umo.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dph.jiagoushi.top

[U24] Py：路径操作
来源：http://rfx.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gqb.ybcxt.top

[U25] Py：CSV 按字典读
来源：http://jca.fanxiaobao.xyz

csv.DictReader(f)
来源：http://shj.ivvv.top

[U26] Py：并发下载
来源：http://jly.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qzt.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://ksu.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://jop.shuidangran.top

[U28] Py：类型别名
来源：http://tfq.xuetiantiany.cn

UserId = int
来源：http://kkq.zhengqikj.top

[U29] Py：属性校验
来源：http://iav.bjfxy.top

@property 与 @x.setter 配合
来源：http://uqi.tanke756.top

[U30] Py：数据类
来源：http://pvq.jinqigfzy.top

@dataclass(slots=True)
来源：http://alo.havefunace.top

[U31] Py：单测
来源：http://mqg.mhx1999.top

python -m pytest -q
来源：http://rkc.hnxiangtu.top

[U32] Py：代码格式化
来源：http://txo.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://hms.xuetiantiany.cn

[U33] Py：打包发布
来源：http://top.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://nhy.fzhhl.top

[U34] Py：判断编码
来源：http://zcs.chenjidiqi.icu

chardet.detect(raw)
来源：http://xvb.zdbjq.cn

[U35] Py：发送邮件
来源：http://xje.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kza.fengsongda.top

[U36] Py：定时任务
来源：http://foq.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://krb.yangfankeji.com

[U37] Py：读写 Excel
来源：http://qcl.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://kbk.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://pye.meibo888.top

Path(__file__).resolve().parent
来源：http://ulb.ydjk.org.cn

[U39] Py：判断是否在交互环境
来源：http://jup.sxryk.cn

sys.stdout.isatty()
来源：http://vfr.yj202588.top

[U40] Py：打印到标准错误
来源：http://htz.zdqjudy.top

print("err", file=sys.stderr)
来源：http://lvn.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://cem.hysaishi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://avh.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://aza.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kht.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://ews.shzxlz.cn

namespace App\Http;
来源：http://vse.smart0.xyz

[U44] PHP：开启严格类型
来源：http://wlq.ppjwa.cn

declare(strict_types=1);
来源：http://xry.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://qgi.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://anj.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://zhp.0kj1m.cn

?string $name = null
来源：http://amp.gaohongyu789.top

[U47] PHP：联合类型
来源：http://bba.guannengcc.top

int|string $id
来源：http://fra.birdmap.top

[U48] PHP：纯枚举
来源：http://ixr.yfazqb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://smh.zhaomingkeji.xyz

[U49] PHP：只读属性
来源：http://sjv.sweek.top

public readonly string $name
来源：http://dfn.wangshuangyany.cn

[U50] PHP：构造器属性提升
来源：http://khc.316326.xyz

public function __construct(private int $id) {}
来源：http://prq.aibaodan.cn

[U51] PHP：数组解构
来源：http://wci.jyoumei.cn

[$a, $b] = $arr;
来源：http://cef.svipenyu.cn

[U52] PHP：箭头函数
来源：http://aof.bbcook.cn

$double = fn($x) => $x * 2;
来源：http://ngs.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://ohx.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://vcm.wangdashe.top

[U54] PHP：空安全调用
来源：http://bwk.xuanzx.com

$obj?->method()
来源：http://ern.fengsongda.top

[U55] PHP：match 表达式
来源：http://yme.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wzs.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://unj.gotoacloud.top

f(a: 1, b: 2)
来源：http://hrf.zdqjudy.top

[U57] PHP：字符串插值
来源：http://use.xingfuxueyuan.xyz

"值: {$a}"
来源：http://hps.wangshuangyany.cn

[U58] PHP：数组三件套
来源：http://vtx.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lgi.tian-w.cn


<!-- 参考信息 -->