代发 wailian999

[S43] C++：智能指针
来源：http://yfg.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://tuo.shuidangran.top

[S44] C++：引用传参
来源：http://vzm.yvedp.cn

void inc(int &x) { ++x; }
来源：http://kpq.sjlbkw.cn

[S45] C++：lambda
来源：http://egr.zycfv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oxb.yuxming.cn

[S46] C++：函数模板
来源：http://zed.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dli.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://nec.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://llg.yvedp.cn

[S48] C++：逐行读文件
来源：http://lck.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://nhx.mhx1999.top

while (std::getline(in, line)) { }
来源：http://hkr.xylfe.cn

[S49] C++：写文件
来源：http://qez.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ery.jinghuilouyu.cn

[S50] C++：格式化数字
来源：http://gfa.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jor.yonumen.top

[S51] C++：显式类型转换
来源：http://pzw.ydzc1.top

static_cast<double>(a) / b
来源：http://lwd.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://xxh.daria6918.cn

int size() const noexcept { return n_; }
来源：http://zgw.wangshuangyany.cn

[S53] C++：移动语义
来源：http://fxp.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://njv.hcnkem.com

[S54] C++：异常处理
来源：http://bcu.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://boe.cqqwz.cn

[S55] C++：结构化绑定
来源：http://abd.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://bnm.pengpengdd.cyou

[S56] C++：optional
来源：http://rpq.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pdb.smart0.xyz

[S57] C++：编译期常量
来源：http://bnd.gogol.net.cn

constexpr int N = 10;
来源：http://clf.meibo888.top

[S58] C++：命名空间
来源：http://gju.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://yfh.jqgufenzy.top

[S59] C++：静态断言
来源：http://ixe.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oqs.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://maz.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://goq.yonumen.top

================================================================================
来源：http://jks.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hni.ppjwa.cn

================================================================================
来源：http://pno.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://jvg.yuxming.cn

println("Hello")
来源：http://cjx.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://huc.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ive.yonumen.top

[T03] Kotlin：字符串模板
来源：http://syk.cdnleiting.top

"值: $b"
来源：http://hzj.birdmap.top

[T04] Kotlin：空安全
来源：http://ycy.zdbjq.cn

val n: String? = null;  n?.length
来源：http://yka.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://oal.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nld.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://lkr.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vrk.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://kbb.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://mwf.iojbl.cn

[T08] Kotlin：数据类
来源：http://rwx.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://fwr.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://nmm.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://hth.yfazqb.com

[T10] Kotlin：默认参数
来源：http://trn.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hbi.ctjpmb.com

[T11] Kotlin：协程
来源：http://ggm.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ocl.nanxuanxn.top

[T12] Kotlin：解构声明
来源：http://xva.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://bba.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://qeq.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://hxi.nwbrower.top

[T14] Kotlin：循环
来源：http://nxz.zycfv.cn

for (i in 1..10) println(i)
来源：http://sry.yuxming.cn

[T15] Kotlin：接口
来源：http://boz.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://uym.hfpthk.cn

[T16] Swift：Hello World
来源：http://zfu.zhixingplan.top

print("Hello")
来源：http://nwr.jqgfzy.top

[T17] Swift：变量与常量
来源：http://xwl.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://kup.sufxvd.cn

[T18] Swift：字符串插值
来源：http://yua.chenzaomai.com

"值: \(b)"
来源：http://obx.xinyue.icu

[T19] Swift：可选绑定
来源：http://esf.nwbrower.top

if let n = opt { print(n) }
来源：http://tlq.birdmap.top

[T20] Swift：数组操作
来源：http://kpm.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://tyb.bjfxy.top

[T21] Swift：遍历
来源：http://tsw.jlsjyb.cn

for x in a { print(x) }
来源：http://vjc.chenlongwang.top

[T22] Swift：字典
来源：http://bme.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://xux.xziqi.cn

[T23] Swift：函数
来源：http://ftv.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xfp.cdnleiting.top

[T24] Swift：闭包
来源：http://syf.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gmp.sufxvd.cn

[T25] Swift：结构体
来源：http://qud.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://cce.zhengqikj.top

[T26] Swift：类与重写
来源：http://upn.yj20258888.top

class A: Base { override func f() {} }
来源：http://dps.hnqzz.top

[T27] Swift：错误处理
来源：http://gmq.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://vsz.xylfe.cn

[T28] Swift：枚举
来源：http://rjx.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://yqk.cashguo.top

[T29] Swift：guard 提前返回
来源：http://crl.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://jeg.ydjk.org.cn

[T30] Swift：协议
来源：http://wsx.chenjidiqi.icu

protocol Shape { func area() -> Double }
来源：http://saa.zycfv.cn

[T31] Lua：Hello World
来源：http://xmg.fktsv.cn

print("Hello")
来源：http://vto.yuanzhike.top

[T32] Lua：局部变量
来源：http://jxu.hcnkem.com

local a = 1
来源：http://fzz.uphjek.com

[T33] Lua：表（数组）
来源：http://dxn.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bjc.yuanzhike.top

[T34] Lua：遍历表
来源：http://atp.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vqs.0kj1m.cn

[T35] Lua：字典表
来源：http://blf.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://izs.aizwys.cn

[T36] Lua：函数
来源：http://hfg.hysaishi.cn

function add(a, b) return a + b end
来源：http://izk.yueranfly.top

[T37] Lua：字符串拼接
来源：http://twh.gaohongyu789.top

"a" .. "b"
来源：http://apo.yangfankeji.com

[T38] Lua：条件
来源：http://baj.pycfn.com

if x > 0 then print("正") end
来源：http://qxd.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://rew.yongpay.top

string.find(s, "%d+")
来源：http://nic.smart0.xyz

[T40] Lua：元表
来源：http://ihm.ydzc1.top

setmetatable({}, { __index = base })
来源：http://kqt.cashguo.top

[T41] Perl：Hello World
来源：http://uzk.hongshengwenyu.top

print "Hello\n";
来源：http://qcl.iojbl.cn

[T42] Perl：变量类型
来源：http://fev.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hdv.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://akf.zdbjq.cn

"值: $a"
来源：http://mve.jiagoushi.top

[T44] Perl：条件
来源：http://abt.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://eph.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://led.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://esr.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://kzi.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xsc.shzxlz.cn

[T47] Perl：正则捕获
来源：http://inb.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://uuh.smart0.xyz

[T48] Perl：正则替换
来源：http://odp.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://zqd.tianlin.xyz

[T49] Perl：函数
来源：http://myi.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lrp.tanke756.top

[T50] Perl：逐行读文件
来源：http://sga.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ykj.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://yvb.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://xwv.wangdashe.top

println("Hello")
来源：http://vak.iojbl.cn

[T52] Scala：变量
来源：http://fec.yueranfly.top

val a = 1;  var b = 2
来源：http://far.smart0.xyz

[T53] Scala：字符串插值
来源：http://flf.ivvv.top

s"值: $b"
来源：http://irr.cucudq.cn

[T54] Scala：集合映射
来源：http://lta.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://rpp.tarul.cn

[T55] Scala：集合过滤
来源：http://fsy.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://uvw.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://szi.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://ikz.epnwcf.com

[T57] Scala：模式匹配
来源：http://cns.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://kxf.shuidangran.top

[T58] Scala：函数定义
来源：http://juf.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pfk.hongshengwenyu.top

[T59] Scala：循环
来源：http://mkr.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://apg.sjlbkw.cn

[T60] Scala：折叠
来源：http://pyt.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jds.aibaodan.cn

================================================================================
来源：http://tex.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fnh.tian-w.cn

================================================================================
来源：http://tti.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://hac.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://zgi.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://uhs.xziqi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://osc.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://bdx.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://nzd.iojbl.cn

[U04] Py：变量调试打印
来源：http://kpo.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ekf.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://ake.wangdashe.top

list(dict.fromkeys(arr))
来源：http://jrt.fktsv.cn

[U06] Py：合并两个字典
来源：http://ojo.chenlongwang.top

{**a, **b}
来源：http://sry.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://tzd.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://mdx.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://ygn.shzxlz.cn

[y for x in nested for y in x]
来源：http://wgv.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://etg.yongpay.top

max(d, key=d.get)
来源：http://qas.tanke756.top

[U10] Py：按值排序字典
来源：http://dfv.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://npz.yj202588.top

[U11] Py：生成器表达式
来源：http://zdc.feifeiyinyue.top

(x * 2 for x in arr)
来源：http://kmi.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kdu.gogol.net.cn

Counter(arr).most_common(3)
来源：http://thv.shzxlz.cn

[U13] Py：固定长度队列
来源：http://kge.ppjwa.cn

deque(maxlen=10)
来源：http://apw.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://ybg.cdnleiting.top

defaultdict(list)
来源：http://wmk.smart0.xyz

[U15] Py：高精度计时
来源：http://ikj.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://umj.xylfe.cn

[U16] Py：命令行参数解析
来源：http://lob.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nnb.jinqigfzy.top

[U17] Py：初始化日志
来源：http://von.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://pfe.ppjwa.cn

[U18] Py：预编译正则
来源：http://fxw.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://pgk.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://ylu.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ote.yj202588.top

[U20] Py：缓存函数结果
来源：http://pmh.hnxiangtu.top

@functools.lru_cache(maxsize=None)
来源：http://kmb.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://ptt.jiagoushi.top

@contextlib.contextmanager
来源：http://mrv.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://vnf.snrcjt.cn

list(zip(*m))
来源：http://isr.hcnkem.com

[U23] Py：分块读取大文件
来源：http://lew.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zuc.hnxiangtu.top

[U24] Py：路径操作
来源：http://rrt.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://slv.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://ddd.bbcook.cn

csv.DictReader(f)
来源：http://xij.zdbjq.cn

[U26] Py：并发下载
来源：http://daf.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gai.xuanzx.com

[U27] Py：异步 HTTP
来源：http://mwm.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://zks.zhijiandao.cn

[U28] Py：类型别名
来源：http://wzr.haohaochexian.top

UserId = int
来源：http://sbh.svipenyu.cn

[U29] Py：属性校验
来源：http://vhp.tianlin.xyz

@property 与 @x.setter 配合
来源：http://rgh.hcnkem.com

[U30] Py：数据类
来源：http://qgt.ybcxt.top

@dataclass(slots=True)
来源：http://cym.hysaishi.cn

[U31] Py：单测
来源：http://gry.bbcook.cn

python -m pytest -q
来源：http://dqp.xuanzx.com

[U32] Py：代码格式化
来源：http://ydw.cqqwz.cn

ruff format . && ruff check --fix .
来源：http://mfd.ppjwa.cn

[U33] Py：打包发布
来源：http://aev.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://tos.aibaodan.cn

[U34] Py：判断编码
来源：http://ztp.dashuyun.cn

chardet.detect(raw)
来源：http://nlz.yj20258888.top

[U35] Py：发送邮件
来源：http://xpy.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dqu.kuanghao11.cn

[U36] Py：定时任务
来源：http://ehk.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://gan.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://wsb.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://foy.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://bcq.tian-w.cn

Path(__file__).resolve().parent
来源：http://sjm.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://vxk.jqgufenzy.top

sys.stdout.isatty()
来源：http://ssx.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://lxw.fktsv.cn

print("err", file=sys.stderr)
来源：http://nhs.hywenlv.cn

[U41] PHP：初始化 Composer 项目
来源：http://ybw.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cpu.xylfe.cn

[U42] PHP：PSR-4 自动加载
来源：http://zsf.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eot.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://ccd.zhengqikj.top

namespace App\Http;
来源：http://wmu.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://hgt.wangshuangyany.cn

declare(strict_types=1);
来源：http://uup.nwbrower.top

[U45] PHP：类型声明与返回类型
来源：http://eer.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bmx.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://rkf.jinqigufen.top

?string $name = null
来源：http://gun.zdbjq.cn

[U47] PHP：联合类型
来源：http://vxl.fanxiaobao.xyz

int|string $id
来源：http://cop.haohaochexian.top

[U48] PHP：纯枚举
来源：http://wlu.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ezw.cdnleiting.top

[U49] PHP：只读属性
来源：http://zwc.gzhubu.top

public readonly string $name
来源：http://qba.chenjidiqi.icu

[U50] PHP：构造器属性提升
来源：http://che.smart0.xyz

public function __construct(private int $id) {}
来源：http://ytq.zhaomingkeji.xyz

[U51] PHP：数组解构
来源：http://iws.wangdashe.top

[$a, $b] = $arr;
来源：http://jek.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://mga.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://dpk.havefunace.top

[U53] PHP：空合并运算符
来源：http://jqd.cheryme.top

$v = $a ?? $b ?? "default";
来源：http://ree.andypj.xyz

[U54] PHP：空安全调用
来源：http://ggh.mhx1999.top

$obj?->method()
来源：http://xof.xinyue.icu

[U55] PHP：match 表达式
来源：http://fck.wangdashe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xbw.jinqigfzy.top

[U56] PHP：命名参数
来源：http://obv.yongpay.top

f(a: 1, b: 2)
来源：http://jzk.aibaodan.cn

[U57] PHP：字符串插值
来源：http://hqf.chenzaomai.com

"值: {$a}"
来源：http://kxj.bjfxy.top

[U58] PHP：数组三件套
来源：http://cis.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jqd.yuxming.cn

[U59] PHP：自定义排序
来源：http://bew.yanxiufei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ioa.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://war.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xqj.feifeiyinyue.top

[U61] PHP：正则
来源：http://ypn.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jny.shuidangran.top

[U62] PHP：日期对象
来源：http://ntu.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://axg.zycfv.cn

[U63] PHP：文件读写
来源：http://wlt.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zgx.fengsongda.top

[U64] PHP：目录遍历
来源：http://mxh.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://urp.shuidangran.top

[U65] PHP：会话
来源：http://zlg.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ben.ivvv.top

[U66] PHP：设置 Cookie
来源：http://umu.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ned.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://eqc.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xwh.epnwcf.com

[U68] PHP：PDO 连接
来源：http://tfx.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qur.pengpengdd.cyou


<!-- 参考信息 -->