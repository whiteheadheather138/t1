代发 wailian999

[S39] C++：自定义比较器排序
来源：http://sgt.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kqb.hcnkem.com

[S40] C++：查找元素
来源：http://noz.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fqq.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://fsp.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vcr.9152youxi.cn

[S42] C++：继承与虚函数
来源：http://osx.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://yav.jiagoushi.top

[S43] C++：智能指针
来源：http://uhw.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://tyu.epnwcf.com

[S44] C++：引用传参
来源：http://iim.bbcook.cn

void inc(int &x) { ++x; }
来源：http://xmz.cashguo.top

[S45] C++：lambda
来源：http://hsu.tanke756.top

auto add = [](int a, int b) { return a + b; };
来源：http://bnx.cqqwz.cn

[S46] C++：函数模板
来源：http://lxx.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qrc.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://tqz.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mtq.zdbjq.cn

[S48] C++：逐行读文件
来源：http://dgz.xylfe.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zjv.shuidangran.top

while (std::getline(in, line)) { }
来源：http://ypl.gogol.net.cn

[S49] C++：写文件
来源：http://wpc.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hcg.kuanghao11.cn

[S50] C++：格式化数字
来源：http://avt.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tuh.52xcode.cn

[S51] C++：显式类型转换
来源：http://drn.zhixingplan.top

static_cast<double>(a) / b
来源：http://zme.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://org.ydjk.org.cn

int size() const noexcept { return n_; }
来源：http://eat.9152youxi.cn

[S53] C++：移动语义
来源：http://hxv.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://edz.svipenyu.cn

[S54] C++：异常处理
来源：http://xlh.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aiz.jianghu66.top

[S55] C++：结构化绑定
来源：http://ihe.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://cwq.yuxming.cn

[S56] C++：optional
来源：http://ftd.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mqi.gogol.net.cn

[S57] C++：编译期常量
来源：http://fnz.cheryme.top

constexpr int N = 10;
来源：http://bfz.ehwqpu.com

[S58] C++：命名空间
来源：http://gdk.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://kgj.snrcjt.cn

[S59] C++：静态断言
来源：http://sth.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tcd.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://jvd.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jbf.aibaodan.cn

================================================================================
来源：http://kfy.dianchejie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tfr.jiagoushi.top

================================================================================
来源：http://jda.pycfn.com

[T01] Kotlin：Hello World
来源：http://xox.wangdashe.top

println("Hello")
来源：http://bvw.daxiang520.top

[T02] Kotlin：变量
来源：http://sfp.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eap.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://tna.chenzaomai.com

"值: $b"
来源：http://hvz.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://nrq.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://mus.meibo888.top

[T05] Kotlin：when 表达式
来源：http://hxg.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hef.vehdjk.com

[T06] Kotlin：集合映射
来源：http://cqb.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sre.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://xaa.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://axq.fzhhl.top

[T08] Kotlin：数据类
来源：http://ccz.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://eaa.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://ata.yongpay.top

fun String.exclaim() = this + "!"
来源：http://oil.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://bae.shzxlz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lgs.zdbjq.cn

[T11] Kotlin：协程
来源：http://ire.52xcode.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cdz.ydzc1.top

[T12] Kotlin：解构声明
来源：http://afb.gogol.net.cn

val (a, b) = Pair(1, 2)
来源：http://gbc.yj202588.top

[T13] Kotlin：只读 Map
来源：http://qeb.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://fen.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://sgn.daxiang520.top

for (i in 1..10) println(i)
来源：http://cya.xziqi.cn

[T15] Kotlin：接口
来源：http://lwt.guowangkeji.top

interface Shape { fun area(): Double }
来源：http://bih.ydjk.org.cn

[T16] Swift：Hello World
来源：http://zyv.chenlongwang.top

print("Hello")
来源：http://amq.meibo888.top

[T17] Swift：变量与常量
来源：http://zcd.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://ucy.yj20258.top

[T18] Swift：字符串插值
来源：http://gke.havefunace.top

"值: \(b)"
来源：http://jiz.hywenlv.cn

[T19] Swift：可选绑定
来源：http://feq.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://you.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://bro.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://vjo.dianchejie.cn

[T21] Swift：遍历
来源：http://uwo.haohaochexian.top

for x in a { print(x) }
来源：http://qqy.tarul.cn

[T22] Swift：字典
来源：http://hal.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://wzq.yanxiufei.cn

[T23] Swift：函数
来源：http://mmp.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kjk.svipenyu.cn

[T24] Swift：闭包
来源：http://fbk.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ucr.chenzaomai.com

[T25] Swift：结构体
来源：http://krb.hongshengwenyu.top

struct P { var x: Int }
来源：http://rzh.bbcook.cn

[T26] Swift：类与重写
来源：http://ave.52xcode.cn

class A: Base { override func f() {} }
来源：http://pxp.xylfe.cn

[T27] Swift：错误处理
来源：http://hbd.52xcode.cn

do { try f() } catch { print(error) }
来源：http://roc.vqdsnc.cn

[T28] Swift：枚举
来源：http://aoe.xziqi.cn

enum Color { case red, green }
来源：http://fdc.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://laj.hcnkem.com

guard let x = opt else { return }
来源：http://bsa.vehdjk.com

[T30] Swift：协议
来源：http://xvw.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://lxw.cdnleiting.top

[T31] Lua：Hello World
来源：http://xsg.birdmap.top

print("Hello")
来源：http://ozv.xinyue.icu

[T32] Lua：局部变量
来源：http://ilu.zdqjudy.top

local a = 1
来源：http://dsw.jiagoushi.top

[T33] Lua：表（数组）
来源：http://vof.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pyr.zhengqikj.top

[T34] Lua：遍历表
来源：http://yau.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hdq.tian-w.cn

[T35] Lua：字典表
来源：http://wnj.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://htw.316326.xyz

[T36] Lua：函数
来源：http://gbq.jinyuanbaomall.cn

function add(a, b) return a + b end
来源：http://hen.sxryk.cn

[T37] Lua：字符串拼接
来源：http://dpa.cheryme.top

"a" .. "b"
来源：http://ept.daxiang520.top

[T38] Lua：条件
来源：http://aje.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://rfm.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://gcj.yonumen.top

string.find(s, "%d+")
来源：http://pkn.smart0.xyz

[T40] Lua：元表
来源：http://wpm.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://ezm.zhijiandao.cn

[T41] Perl：Hello World
来源：http://ykm.zycfv.cn

print "Hello\n";
来源：http://eje.xylfe.cn

[T42] Perl：变量类型
来源：http://okv.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dsi.snrcjt.cn

[T43] Perl：字符串插值
来源：http://dge.fanxiaobao.xyz

"值: $a"
来源：http://asr.fktsv.cn

[T44] Perl：条件
来源：http://zgl.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://pwf.ehwqpu.com

[T45] Perl：数组遍历
来源：http://qof.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://axr.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://mco.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://swh.ctjpmb.com

[T47] Perl：正则捕获
来源：http://tvo.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gaa.dianchejie.cn

[T48] Perl：正则替换
来源：http://dzm.guannengcc.top

$s =~ s/old/new/g;
来源：http://zmp.zhijiandao.cn

[T49] Perl：函数
来源：http://aay.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nyp.cheryme.top

[T50] Perl：逐行读文件
来源：http://vcv.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dth.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://jkf.cdnleiting.top

[T51] Scala：Hello World
来源：http://zhr.wangshuangyany.cn

println("Hello")
来源：http://lhz.zycfv.cn

[T52] Scala：变量
来源：http://nva.svipenyu.cn

val a = 1;  var b = 2
来源：http://jve.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://dua.gaohongyu789.top

s"值: $b"
来源：http://vhz.gaohongyu789.top

[T54] Scala：集合映射
来源：http://dvm.cheryme.top

List(1, 2, 3).map(_ * 2)
来源：http://vkf.hnqzz.top

[T55] Scala：集合过滤
来源：http://qrq.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://umj.shzxlz.cn

[T56] Scala：样例类
来源：http://lrv.jyoumei.cn

case class User(name: String, age: Int)
来源：http://ary.zhiwuduotai.top

[T57] Scala：模式匹配
来源：http://xvl.jqgfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://isg.hesvh.cn

[T58] Scala：函数定义
来源：http://fke.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ooc.yj202588.top

[T59] Scala：循环
来源：http://xfw.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://fqi.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://uud.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pro.aizwys.cn

================================================================================
来源：http://byi.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://elf.tian-w.cn

================================================================================
来源：http://kak.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://ekj.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://rvb.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://tme.meibo888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vpo.meibo888.top

[U03] Py：加载 .env 配置
来源：http://ozf.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://omw.daria6918.cn

[U04] Py：变量调试打印
来源：http://ryw.redwolf501.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pks.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://var.redwolf501.top

list(dict.fromkeys(arr))
来源：http://lmw.dianchejie.cn

[U06] Py：合并两个字典
来源：http://nem.hcnkem.com

{**a, **b}
来源：http://ekv.vehdjk.com

[U07] Py：反转字典键值
来源：http://tzj.fehbvm.com

{v: k for k, v in d.items()}
来源：http://qlj.yuanzhike.top

[U08] Py：展平二维列表
来源：http://zqj.yueranfly.top

[y for x in nested for y in x]
来源：http://yqw.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://okh.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://zpa.zhixingplan.top

[U10] Py：按值排序字典
来源：http://ohr.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ohv.bbcook.cn

[U11] Py：生成器表达式
来源：http://mdh.yueranfly.top

(x * 2 for x in arr)
来源：http://mrp.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pal.hysaishi.cn

Counter(arr).most_common(3)
来源：http://dus.jiagoushi.top

[U13] Py：固定长度队列
来源：http://fmv.yj202588.top

deque(maxlen=10)
来源：http://gmq.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://nvq.iojbl.cn

defaultdict(list)
来源：http://xbt.birdmap.top

[U15] Py：高精度计时
来源：http://syh.zdbjq.cn

t = time.perf_counter()
来源：http://syw.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://apt.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hry.tian-w.cn

[U17] Py：初始化日志
来源：http://wks.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ydw.sjlbkw.cn

[U18] Py：预编译正则
来源：http://qnd.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://efj.yvedp.cn

[U19] Py：正则替换带回调
来源：http://eiy.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bgy.redwolf501.top

[U20] Py：缓存函数结果
来源：http://sim.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://slj.hongshengwenyu.top

[U21] Py：自定义上下文管理器
来源：http://vxh.yueranfly.top

@contextlib.contextmanager
来源：http://wix.yonumen.top

[U22] Py：矩阵转置
来源：http://ycr.gaohongyu789.top

list(zip(*m))
来源：http://hxd.52xcode.cn

[U23] Py：分块读取大文件
来源：http://diu.ywan-chungtsiang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://euw.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://raw.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://slu.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://fyg.tianlin.xyz

csv.DictReader(f)
来源：http://fap.jinghuilouyu.cn

[U26] Py：并发下载
来源：http://vgu.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dou.yfazqb.com

[U27] Py：异步 HTTP
来源：http://ckw.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://wvb.zhengqikj.top

[U28] Py：类型别名
来源：http://xfn.chenjidiqi.icu

UserId = int
来源：http://qae.bbcook.cn

[U29] Py：属性校验
来源：http://sla.yueranfly.top

@property 与 @x.setter 配合
来源：http://htz.shzxlz.cn

[U30] Py：数据类
来源：http://nqi.xingfuxueyuan.xyz

@dataclass(slots=True)
来源：http://mqq.cashguo.top

[U31] Py：单测
来源：http://iqc.bbcook.cn

python -m pytest -q
来源：http://wyh.zdqjudy.top

[U32] Py：代码格式化
来源：http://tzb.meibo888.top

ruff format . && ruff check --fix .
来源：http://oxk.birdmap.top

[U33] Py：打包发布
来源：http://dma.zhongyouzk.top

python -m build  （依赖 pyproject.toml）
来源：http://wsz.sjlbkw.cn

[U34] Py：判断编码
来源：http://ftn.wangshuangyany.cn

chardet.detect(raw)
来源：http://yjn.nwbrower.top

[U35] Py：发送邮件
来源：http://cmi.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wlf.epnwcf.com

[U36] Py：定时任务
来源：http://ztv.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://czt.nwbrower.top

[U37] Py：读写 Excel
来源：http://duq.yj20258888.top

pandas.read_excel / DataFrame.to_excel
来源：http://wps.jinghuilouyu.cn

[U38] Py：获取脚本所在目录
来源：http://rpp.fzhhl.top

Path(__file__).resolve().parent
来源：http://ssa.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://loe.cqqwz.cn

sys.stdout.isatty()
来源：http://yxe.meibo888.top

[U40] Py：打印到标准错误
来源：http://jpn.cdnleiting.top

print("err", file=sys.stderr)
来源：http://jyi.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://kwa.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://atc.xingfuxueyuan.xyz

[U42] PHP：PSR-4 自动加载
来源：http://kjh.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://htp.zhoulong.xyz

[U43] PHP：声明命名空间
来源：http://plz.hywenlv.cn

namespace App\Http;
来源：http://hxo.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://zjv.tanke756.top

declare(strict_types=1);
来源：http://vmd.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://mcr.meibo888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://unr.gaohongyu789.top

[U46] PHP：可空类型
来源：http://tih.yvedp.cn

?string $name = null
来源：http://usw.ctjpmb.com

[U47] PHP：联合类型
来源：http://uas.hywenlv.cn

int|string $id
来源：http://qwf.yvedp.cn

[U48] PHP：纯枚举
来源：http://wnt.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tmu.mhx1999.top

[U49] PHP：只读属性
来源：http://hcw.nwbrower.top

public readonly string $name
来源：http://kwj.pycfn.com

[U50] PHP：构造器属性提升
来源：http://kzg.ybcxt.top

public function __construct(private int $id) {}
来源：http://odh.yj202588.top

[U51] PHP：数组解构
来源：http://fzm.iojbl.cn

[$a, $b] = $arr;
来源：http://vgi.9152youxi.cn

[U52] PHP：箭头函数
来源：http://phg.gotoacloud.top

$double = fn($x) => $x * 2;
来源：http://evb.bjfxy.top

[U53] PHP：空合并运算符
来源：http://dyx.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://akg.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://xly.fktsv.cn

$obj?->method()
来源：http://zfo.zhoulong.xyz

[U55] PHP：match 表达式
来源：http://klo.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sdt.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://ypx.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://ruj.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://lvy.gaohongyu789.top

"值: {$a}"
来源：http://yjy.fktsv.cn

[U58] PHP：数组三件套
来源：http://zsc.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gkm.dianchejie.cn

[U59] PHP：自定义排序
来源：http://bmg.zhixingplan.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xcg.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://wfz.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lym.52xcode.cn

[U61] PHP：正则
来源：http://hag.chenlongwang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bgj.svipenyu.cn

[U62] PHP：日期对象
来源：http://rau.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vhu.smart0.xyz

[U63] PHP：文件读写
来源：http://qds.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ngm.cqqwz.cn

[U64] PHP：目录遍历
来源：http://pdu.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://cen.ehwqpu.com


<!-- 参考信息 -->