代发 wailian999

[S41] C++：类与构造函数
来源：http://rvo.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://agn.daria6918.cn

[S42] C++：继承与虚函数
来源：http://zav.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://ibr.ydjk.org.cn

[S43] C++：智能指针
来源：http://tzu.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://okx.jyoumei.cn

[S44] C++：引用传参
来源：http://pnv.birdmap.top

void inc(int &x) { ++x; }
来源：http://bmg.zhixingplan.top

[S45] C++：lambda
来源：http://nii.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uhq.ydzc1.top

[S46] C++：函数模板
来源：http://xqh.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xbl.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://myl.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hjv.dianchejie.cn

[S48] C++：逐行读文件
来源：http://mjb.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://leg.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://scl.jyoumei.cn

[S49] C++：写文件
来源：http://ssw.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hpu.tian-w.cn

[S50] C++：格式化数字
来源：http://uyj.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://prp.aibaodan.cn

[S51] C++：显式类型转换
来源：http://aai.0kj1m.cn

static_cast<double>(a) / b
来源：http://lzj.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://ilc.hnqzz.top

int size() const noexcept { return n_; }
来源：http://ovt.cqqwz.cn

[S53] C++：移动语义
来源：http://sbm.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://egn.yuanzhike.top

[S54] C++：异常处理
来源：http://zsm.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nks.hesvh.cn

[S55] C++：结构化绑定
来源：http://hzw.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://myx.yangfankeji.com

[S56] C++：optional
来源：http://ijo.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sez.hfpthk.cn

[S57] C++：编译期常量
来源：http://cyg.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://nux.yueranfly.top

[S58] C++：命名空间
来源：http://dqv.sysykeji.top

namespace ns { int f() { return 1; } }
来源：http://rfw.epnwcf.com

[S59] C++：静态断言
来源：http://fcj.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fjq.hammf.cn

[S60] C++：遍历并删除元素
来源：http://hvl.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ydv.hammf.cn

================================================================================
来源：http://zpl.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://grw.chenlongwang.top

================================================================================
来源：http://oor.52xcode.cn

[T01] Kotlin：Hello World
来源：http://igd.zhoulong.xyz

println("Hello")
来源：http://fzr.xuanzx.com

[T02] Kotlin：变量
来源：http://rmh.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bzu.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://mwb.sxryk.cn

"值: $b"
来源：http://iil.snrcjt.cn

[T04] Kotlin：空安全
来源：http://gui.aizwys.cn

val n: String? = null;  n?.length
来源：http://xtu.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://ynn.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ogz.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://gyu.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rrx.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://wcd.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://crm.ehwqpu.com

[T08] Kotlin：数据类
来源：http://fiw.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://qdf.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://kuu.ydzc1.top

fun String.exclaim() = this + "!"
来源：http://kwy.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://kwp.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kpq.nwbrower.top

[T11] Kotlin：协程
来源：http://lld.jinyuanbaomall.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iyy.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://etv.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://iic.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://okd.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://jen.gotoacloud.top

[T14] Kotlin：循环
来源：http://rxv.jyoumei.cn

for (i in 1..10) println(i)
来源：http://uus.aibaodan.cn

[T15] Kotlin：接口
来源：http://eys.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://nwn.zycfv.cn

[T16] Swift：Hello World
来源：http://sfz.kuanghao11.cn

print("Hello")
来源：http://xgz.chenlongwang.top

[T17] Swift：变量与常量
来源：http://ohz.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://okt.fktsv.cn

[T18] Swift：字符串插值
来源：http://npf.ppjwa.cn

"值: \(b)"
来源：http://ikv.dashuyun.cn

[T19] Swift：可选绑定
来源：http://ihq.dashuyun.cn

if let n = opt { print(n) }
来源：http://ggz.shuidangran.top

[T20] Swift：数组操作
来源：http://pvm.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ocl.nanxuanxn.top

[T21] Swift：遍历
来源：http://tzu.jqgfzy.top

for x in a { print(x) }
来源：http://dnd.dianchejie.cn

[T22] Swift：字典
来源：http://swx.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xdt.andypj.xyz

[T23] Swift：函数
来源：http://mds.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bkd.zdbjq.cn

[T24] Swift：闭包
来源：http://iok.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ubz.zhengqikj.top

[T25] Swift：结构体
来源：http://yvr.yvedp.cn

struct P { var x: Int }
来源：http://avu.sjlbkw.cn

[T26] Swift：类与重写
来源：http://ptp.xuanzx.com

class A: Base { override func f() {} }
来源：http://iwp.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://hnc.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://jjy.tian-w.cn

[T28] Swift：枚举
来源：http://cit.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://rwl.pycfn.com

[T29] Swift：guard 提前返回
来源：http://njl.yfazqb.com

guard let x = opt else { return }
来源：http://xwz.guowangkeji.top

[T30] Swift：协议
来源：http://pxg.yj20258888.top

protocol Shape { func area() -> Double }
来源：http://kaa.hcnkem.com

[T31] Lua：Hello World
来源：http://vhu.jinghuilouyu.cn

print("Hello")
来源：http://tja.tian-w.cn

[T32] Lua：局部变量
来源：http://uez.uphjek.com

local a = 1
来源：http://siz.xziqi.cn

[T33] Lua：表（数组）
来源：http://xrl.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sij.jiagoushi.top

[T34] Lua：遍历表
来源：http://qwi.andypj.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://gup.uphjek.com

[T35] Lua：字典表
来源：http://czp.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://tkd.jinqigfzy.top

[T36] Lua：函数
来源：http://nas.sjlbkw.cn

function add(a, b) return a + b end
来源：http://lbj.fzhhl.top

[T37] Lua：字符串拼接
来源：http://euq.dianchejie.cn

"a" .. "b"
来源：http://naj.zhiwuduotai.top

[T38] Lua：条件
来源：http://pgs.smart0.xyz

if x > 0 then print("正") end
来源：http://ocy.yueranfly.top

[T39] Lua：模式匹配
来源：http://tmj.jqgufenzy.top

string.find(s, "%d+")
来源：http://yyi.wangdashe.top

[T40] Lua：元表
来源：http://wsj.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://fmi.snrcjt.cn

[T41] Perl：Hello World
来源：http://gqn.yongpay.top

print "Hello\n";
来源：http://ywd.vehdjk.com

[T42] Perl：变量类型
来源：http://wyz.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tov.nanxuanxn.top

[T43] Perl：字符串插值
来源：http://rld.yanxiufei.cn

"值: $a"
来源：http://wal.ivvv.top

[T44] Perl：条件
来源：http://iup.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://wbj.cdnleiting.top

[T45] Perl：数组遍历
来源：http://fyx.zhijiandao.cn

for my $x (@arr) { print $x; }
来源：http://jfv.guowangkeji.top

[T46] Perl：哈希操作
来源：http://ajc.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ebj.haohaochexian.top

[T47] Perl：正则捕获
来源：http://ibb.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qrs.gotoacloud.top

[T48] Perl：正则替换
来源：http://ivz.pycfn.com

$s =~ s/old/new/g;
来源：http://coi.feifeiyinyue.top

[T49] Perl：函数
来源：http://guz.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sex.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://mja.52xcode.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lcm.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://jyy.tianlin.xyz

[T51] Scala：Hello World
来源：http://kcg.shanyushiyangkeji.top

println("Hello")
来源：http://buq.mhx1999.top

[T52] Scala：变量
来源：http://hix.hnqzz.top

val a = 1;  var b = 2
来源：http://oxz.ctjpmb.com

[T53] Scala：字符串插值
来源：http://meb.zdbjq.cn

s"值: $b"
来源：http://zkp.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://aek.hammf.cn

List(1, 2, 3).map(_ * 2)
来源：http://kgw.ehwqpu.com

[T55] Scala：集合过滤
来源：http://ldn.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://dte.zhongyouzk.top

[T56] Scala：样例类
来源：http://vnv.yuxming.cn

case class User(name: String, age: Int)
来源：http://wkx.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://ytc.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://arr.wangdashe.top

[T58] Scala：函数定义
来源：http://wmb.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://kaa.hongshengwenyu.top

[T59] Scala：循环
来源：http://ict.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://sed.jyoumei.cn

[T60] Scala：折叠
来源：http://rpf.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://shs.fzhhl.top

================================================================================
来源：http://far.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yru.redwolf501.top

================================================================================
来源：http://fkg.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://chk.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://szu.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://jjd.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vtb.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://wrj.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vbn.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://dci.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gtj.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://rnc.zhengqikj.top

list(dict.fromkeys(arr))
来源：http://ojq.yvedp.cn

[U06] Py：合并两个字典
来源：http://sre.cheryme.top

{**a, **b}
来源：http://fxa.bjfxy.top

[U07] Py：反转字典键值
来源：http://srh.xuanzx.com

{v: k for k, v in d.items()}
来源：http://qai.feifeiyinyue.top

[U08] Py：展平二维列表
来源：http://uas.jyoumei.cn

[y for x in nested for y in x]
来源：http://ffa.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://kgj.yanxiufei.cn

max(d, key=d.get)
来源：http://jjq.nwbrower.top

[U10] Py：按值排序字典
来源：http://mgd.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dgm.yfazqb.com

[U11] Py：生成器表达式
来源：http://bam.0kj1m.cn

(x * 2 for x in arr)
来源：http://zjb.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://tco.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://mlz.tianlin.xyz

[U13] Py：固定长度队列
来源：http://xmo.nanxinkj.top

deque(maxlen=10)
来源：http://rjj.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://knx.zhengqikj.top

defaultdict(list)
来源：http://fob.zycfv.cn

[U15] Py：高精度计时
来源：http://zej.cdnleiting.top

t = time.perf_counter()
来源：http://xyq.wangdashe.top

[U16] Py：命令行参数解析
来源：http://gia.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qro.nanxuanxn.top

[U17] Py：初始化日志
来源：http://vdr.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://mtj.tanke756.top

[U18] Py：预编译正则
来源：http://bqh.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://mtj.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://gko.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nhq.yfazqb.com

[U20] Py：缓存函数结果
来源：http://ssw.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://gaw.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://jlo.guannengcc.top

@contextlib.contextmanager
来源：http://qqu.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://tcd.yueranfly.top

list(zip(*m))
来源：http://pqa.bjfxy.top

[U23] Py：分块读取大文件
来源：http://qhj.yfazqb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wbe.birdmap.top

[U24] Py：路径操作
来源：http://zlm.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qjc.havefunace.top

[U25] Py：CSV 按字典读
来源：http://kpi.xylfe.cn

csv.DictReader(f)
来源：http://ebm.andypj.xyz

[U26] Py：并发下载
来源：http://taj.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hbr.dianchejie.cn

[U27] Py：异步 HTTP
来源：http://duy.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://dog.yvedp.cn

[U28] Py：类型别名
来源：http://lzj.sufxvd.cn

UserId = int
来源：http://qql.jinqigufen.top

[U29] Py：属性校验
来源：http://rns.fzhhl.top

@property 与 @x.setter 配合
来源：http://sak.chenjidiqi.icu

[U30] Py：数据类
来源：http://nik.andypj.xyz

@dataclass(slots=True)
来源：http://fvf.tanke756.top

[U31] Py：单测
来源：http://wcd.chenlongwang.top

python -m pytest -q
来源：http://tew.zdqjudy.top

[U32] Py：代码格式化
来源：http://bio.cashguo.top

ruff format . && ruff check --fix .
来源：http://yvd.0kj1m.cn

[U33] Py：打包发布
来源：http://lua.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://pun.nanxuanxn.top

[U34] Py：判断编码
来源：http://hdh.nwbrower.top

chardet.detect(raw)
来源：http://zje.vehdjk.com

[U35] Py：发送邮件
来源：http://txq.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cvm.yvedp.cn

[U36] Py：定时任务
来源：http://day.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://msv.fktsv.cn

[U37] Py：读写 Excel
来源：http://nvl.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vpo.cdnleiting.top

[U38] Py：获取脚本所在目录
来源：http://ytf.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://vye.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://ibu.jianghu66.top

sys.stdout.isatty()
来源：http://snr.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://fym.zhixingplan.top

print("err", file=sys.stderr)
来源：http://woo.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://dok.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lhc.hnqzz.top

[U42] PHP：PSR-4 自动加载
来源：http://npx.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://phd.mhx1999.top

[U43] PHP：声明命名空间
来源：http://agk.jinghuilouyu.cn

namespace App\Http;
来源：http://hkj.bjfxy.top

[U44] PHP：开启严格类型
来源：http://xxs.andypj.xyz

declare(strict_types=1);
来源：http://lln.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://ofw.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://bdq.wangdashe.top

[U46] PHP：可空类型
来源：http://taj.cheryme.top

?string $name = null
来源：http://fgo.zdbjq.cn

[U47] PHP：联合类型
来源：http://cyv.kuanghao11.cn

int|string $id
来源：http://nsw.tarul.cn

[U48] PHP：纯枚举
来源：http://bbg.bjfxy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nbv.mhx1999.top

[U49] PHP：只读属性
来源：http://kan.0kj1m.cn

public readonly string $name
来源：http://yah.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://fwc.feifeiyinyue.top

public function __construct(private int $id) {}
来源：http://tdf.jyoumei.cn

[U51] PHP：数组解构
来源：http://cfw.hfpthk.cn

[$a, $b] = $arr;
来源：http://lxp.xuetiantiany.cn

[U52] PHP：箭头函数
来源：http://xvk.gotoacloud.top

$double = fn($x) => $x * 2;
来源：http://kdw.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://gqn.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://zqc.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://mwo.316326.xyz

$obj?->method()
来源：http://ifp.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://ybs.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wvi.daria6918.cn

[U56] PHP：命名参数
来源：http://jiq.sjlbkw.cn

f(a: 1, b: 2)
来源：http://ypp.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://hja.haohaochexian.top

"值: {$a}"
来源：http://kbk.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://oxv.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ysg.quarkkingdee.top

[U59] PHP：自定义排序
来源：http://isk.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://onu.hammf.cn

[U60] PHP：JSON 编解码
来源：http://jnv.hnxiangtu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sya.yj202588.top

[U61] PHP：正则
来源：http://grz.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gnl.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://qch.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dah.fehbvm.com

[U63] PHP：文件读写
来源：http://euw.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ysk.aizwys.cn

[U64] PHP：目录遍历
来源：http://ium.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://whz.zhongyouzk.top

[U65] PHP：会话
来源：http://kfj.jqgfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ooz.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://bpf.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lzk.hongshengwenyu.top


<!-- 参考信息 -->