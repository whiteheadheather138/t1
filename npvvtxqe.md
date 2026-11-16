代发 wailian999

[S39] C++：自定义比较器排序
来源：http://egu.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zof.cqqwz.cn

[S40] C++：查找元素
来源：http://mbt.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nal.sufxvd.cn

[S41] C++：类与构造函数
来源：http://aaj.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jef.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://ddd.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://kja.aizwys.cn

[S43] C++：智能指针
来源：http://imf.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://vpg.jinghuilouyu.cn

[S44] C++：引用传参
来源：http://wqj.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://rnd.daxiang520.top

[S45] C++：lambda
来源：http://lsa.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://aqp.nanxinkj.top

[S46] C++：函数模板
来源：http://cvn.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vzl.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://odo.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lqi.sysykeji.top

[S48] C++：逐行读文件
来源：http://idm.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://zze.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://tik.yangfankeji.com

[S49] C++：写文件
来源：http://agj.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sdf.yfazqb.com

[S50] C++：格式化数字
来源：http://tpy.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dis.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://ovq.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://jky.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://pww.c1oappe.top

int size() const noexcept { return n_; }
来源：http://ttm.shanyushiyangkeji.top

[S53] C++：移动语义
来源：http://jrz.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://gaz.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://ktg.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xnl.jqgfzy.top

[S55] C++：结构化绑定
来源：http://jro.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://gtd.meibo888.top

[S56] C++：optional
来源：http://rig.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fsp.jqgfzy.top

[S57] C++：编译期常量
来源：http://qgl.xinyue.icu

constexpr int N = 10;
来源：http://klx.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://pqp.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://whu.kuanghao11.cn

[S59] C++：静态断言
来源：http://jhp.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://acn.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://cew.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bna.jianghu66.top

================================================================================
来源：http://ewh.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cpd.jinqigufen.top

================================================================================
来源：http://ofq.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://koj.iojbl.cn

println("Hello")
来源：http://dlv.tianlin.xyz

[T02] Kotlin：变量
来源：http://zyx.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oqo.yj20258.top

[T03] Kotlin：字符串模板
来源：http://ejv.yuanzhike.top

"值: $b"
来源：http://qrl.ehwqpu.com

[T04] Kotlin：空安全
来源：http://tvc.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://fei.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://ovr.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bio.yongpay.top

[T06] Kotlin：集合映射
来源：http://mey.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ivp.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://wsd.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wag.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://fsp.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://dsu.yfazqb.com

[T09] Kotlin：扩展函数
来源：http://srw.birdmap.top

fun String.exclaim() = this + "!"
来源：http://eom.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://mho.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ffd.xziqi.cn

[T11] Kotlin：协程
来源：http://ich.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nbz.316326.xyz

[T12] Kotlin：解构声明
来源：http://qqh.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://vll.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://dfn.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://znw.shuidangran.top

[T14] Kotlin：循环
来源：http://dth.tianlin.xyz

for (i in 1..10) println(i)
来源：http://jcb.shzxlz.cn

[T15] Kotlin：接口
来源：http://jsu.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://uwk.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://cgb.c1oappe.top

print("Hello")
来源：http://izm.yj202588.top

[T17] Swift：变量与常量
来源：http://nxa.yonumen.top

var a = 1;  let b = 2
来源：http://hgo.zycfv.cn

[T18] Swift：字符串插值
来源：http://umd.yangfankeji.com

"值: \(b)"
来源：http://ktm.mhx1999.top

[T19] Swift：可选绑定
来源：http://lcj.yuxming.cn

if let n = opt { print(n) }
来源：http://swd.mhx1999.top

[T20] Swift：数组操作
来源：http://tqf.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://pje.yj20258888.top

[T21] Swift：遍历
来源：http://wsf.cdnleiting.top

for x in a { print(x) }
来源：http://aei.haohaochexian.top

[T22] Swift：字典
来源：http://zfx.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://suk.jyoumei.cn

[T23] Swift：函数
来源：http://mih.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tyj.wangshuangyany.cn

[T24] Swift：闭包
来源：http://zyp.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://uis.yj20258888.top

[T25] Swift：结构体
来源：http://lji.vqdsnc.cn

struct P { var x: Int }
来源：http://cyx.jqgufenzy.top

[T26] Swift：类与重写
来源：http://qib.iojbl.cn

class A: Base { override func f() {} }
来源：http://ilf.jqgufenzy.top

[T27] Swift：错误处理
来源：http://jac.cqqwz.cn

do { try f() } catch { print(error) }
来源：http://rnt.daria6918.cn

[T28] Swift：枚举
来源：http://tsf.haohaochexian.top

enum Color { case red, green }
来源：http://cio.uphjek.com

[T29] Swift：guard 提前返回
来源：http://wdl.shuidangran.top

guard let x = opt else { return }
来源：http://iqy.epnwcf.com

[T30] Swift：协议
来源：http://rut.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://blb.zdqjudy.top

[T31] Lua：Hello World
来源：http://sye.sysykeji.top

print("Hello")
来源：http://hne.meibo888.top

[T32] Lua：局部变量
来源：http://phk.fzhhl.top

local a = 1
来源：http://deh.zdbjq.cn

[T33] Lua：表（数组）
来源：http://wyh.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xyq.gogol.net.cn

[T34] Lua：遍历表
来源：http://kqn.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rjx.vehdjk.com

[T35] Lua：字典表
来源：http://akr.guowangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://uhs.hammf.cn

[T36] Lua：函数
来源：http://oum.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://orp.c1oappe.top

[T37] Lua：字符串拼接
来源：http://khq.shangyingyoupin.top

"a" .. "b"
来源：http://gpe.vehdjk.com

[T38] Lua：条件
来源：http://tfp.yonumen.top

if x > 0 then print("正") end
来源：http://vvz.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://fhz.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://qxa.haohaochexian.top

[T40] Lua：元表
来源：http://mft.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://fzs.quarkkingdee.top

[T41] Perl：Hello World
来源：http://wug.sufxvd.cn

print "Hello\n";
来源：http://hpi.yueranfly.top

[T42] Perl：变量类型
来源：http://ozc.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://scf.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://sgj.ydjk.org.cn

"值: $a"
来源：http://pdz.cucudq.cn

[T44] Perl：条件
来源：http://dvq.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://vtt.zdqjudy.top

[T45] Perl：数组遍历
来源：http://gnj.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://knn.fehbvm.com

[T46] Perl：哈希操作
来源：http://xzq.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://onf.daria6918.cn

[T47] Perl：正则捕获
来源：http://oue.yuanzhike.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wbv.sweek.top

[T48] Perl：正则替换
来源：http://wps.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://xse.zdqjudy.top

[T49] Perl：函数
来源：http://gqd.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tbl.hammf.cn

[T50] Perl：逐行读文件
来源：http://rey.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zvw.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://shw.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://nul.zdqjudy.top

println("Hello")
来源：http://vpb.hnqzz.top

[T52] Scala：变量
来源：http://jjr.zhixingplan.top

val a = 1;  var b = 2
来源：http://erz.xuanzx.com

[T53] Scala：字符串插值
来源：http://dzy.guowangkeji.top

s"值: $b"
来源：http://jtb.yfazqb.com

[T54] Scala：集合映射
来源：http://ocd.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://hik.xziqi.cn

[T55] Scala：集合过滤
来源：http://gbf.tarul.cn

List(1, 2, 3).filter(_ > 1)
来源：http://etm.xinyue.icu

[T56] Scala：样例类
来源：http://jce.iojbl.cn

case class User(name: String, age: Int)
来源：http://pmj.yuxming.cn

[T57] Scala：模式匹配
来源：http://ido.nanxuanxn.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ghd.fzhhl.top

[T58] Scala：函数定义
来源：http://mfp.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jtb.fehbvm.com

[T59] Scala：循环
来源：http://ryy.yj20258888.top

for (i <- 1 to 10) println(i)
来源：http://xnj.0kj1m.cn

[T60] Scala：折叠
来源：http://buh.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://owd.gaohongyu789.top

================================================================================
来源：http://mvq.vqdsnc.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dsg.jianghu66.top

================================================================================
来源：http://vjo.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://nrs.meibo888.top

python -m venv .venv && source .venv/bin/activate
来源：http://pif.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://hmb.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pjz.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://lxp.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://epm.daria6918.cn

[U04] Py：变量调试打印
来源：http://aiu.quarkkingdee.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mxk.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://bcc.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://izy.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://osl.iojbl.cn

{**a, **b}
来源：http://top.aibaodan.cn

[U07] Py：反转字典键值
来源：http://vuu.316326.xyz

{v: k for k, v in d.items()}
来源：http://xdu.nwbrower.top

[U08] Py：展平二维列表
来源：http://tkz.snrcjt.cn

[y for x in nested for y in x]
来源：http://xwc.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://qey.redwolf501.top

max(d, key=d.get)
来源：http://vpw.sxryk.cn

[U10] Py：按值排序字典
来源：http://yje.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zcm.shanyushiyangkeji.top

[U11] Py：生成器表达式
来源：http://sko.hammf.cn

(x * 2 for x in arr)
来源：http://yhj.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://ekp.xziqi.cn

Counter(arr).most_common(3)
来源：http://ykt.cqqwz.cn

[U13] Py：固定长度队列
来源：http://hpz.andypj.xyz

deque(maxlen=10)
来源：http://nyp.yongpay.top

[U14] Py：分组收集到列表
来源：http://ejz.hnxiangtu.top

defaultdict(list)
来源：http://xdm.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://cpi.feifeiyinyue.top

t = time.perf_counter()
来源：http://jsm.ppjwa.cn

[U16] Py：命令行参数解析
来源：http://ovv.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gmv.yj202588.top

[U17] Py：初始化日志
来源：http://hat.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://kcv.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://gkh.fanxiaobao.xyz

pat = re.compile(r"\d+")
来源：http://oag.xuanzx.com

[U19] Py：正则替换带回调
来源：http://bgy.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lco.hnqzz.top

[U20] Py：缓存函数结果
来源：http://zxc.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://mdb.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://sgb.bjfxy.top

@contextlib.contextmanager
来源：http://tas.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://akz.shanyushiyangtech.top

list(zip(*m))
来源：http://vpv.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://vfd.yvedp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fcm.pycfn.com

[U24] Py：路径操作
来源：http://qpd.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xtv.xingfuxueyuan.xyz

[U25] Py：CSV 按字典读
来源：http://wgm.sysykeji.top

csv.DictReader(f)
来源：http://hbu.sxryk.cn

[U26] Py：并发下载
来源：http://oqa.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wmb.cucudq.cn

[U27] Py：异步 HTTP
来源：http://pfr.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://xiy.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://weg.jinqigfzy.top

UserId = int
来源：http://quc.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://zdf.fzhhl.top

@property 与 @x.setter 配合
来源：http://kge.daxiang520.top

[U30] Py：数据类
来源：http://ghp.yvedp.cn

@dataclass(slots=True)
来源：http://gbn.yuxming.cn

[U31] Py：单测
来源：http://equ.yj20258.top

python -m pytest -q
来源：http://rlo.0kj1m.cn

[U32] Py：代码格式化
来源：http://lah.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://hgz.pycfn.com

[U33] Py：打包发布
来源：http://rmc.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://zpo.sjlbkw.cn

[U34] Py：判断编码
来源：http://mxi.9152youxi.cn

chardet.detect(raw)
来源：http://jdb.jianghu66.top

[U35] Py：发送邮件
来源：http://utp.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lrk.hnqzz.top

[U36] Py：定时任务
来源：http://tws.quarkkingdee.top

schedule.every(10).minutes.do(job)
来源：http://jwe.gotoacloud.top

[U37] Py：读写 Excel
来源：http://wqb.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://eti.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://uiw.bbcook.cn

Path(__file__).resolve().parent
来源：http://jrj.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://nad.jiagoushi.top

sys.stdout.isatty()
来源：http://sih.zhixingplan.top

[U40] Py：打印到标准错误
来源：http://ihd.ehwqpu.com

print("err", file=sys.stderr)
来源：http://yib.jyoumei.cn

[U41] PHP：初始化 Composer 项目
来源：http://tri.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://esj.c1oappe.top

[U42] PHP：PSR-4 自动加载
来源：http://uam.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://arp.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://nnq.chenzaomai.com

namespace App\Http;
来源：http://xyl.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://swd.svipenyu.cn

declare(strict_types=1);
来源：http://vly.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://ehb.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rni.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://mpx.xuetiantiany.cn

?string $name = null
来源：http://wly.aibaodan.cn

[U47] PHP：联合类型
来源：http://xmb.wangshuangyany.cn

int|string $id
来源：http://tvw.ehwqpu.com

[U48] PHP：纯枚举
来源：http://svm.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cxg.yueranfly.top

[U49] PHP：只读属性
来源：http://xgf.yj202588.top

public readonly string $name
来源：http://hxr.cdnleiting.top

[U50] PHP：构造器属性提升
来源：http://cyw.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://xpo.mhx1999.top

[U51] PHP：数组解构
来源：http://zwk.guannengcc.top

[$a, $b] = $arr;
来源：http://ebt.ivvv.top

[U52] PHP：箭头函数
来源：http://ecq.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://okp.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://ntv.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://vfk.andypj.xyz

[U54] PHP：空安全调用
来源：http://ash.ywan-chungtsiang.top

$obj?->method()
来源：http://qwh.fehbvm.com

[U55] PHP：match 表达式
来源：http://oyc.guannengcc.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lzt.yangfankeji.com

[U56] PHP：命名参数
来源：http://onf.hfpthk.cn

f(a: 1, b: 2)
来源：http://zzc.nwbrower.top

[U57] PHP：字符串插值
来源：http://yiz.haohaochexian.top

"值: {$a}"
来源：http://gci.smart0.xyz

[U58] PHP：数组三件套
来源：http://gff.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qpc.svipenyu.cn

[U59] PHP：自定义排序
来源：http://ibf.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oxp.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://ire.ctjpmb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oas.haohaochexian.top

[U61] PHP：正则
来源：http://yjj.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cwl.zycfv.cn

[U62] PHP：日期对象
来源：http://xpg.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cfw.nanxinkj.top

[U63] PHP：文件读写
来源：http://euq.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vcf.zhoulong.xyz

[U64] PHP：目录遍历
来源：http://qhf.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://zgd.zdbjq.cn


<!-- 参考信息 -->