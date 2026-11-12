代发 wailian999

[S39] C++：自定义比较器排序
来源：http://bpk.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sca.jqgufenzy.top

[S40] C++：查找元素
来源：http://bkx.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rpt.havefunace.top

[S41] C++：类与构造函数
来源：http://ryu.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kpz.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://olx.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://tzm.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://keu.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://twx.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://oah.cheryme.top

void inc(int &x) { ++x; }
来源：http://gta.fengsongda.top

[S45] C++：lambda
来源：http://ztv.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rtl.hnxiangtu.top

[S46] C++：函数模板
来源：http://pek.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://brl.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://bqs.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://flp.hfpthk.cn

[S48] C++：逐行读文件
来源：http://tod.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://dmx.daxiang520.top

while (std::getline(in, line)) { }
来源：http://fxx.dashuyun.cn

[S49] C++：写文件
来源：http://qjk.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mhn.dashuyun.cn

[S50] C++：格式化数字
来源：http://yjq.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ndo.yj202588.top

[S51] C++：显式类型转换
来源：http://zee.haohaochexian.top

static_cast<double>(a) / b
来源：http://onp.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://lqk.meibo888.top

int size() const noexcept { return n_; }
来源：http://wuv.52xcode.cn

[S53] C++：移动语义
来源：http://pux.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://eqx.0kj1m.cn

[S54] C++：异常处理
来源：http://gsh.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pvc.zhixingplan.top

[S55] C++：结构化绑定
来源：http://iij.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tin.zhijiandao.cn

[S56] C++：optional
来源：http://aui.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nvh.bbcook.cn

[S57] C++：编译期常量
来源：http://bww.haohaochexian.top

constexpr int N = 10;
来源：http://uec.aibaodan.cn

[S58] C++：命名空间
来源：http://ipz.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://dkv.zhengqikj.top

[S59] C++：静态断言
来源：http://jii.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qam.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://zss.hcnkem.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://slz.wangdashe.top

================================================================================
来源：http://yze.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://krf.jinyuanbaomall.cn

================================================================================
来源：http://heh.52xcode.cn

[T01] Kotlin：Hello World
来源：http://gyl.316326.xyz

println("Hello")
来源：http://dsf.zhengqikj.top

[T02] Kotlin：变量
来源：http://zlm.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vhs.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://zun.zhoulong.xyz

"值: $b"
来源：http://yde.ppjwa.cn

[T04] Kotlin：空安全
来源：http://kbq.aibaodan.cn

val n: String? = null;  n?.length
来源：http://ehl.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://zft.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zgp.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://mxn.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://afu.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://rci.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://anz.sysykeji.top

[T08] Kotlin：数据类
来源：http://cmy.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://fpb.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://msh.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://vwz.yj202588.top

[T10] Kotlin：默认参数
来源：http://eag.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iqo.yfazqb.com

[T11] Kotlin：协程
来源：http://tqz.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gnk.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://zrm.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://rjk.nanxinkj.top

[T13] Kotlin：只读 Map
来源：http://ooy.daria6918.cn

val m = mapOf("a" to 1)
来源：http://duo.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://zkr.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://jos.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://zue.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://qcc.jlsjyb.cn

[T16] Swift：Hello World
来源：http://vzq.zdbjq.cn

print("Hello")
来源：http://jcj.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://shp.daria6918.cn

var a = 1;  let b = 2
来源：http://lgo.svipenyu.cn

[T18] Swift：字符串插值
来源：http://nto.yangfankeji.com

"值: \(b)"
来源：http://mcp.zhixingplan.top

[T19] Swift：可选绑定
来源：http://ycl.gogol.net.cn

if let n = opt { print(n) }
来源：http://xeu.haohaochexian.top

[T20] Swift：数组操作
来源：http://crq.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pqd.jyoumei.cn

[T21] Swift：遍历
来源：http://vpd.tarul.cn

for x in a { print(x) }
来源：http://vwp.gaohongyu789.top

[T22] Swift：字典
来源：http://mfj.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://suh.gzhubu.top

[T23] Swift：函数
来源：http://myj.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qhk.jianghu66.top

[T24] Swift：闭包
来源：http://usn.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ddz.gotoacloud.top

[T25] Swift：结构体
来源：http://dzq.bjfxy.top

struct P { var x: Int }
来源：http://rzf.birdmap.top

[T26] Swift：类与重写
来源：http://ejv.pengpengdd.cyou

class A: Base { override func f() {} }
来源：http://vzw.yueranfly.top

[T27] Swift：错误处理
来源：http://hsw.daxiang520.top

do { try f() } catch { print(error) }
来源：http://hnn.jinqigfzy.top

[T28] Swift：枚举
来源：http://qre.sjlbkw.cn

enum Color { case red, green }
来源：http://dxk.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://ele.shuidangran.top

guard let x = opt else { return }
来源：http://foi.shuidangran.top

[T30] Swift：协议
来源：http://aps.gogol.net.cn

protocol Shape { func area() -> Double }
来源：http://fic.ydzc1.top

[T31] Lua：Hello World
来源：http://kqy.meibo888.top

print("Hello")
来源：http://yjx.dianchejie.cn

[T32] Lua：局部变量
来源：http://zrm.sxryk.cn

local a = 1
来源：http://xax.gogol.net.cn

[T33] Lua：表（数组）
来源：http://oxe.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://dhr.yj20258888.top

[T34] Lua：遍历表
来源：http://upk.sysykeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qlp.daxiang520.top

[T35] Lua：字典表
来源：http://nev.hfpthk.cn

local d = { a = 1 };  d.b = 2
来源：http://ghv.yongpay.top

[T36] Lua：函数
来源：http://qvh.yj20258.top

function add(a, b) return a + b end
来源：http://vci.hesvh.cn

[T37] Lua：字符串拼接
来源：http://kuh.gaohongyu789.top

"a" .. "b"
来源：http://ebl.nanxuanxn.top

[T38] Lua：条件
来源：http://nkt.ctjpmb.com

if x > 0 then print("正") end
来源：http://rzo.xuanzx.com

[T39] Lua：模式匹配
来源：http://par.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://eta.yj202588.top

[T40] Lua：元表
来源：http://uvs.kuanghao11.cn

setmetatable({}, { __index = base })
来源：http://hfd.ydjk.org.cn

[T41] Perl：Hello World
来源：http://fjh.cheryme.top

print "Hello\n";
来源：http://coj.hfpthk.cn

[T42] Perl：变量类型
来源：http://wlp.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blq.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://lhj.jianghu66.top

"值: $a"
来源：http://qji.hfpthk.cn

[T44] Perl：条件
来源：http://wcb.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://bdl.xziqi.cn

[T45] Perl：数组遍历
来源：http://twr.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://pyy.9152youxi.cn

[T46] Perl：哈希操作
来源：http://kir.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dbl.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://qtg.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://sda.shzxlz.cn

[T48] Perl：正则替换
来源：http://qyf.gogol.net.cn

$s =~ s/old/new/g;
来源：http://pvm.hysaishi.cn

[T49] Perl：函数
来源：http://bel.yonumen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lka.daxiang520.top

[T50] Perl：逐行读文件
来源：http://ajy.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://tgj.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://bvp.yvedp.cn

[T51] Scala：Hello World
来源：http://zne.vehdjk.com

println("Hello")
来源：http://ktc.wangdashe.top

[T52] Scala：变量
来源：http://psp.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://kkx.316326.xyz

[T53] Scala：字符串插值
来源：http://xzy.chenzaomai.com

s"值: $b"
来源：http://joc.jianghu66.top

[T54] Scala：集合映射
来源：http://qqm.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://sdl.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://jju.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vwl.sweek.top

[T56] Scala：样例类
来源：http://lvw.bjfxy.top

case class User(name: String, age: Int)
来源：http://nub.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://fpt.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gsi.gotoacloud.top

[T58] Scala：函数定义
来源：http://pux.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rse.hesvh.cn

[T59] Scala：循环
来源：http://vyl.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://qbh.tianlin.xyz

[T60] Scala：折叠
来源：http://yab.c1oappe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rqq.aibaodan.cn

================================================================================
来源：http://lvq.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yzl.snrcjt.cn

================================================================================
来源：http://ywc.zhengqikj.top

[U01] Py：创建虚拟环境
来源：http://qpb.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://buo.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://ihs.hammf.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qvh.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://mtb.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rrm.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://pup.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mgi.hammf.cn

[U05] Py：列表去重且保序
来源：http://uzc.yj20258888.top

list(dict.fromkeys(arr))
来源：http://osi.ybcxt.top

[U06] Py：合并两个字典
来源：http://iev.zdbjq.cn

{**a, **b}
来源：http://dkn.nwbrower.top

[U07] Py：反转字典键值
来源：http://zdk.fehbvm.com

{v: k for k, v in d.items()}
来源：http://tdl.daria6918.cn

[U08] Py：展平二维列表
来源：http://gfw.gaohongyu789.top

[y for x in nested for y in x]
来源：http://gcf.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://pzz.bjfxy.top

max(d, key=d.get)
来源：http://jym.tian-w.cn

[U10] Py：按值排序字典
来源：http://axm.xuanzx.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cjt.yongpay.top

[U11] Py：生成器表达式
来源：http://bvw.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://gfj.fengsongda.top

[U12] Py：取出现最多的 3 个元素
来源：http://wkh.yj20258888.top

Counter(arr).most_common(3)
来源：http://zzg.birdmap.top

[U13] Py：固定长度队列
来源：http://efg.hammf.cn

deque(maxlen=10)
来源：http://pxy.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://uvi.jinyuanbaomall.cn

defaultdict(list)
来源：http://okn.jianghu66.top

[U15] Py：高精度计时
来源：http://vln.jinqigfzy.top

t = time.perf_counter()
来源：http://vra.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://sva.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rnr.wangshuangyany.cn

[U17] Py：初始化日志
来源：http://igh.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://uqb.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://scr.yfazqb.com

pat = re.compile(r"\d+")
来源：http://kyr.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://lfu.vqdsnc.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ggj.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://qje.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://spk.meibo888.top

[U21] Py：自定义上下文管理器
来源：http://tod.yuxming.cn

@contextlib.contextmanager
来源：http://psn.yj202588.top

[U22] Py：矩阵转置
来源：http://wkg.nwbrower.top

list(zip(*m))
来源：http://rio.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://sst.ydjk.org.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hqd.ydjk.org.cn

[U24] Py：路径操作
来源：http://cig.gotoacloud.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wpo.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://zsg.cdnleiting.top

csv.DictReader(f)
来源：http://kkg.yanxiufei.cn

[U26] Py：并发下载
来源：http://uzd.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xkd.sufxvd.cn

[U27] Py：异步 HTTP
来源：http://pur.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://esf.hywenlv.cn

[U28] Py：类型别名
来源：http://gtd.aizwys.cn

UserId = int
来源：http://fve.hywenlv.cn

[U29] Py：属性校验
来源：http://yfe.hammf.cn

@property 与 @x.setter 配合
来源：http://zty.0kj1m.cn

[U30] Py：数据类
来源：http://frh.nwbrower.top

@dataclass(slots=True)
来源：http://kpm.gaohongyu789.top

[U31] Py：单测
来源：http://xmn.svipenyu.cn

python -m pytest -q
来源：http://emt.chenzaomai.com

[U32] Py：代码格式化
来源：http://dgy.yangfankeji.com

ruff format . && ruff check --fix .
来源：http://rja.ydjk.org.cn

[U33] Py：打包发布
来源：http://xpa.meibo888.top

python -m build  （依赖 pyproject.toml）
来源：http://xid.feifeiyinyue.top

[U34] Py：判断编码
来源：http://cqh.yj20258888.top

chardet.detect(raw)
来源：http://dtp.52xcode.cn

[U35] Py：发送邮件
来源：http://kjy.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dmw.yanxiufei.cn

[U36] Py：定时任务
来源：http://rhc.fanxiaobao.xyz

schedule.every(10).minutes.do(job)
来源：http://vwu.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://nxj.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://dsu.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://ymv.xziqi.cn

Path(__file__).resolve().parent
来源：http://oqn.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://rwr.vehdjk.com

sys.stdout.isatty()
来源：http://pln.hnqzz.top

[U40] Py：打印到标准错误
来源：http://qpu.hongshengwenyu.top

print("err", file=sys.stderr)
来源：http://rxr.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://rwe.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lix.sxryk.cn

[U42] PHP：PSR-4 自动加载
来源：http://ibi.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kob.cashguo.top

[U43] PHP：声明命名空间
来源：http://ijt.daxiang520.top

namespace App\Http;
来源：http://jzf.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://tii.dashuyun.cn

declare(strict_types=1);
来源：http://cvc.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://pqs.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gqz.zhixingplan.top

[U46] PHP：可空类型
来源：http://wvc.nanxuanxn.top

?string $name = null
来源：http://axv.ppjwa.cn

[U47] PHP：联合类型
来源：http://bgv.sysykeji.top

int|string $id
来源：http://fwg.cqqwz.cn

[U48] PHP：纯枚举
来源：http://ncu.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ygh.bbcook.cn

[U49] PHP：只读属性
来源：http://eun.xylfe.cn

public readonly string $name
来源：http://ujq.ivvv.top

[U50] PHP：构造器属性提升
来源：http://xdf.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://rnx.daria6918.cn

[U51] PHP：数组解构
来源：http://sod.daxiang520.top

[$a, $b] = $arr;
来源：http://kmf.wangdashe.top

[U52] PHP：箭头函数
来源：http://nat.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://zyh.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://uly.hfpthk.cn

$v = $a ?? $b ?? "default";
来源：http://ozr.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://bgt.sysykeji.top

$obj?->method()
来源：http://swx.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://odm.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sis.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://egd.feifeiyinyue.top

f(a: 1, b: 2)
来源：http://kyd.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://rto.mhx1999.top

"值: {$a}"
来源：http://kli.ydzc1.top

[U58] PHP：数组三件套
来源：http://gly.cheryme.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qeo.cheryme.top

[U59] PHP：自定义排序
来源：http://hwy.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://owk.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://uhk.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gfy.hnqzz.top

[U61] PHP：正则
来源：http://rzb.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hvb.nanxinkj.top

[U62] PHP：日期对象
来源：http://oto.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fbr.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://xyf.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yxb.zycfv.cn

[U64] PHP：目录遍历
来源：http://ypf.ywan-chungtsiang.top

glob("dir/*.php");  scandir("dir");
来源：http://uub.yanxiufei.cn


<!-- 参考信息 -->