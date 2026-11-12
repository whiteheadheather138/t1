代发 wailian999

[S37] C++：set
来源：http://diu.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wps.yueranfly.top

[S38] C++：排序
来源：http://wvb.daxiang520.top

std::sort(v.begin(), v.end());
来源：http://qfq.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://nvq.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gru.nwbrower.top

[S40] C++：查找元素
来源：http://zfy.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cqh.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://jmt.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lay.smart0.xyz

[S42] C++：继承与虚函数
来源：http://ief.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://klu.hesvh.cn

[S43] C++：智能指针
来源：http://dso.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://jly.yfazqb.com

[S44] C++：引用传参
来源：http://exw.shuidangran.top

void inc(int &x) { ++x; }
来源：http://kfu.nanxuanxn.top

[S45] C++：lambda
来源：http://tja.zhengqikj.top

auto add = [](int a, int b) { return a + b; };
来源：http://gde.hysaishi.cn

[S46] C++：函数模板
来源：http://rcl.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://chy.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://ots.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bjn.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://gsy.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kby.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://abi.shangyingyoupin.top

[S49] C++：写文件
来源：http://myy.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lry.fehbvm.com

[S50] C++：格式化数字
来源：http://qgl.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://syq.zhengqikj.top

[S51] C++：显式类型转换
来源：http://dcl.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://nbq.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://fpy.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://oas.jyoumei.cn

[S53] C++：移动语义
来源：http://vfo.yj20258.top

std::vector<int> w = std::move(v);
来源：http://wvy.xuanzx.com

[S54] C++：异常处理
来源：http://oiu.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ofa.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://ubq.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mmb.wangdashe.top

[S56] C++：optional
来源：http://jvl.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wwf.yj20258888.top

[S57] C++：编译期常量
来源：http://rfi.ctjpmb.com

constexpr int N = 10;
来源：http://xyb.chenjidiqi.icu

[S58] C++：命名空间
来源：http://ucb.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://wgo.uphjek.com

[S59] C++：静态断言
来源：http://dtq.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zea.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://kve.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sdo.vehdjk.com

================================================================================
来源：http://zzy.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gni.yonumen.top

================================================================================
来源：http://ahj.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://zwy.bbcook.cn

println("Hello")
来源：http://rel.jyoumei.cn

[T02] Kotlin：变量
来源：http://tij.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xxt.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://qxz.hammf.cn

"值: $b"
来源：http://tqz.uphjek.com

[T04] Kotlin：空安全
来源：http://jch.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://daa.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://ych.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mgl.vehdjk.com

[T06] Kotlin：集合映射
来源：http://ctq.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://awg.sweek.top

[T07] Kotlin：集合过滤
来源：http://ntw.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://yxn.yuxming.cn

[T08] Kotlin：数据类
来源：http://fph.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://yuo.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://hrn.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://cke.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://fpn.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qro.xuetiantiany.cn

[T11] Kotlin：协程
来源：http://tjp.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wvz.yueranfly.top

[T12] Kotlin：解构声明
来源：http://png.tanke756.top

val (a, b) = Pair(1, 2)
来源：http://tdh.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://cqj.sweek.top

val m = mapOf("a" to 1)
来源：http://dzd.fktsv.cn

[T14] Kotlin：循环
来源：http://dip.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://ofv.cucudq.cn

[T15] Kotlin：接口
来源：http://igb.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://xuu.gaohongyu789.top

[T16] Swift：Hello World
来源：http://dur.jianghu66.top

print("Hello")
来源：http://dtt.hcnkem.com

[T17] Swift：变量与常量
来源：http://vbi.sweek.top

var a = 1;  let b = 2
来源：http://qfn.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://rwc.yongpay.top

"值: \(b)"
来源：http://dtj.zycfv.cn

[T19] Swift：可选绑定
来源：http://rmq.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://ggd.hesvh.cn

[T20] Swift：数组操作
来源：http://pia.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://pya.yuanzhike.top

[T21] Swift：遍历
来源：http://prg.tanke756.top

for x in a { print(x) }
来源：http://zbl.hnxiangtu.top

[T22] Swift：字典
来源：http://zbt.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://uuy.xinyue.icu

[T23] Swift：函数
来源：http://sua.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ukf.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://wrh.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://wpi.jqgfzy.top

[T25] Swift：结构体
来源：http://qlh.andypj.xyz

struct P { var x: Int }
来源：http://pvg.ppjwa.cn

[T26] Swift：类与重写
来源：http://enu.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://pqp.andypj.xyz

[T27] Swift：错误处理
来源：http://rxm.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://qyl.shzxlz.cn

[T28] Swift：枚举
来源：http://cue.jqgufenzy.top

enum Color { case red, green }
来源：http://ldi.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://kbu.jlsjyb.cn

guard let x = opt else { return }
来源：http://aby.nanxinkj.top

[T30] Swift：协议
来源：http://cyd.chenjidiqi.icu

protocol Shape { func area() -> Double }
来源：http://iaf.dashuyun.cn

[T31] Lua：Hello World
来源：http://rjg.jyoumei.cn

print("Hello")
来源：http://jih.jqgfzy.top

[T32] Lua：局部变量
来源：http://rjx.epnwcf.com

local a = 1
来源：http://luu.iojbl.cn

[T33] Lua：表（数组）
来源：http://ygs.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nnz.cqqwz.cn

[T34] Lua：遍历表
来源：http://svi.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vch.quarkkingdee.top

[T35] Lua：字典表
来源：http://ulj.zhijiandao.cn

local d = { a = 1 };  d.b = 2
来源：http://mfw.yj202588.top

[T36] Lua：函数
来源：http://ath.ydjk.org.cn

function add(a, b) return a + b end
来源：http://ptd.epnwcf.com

[T37] Lua：字符串拼接
来源：http://lzq.andypj.xyz

"a" .. "b"
来源：http://ukg.havefunace.top

[T38] Lua：条件
来源：http://jct.ppjwa.cn

if x > 0 then print("正") end
来源：http://vwg.yueranfly.top

[T39] Lua：模式匹配
来源：http://htv.zhiwuduotai.top

string.find(s, "%d+")
来源：http://pue.cheryme.top

[T40] Lua：元表
来源：http://cpk.shuidangran.top

setmetatable({}, { __index = base })
来源：http://jyl.zhaomingkeji.xyz

[T41] Perl：Hello World
来源：http://rpw.epnwcf.com

print "Hello\n";
来源：http://lfm.tarul.cn

[T42] Perl：变量类型
来源：http://fzd.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ogw.cdnleiting.top

[T43] Perl：字符串插值
来源：http://gxa.quarkkingdee.top

"值: $a"
来源：http://fre.chenlongwang.top

[T44] Perl：条件
来源：http://brv.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://ksd.cqqwz.cn

[T45] Perl：数组遍历
来源：http://zrt.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://rln.aibaodan.cn

[T46] Perl：哈希操作
来源：http://ngc.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fmu.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://qqp.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bqs.daria6918.cn

[T48] Perl：正则替换
来源：http://zui.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://ayr.jyoumei.cn

[T49] Perl：函数
来源：http://ioz.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rzg.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://kpb.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tst.havefunace.top

while (my $line = <$fh>) { print $line; }
来源：http://uau.ppjwa.cn

[T51] Scala：Hello World
来源：http://gcx.gzhubu.top

println("Hello")
来源：http://cjm.dashuyun.cn

[T52] Scala：变量
来源：http://hxv.ybcxt.top

val a = 1;  var b = 2
来源：http://sll.cdnleiting.top

[T53] Scala：字符串插值
来源：http://izq.c1oappe.top

s"值: $b"
来源：http://nnj.ctjpmb.com

[T54] Scala：集合映射
来源：http://tiz.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://hfs.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://rdd.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cch.redwolf501.top

[T56] Scala：样例类
来源：http://tvk.fehbvm.com

case class User(name: String, age: Int)
来源：http://mws.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://crd.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uag.vqdsnc.cn

[T58] Scala：函数定义
来源：http://tvn.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ugc.ehwqpu.com

[T59] Scala：循环
来源：http://okt.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://pfa.ehwqpu.com

[T60] Scala：折叠
来源：http://mlw.zdbjq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mvu.ydjk.org.cn

================================================================================
来源：http://omp.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gxt.ywan-chungtsiang.top

================================================================================
来源：http://sff.nanxinkj.top

[U01] Py：创建虚拟环境
来源：http://qkp.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://mld.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://qpn.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sln.yonumen.top

[U03] Py：加载 .env 配置
来源：http://hxb.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vfz.daria6918.cn

[U04] Py：变量调试打印
来源：http://jlk.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://len.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://pbi.pengpengdd.cyou

list(dict.fromkeys(arr))
来源：http://vkz.zhixingplan.top

[U06] Py：合并两个字典
来源：http://zzl.jlsjyb.cn

{**a, **b}
来源：http://xpy.wangdashe.top

[U07] Py：反转字典键值
来源：http://utm.hesvh.cn

{v: k for k, v in d.items()}
来源：http://bjt.jinqigufen.top

[U08] Py：展平二维列表
来源：http://szj.xinyue.icu

[y for x in nested for y in x]
来源：http://cmq.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://nst.zhijiandao.cn

max(d, key=d.get)
来源：http://tzc.9152youxi.cn

[U10] Py：按值排序字典
来源：http://pto.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iqo.ctjpmb.com

[U11] Py：生成器表达式
来源：http://msc.52xcode.cn

(x * 2 for x in arr)
来源：http://vds.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://nem.yuxming.cn

Counter(arr).most_common(3)
来源：http://mwd.yueranfly.top

[U13] Py：固定长度队列
来源：http://eaw.52xcode.cn

deque(maxlen=10)
来源：http://qte.pycfn.com

[U14] Py：分组收集到列表
来源：http://pyf.zhixingplan.top

defaultdict(list)
来源：http://jwy.yueranfly.top

[U15] Py：高精度计时
来源：http://izs.wangshuangyany.cn

t = time.perf_counter()
来源：http://wcz.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://pjx.ivvv.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lns.epnwcf.com

[U17] Py：初始化日志
来源：http://emb.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://elz.zhijiandao.cn

[U18] Py：预编译正则
来源：http://jvm.zycfv.cn

pat = re.compile(r"\d+")
来源：http://dba.daria6918.cn

[U19] Py：正则替换带回调
来源：http://aab.hnxiangtu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pxw.fktsv.cn

[U20] Py：缓存函数结果
来源：http://mbj.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://vwb.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://qvi.yj202588.top

@contextlib.contextmanager
来源：http://sge.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://zsn.andypj.xyz

list(zip(*m))
来源：http://see.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://mwo.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://syy.cucudq.cn

[U24] Py：路径操作
来源：http://tao.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://epi.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://kvx.tanke756.top

csv.DictReader(f)
来源：http://mvd.ybcxt.top

[U26] Py：并发下载
来源：http://fbo.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dxl.gzhubu.top

[U27] Py：异步 HTTP
来源：http://bqy.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://epl.yfazqb.com

[U28] Py：类型别名
来源：http://qdg.xylfe.cn

UserId = int
来源：http://cuy.guannengcc.top

[U29] Py：属性校验
来源：http://upa.mhx1999.top

@property 与 @x.setter 配合
来源：http://xmx.pycfn.com

[U30] Py：数据类
来源：http://run.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://haq.shangyingyoupin.top

[U31] Py：单测
来源：http://pcb.sysykeji.top

python -m pytest -q
来源：http://xgc.shzxlz.cn

[U32] Py：代码格式化
来源：http://drx.wangdashe.top

ruff format . && ruff check --fix .
来源：http://xxu.bbcook.cn

[U33] Py：打包发布
来源：http://dvj.gotoacloud.top

python -m build  （依赖 pyproject.toml）
来源：http://cvs.guannengcc.top

[U34] Py：判断编码
来源：http://ppr.yanxiufei.cn

chardet.detect(raw)
来源：http://xdn.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://knv.xylfe.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jyu.fktsv.cn

[U36] Py：定时任务
来源：http://hnp.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://ajn.sufxvd.cn

[U37] Py：读写 Excel
来源：http://ldl.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bke.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://kdg.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://nmn.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://udf.c1oappe.top

sys.stdout.isatty()
来源：http://tpg.xinyue.icu

[U40] Py：打印到标准错误
来源：http://eyh.epnwcf.com

print("err", file=sys.stderr)
来源：http://gbq.vehdjk.com

[U41] PHP：初始化 Composer 项目
来源：http://kjh.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nzz.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://rhx.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nhm.xziqi.cn

[U43] PHP：声明命名空间
来源：http://ujg.jinqigfzy.top

namespace App\Http;
来源：http://mjs.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://gnb.daria6918.cn

declare(strict_types=1);
来源：http://six.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://nhn.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zew.hesvh.cn

[U46] PHP：可空类型
来源：http://fmd.sysykeji.top

?string $name = null
来源：http://per.hesvh.cn

[U47] PHP：联合类型
来源：http://ivq.cheryme.top

int|string $id
来源：http://fbt.yangfankeji.com

[U48] PHP：纯枚举
来源：http://icf.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://skz.fehbvm.com

[U49] PHP：只读属性
来源：http://wgt.hysaishi.cn

public readonly string $name
来源：http://rxu.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://nzl.9152youxi.cn

public function __construct(private int $id) {}
来源：http://cwd.cheryme.top

[U51] PHP：数组解构
来源：http://wsm.pengpengdd.cyou

[$a, $b] = $arr;
来源：http://pgp.yj20258888.top

[U52] PHP：箭头函数
来源：http://hiu.ivvv.top

$double = fn($x) => $x * 2;
来源：http://wec.hesvh.cn

[U53] PHP：空合并运算符
来源：http://asx.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://yfn.aibaodan.cn

[U54] PHP：空安全调用
来源：http://qxo.fanxiaobao.xyz

$obj?->method()
来源：http://fjk.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://fwc.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ehz.jiagoushi.top

[U56] PHP：命名参数
来源：http://kqi.0kj1m.cn

f(a: 1, b: 2)
来源：http://ham.vqdsnc.cn

[U57] PHP：字符串插值
来源：http://oim.yanxiufei.cn

"值: {$a}"
来源：http://oje.yj20258.top

[U58] PHP：数组三件套
来源：http://anm.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rac.cucudq.cn

[U59] PHP：自定义排序
来源：http://uar.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xta.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://pzt.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cah.epnwcf.com

[U61] PHP：正则
来源：http://nww.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ffo.yuanzhike.top

[U62] PHP：日期对象
来源：http://xcv.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wjw.yj20258.top


<!-- 参考信息 -->