代发 wailian999

[S35] C++：map
来源：http://zgi.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vlf.cqqwz.cn

[S36] C++：unordered_map
来源：http://byj.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fee.ivvv.top

[S37] C++：set
来源：http://tnz.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nsu.tian-w.cn

[S38] C++：排序
来源：http://jpm.yongpay.top

std::sort(v.begin(), v.end());
来源：http://avw.sweek.top

[S39] C++：自定义比较器排序
来源：http://lje.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ads.zhiwuduotai.top

[S40] C++：查找元素
来源：http://xiy.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nai.c1oappe.top

[S41] C++：类与构造函数
来源：http://mhv.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nrh.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://xgn.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://lzx.ehwqpu.com

[S43] C++：智能指针
来源：http://fjr.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://zfy.fehbvm.com

[S44] C++：引用传参
来源：http://klc.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://auw.hammf.cn

[S45] C++：lambda
来源：http://xtf.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fzs.ctjpmb.com

[S46] C++：函数模板
来源：http://svz.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://usv.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://zqm.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rrr.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://lri.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://okt.sweek.top

while (std::getline(in, line)) { }
来源：http://wla.dashuyun.cn

[S49] C++：写文件
来源：http://cbt.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kkn.jqgfzy.top

[S50] C++：格式化数字
来源：http://xci.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aek.tanke756.top

[S51] C++：显式类型转换
来源：http://oky.zdbjq.cn

static_cast<double>(a) / b
来源：http://sus.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://bsy.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://kpu.wangdashe.top

[S53] C++：移动语义
来源：http://bxe.birdmap.top

std::vector<int> w = std::move(v);
来源：http://bpb.nanxuanxn.top

[S54] C++：异常处理
来源：http://hny.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vqc.vehdjk.com

[S55] C++：结构化绑定
来源：http://npq.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hfr.fengsongda.top

[S56] C++：optional
来源：http://bzb.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bvp.shuidangran.top

[S57] C++：编译期常量
来源：http://lbg.haohaochexian.top

constexpr int N = 10;
来源：http://exh.iojbl.cn

[S58] C++：命名空间
来源：http://nxp.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://zxt.hysaishi.cn

[S59] C++：静态断言
来源：http://esn.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lni.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://nis.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kbk.havefunace.top

================================================================================
来源：http://vsh.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yzj.vqdsnc.cn

================================================================================
来源：http://syb.bbcook.cn

[T01] Kotlin：Hello World
来源：http://efg.sxryk.cn

println("Hello")
来源：http://zes.yongpay.top

[T02] Kotlin：变量
来源：http://jcf.hnxiangtu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mgx.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://aqd.zycfv.cn

"值: $b"
来源：http://qmw.hammf.cn

[T04] Kotlin：空安全
来源：http://yti.yj20258888.top

val n: String? = null;  n?.length
来源：http://onh.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://maq.jinyuanbaomall.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://svn.tian-w.cn

[T06] Kotlin：集合映射
来源：http://foz.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://euj.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://osd.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://tcq.ehwqpu.com

[T08] Kotlin：数据类
来源：http://not.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://get.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://uja.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://zcp.bbcook.cn

[T10] Kotlin：默认参数
来源：http://rna.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kmx.fktsv.cn

[T11] Kotlin：协程
来源：http://xef.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kqn.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://ldv.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://ffo.jlsjyb.cn

[T13] Kotlin：只读 Map
来源：http://scw.aizwys.cn

val m = mapOf("a" to 1)
来源：http://rmq.cqqwz.cn

[T14] Kotlin：循环
来源：http://nrz.gzhubu.top

for (i in 1..10) println(i)
来源：http://ejj.fzhhl.top

[T15] Kotlin：接口
来源：http://xlp.nwbrower.top

interface Shape { fun area(): Double }
来源：http://ndb.pycfn.com

[T16] Swift：Hello World
来源：http://aqi.hnqzz.top

print("Hello")
来源：http://auy.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://mls.cheryme.top

var a = 1;  let b = 2
来源：http://kvl.ydzc1.top

[T18] Swift：字符串插值
来源：http://lgs.nwbrower.top

"值: \(b)"
来源：http://uhl.redwolf501.top

[T19] Swift：可选绑定
来源：http://ybw.meibo888.top

if let n = opt { print(n) }
来源：http://hmd.quarkkingdee.top

[T20] Swift：数组操作
来源：http://nwc.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jnn.mhx1999.top

[T21] Swift：遍历
来源：http://jse.haohaochexian.top

for x in a { print(x) }
来源：http://yrz.sxryk.cn

[T22] Swift：字典
来源：http://nvg.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mau.ydzc1.top

[T23] Swift：函数
来源：http://jqt.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jas.yj20258888.top

[T24] Swift：闭包
来源：http://twl.fengsongda.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://edv.jqgfzy.top

[T25] Swift：结构体
来源：http://uec.yongpay.top

struct P { var x: Int }
来源：http://wpr.hysaishi.cn

[T26] Swift：类与重写
来源：http://npz.xziqi.cn

class A: Base { override func f() {} }
来源：http://hqr.sjlbkw.cn

[T27] Swift：错误处理
来源：http://agt.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://kib.jqgfzy.top

[T28] Swift：枚举
来源：http://xud.ctjpmb.com

enum Color { case red, green }
来源：http://rjq.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://wsj.xinyue.icu

guard let x = opt else { return }
来源：http://tov.dashuyun.cn

[T30] Swift：协议
来源：http://mbu.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://mya.gaohongyu789.top

[T31] Lua：Hello World
来源：http://ofd.316326.xyz

print("Hello")
来源：http://irl.nwbrower.top

[T32] Lua：局部变量
来源：http://tkg.aizwys.cn

local a = 1
来源：http://ptf.yonumen.top

[T33] Lua：表（数组）
来源：http://jxi.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tqj.jiagoushi.top

[T34] Lua：遍历表
来源：http://xpn.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pwo.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://ith.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://uhx.daxiang520.top

[T36] Lua：函数
来源：http://awy.yuxming.cn

function add(a, b) return a + b end
来源：http://udx.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://efx.chenjidiqi.icu

"a" .. "b"
来源：http://mkx.andypj.xyz

[T38] Lua：条件
来源：http://pux.bjfxy.top

if x > 0 then print("正") end
来源：http://cbo.yfazqb.com

[T39] Lua：模式匹配
来源：http://bdq.gotoacloud.top

string.find(s, "%d+")
来源：http://ztb.aizwys.cn

[T40] Lua：元表
来源：http://ylo.redwolf501.top

setmetatable({}, { __index = base })
来源：http://wgu.sufxvd.cn

[T41] Perl：Hello World
来源：http://zxy.kuanghao11.cn

print "Hello\n";
来源：http://uwf.52xcode.cn

[T42] Perl：变量类型
来源：http://yqr.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gxj.yongpay.top

[T43] Perl：字符串插值
来源：http://yfx.jinyuanbaomall.cn

"值: $a"
来源：http://vze.yj202588.top

[T44] Perl：条件
来源：http://aus.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://tnb.iojbl.cn

[T45] Perl：数组遍历
来源：http://ipm.cashguo.top

for my $x (@arr) { print $x; }
来源：http://dfa.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://eog.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qwf.wangdashe.top

[T47] Perl：正则捕获
来源：http://cgz.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gfm.xziqi.cn

[T48] Perl：正则替换
来源：http://ozy.zdqjudy.top

$s =~ s/old/new/g;
来源：http://vsl.haohaochexian.top

[T49] Perl：函数
来源：http://aqg.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xrb.tanke756.top

[T50] Perl：逐行读文件
来源：http://nzk.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ddt.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://gsd.xylfe.cn

[T51] Scala：Hello World
来源：http://xzx.xinyue.icu

println("Hello")
来源：http://pbl.haohaochexian.top

[T52] Scala：变量
来源：http://rgc.jlsjyb.cn

val a = 1;  var b = 2
来源：http://qtp.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://vpx.wangdashe.top

s"值: $b"
来源：http://mpc.gaohongyu789.top

[T54] Scala：集合映射
来源：http://qih.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://owj.316326.xyz

[T55] Scala：集合过滤
来源：http://nju.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://zuw.yj20258.top

[T56] Scala：样例类
来源：http://exv.ppjwa.cn

case class User(name: String, age: Int)
来源：http://zxi.dashuyun.cn

[T57] Scala：模式匹配
来源：http://hwn.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nel.jqgufenzy.top

[T58] Scala：函数定义
来源：http://emr.haohaochexian.top

def add(a: Int, b: Int): Int = a + b
来源：http://waj.guannengcc.top

[T59] Scala：循环
来源：http://ksu.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://lbp.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://kll.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ybt.chenjidiqi.icu

================================================================================
来源：http://mam.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cpm.gotoacloud.top

================================================================================
来源：http://pxo.dianchejie.cn

[U01] Py：创建虚拟环境
来源：http://ftf.zycfv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rtx.xuetiantiany.cn

[U02] Py：导出 / 安装依赖
来源：http://omg.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ucy.jyoumei.cn

[U03] Py：加载 .env 配置
来源：http://cev.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rvp.zdqjudy.top

[U04] Py：变量调试打印
来源：http://abz.epnwcf.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xnb.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://zio.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://zdb.316326.xyz

[U06] Py：合并两个字典
来源：http://cpv.zycfv.cn

{**a, **b}
来源：http://gwl.daxiang520.top

[U07] Py：反转字典键值
来源：http://yff.meibo888.top

{v: k for k, v in d.items()}
来源：http://guv.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://uky.ppjwa.cn

[y for x in nested for y in x]
来源：http://dna.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://yhc.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://zej.iojbl.cn

[U10] Py：按值排序字典
来源：http://cid.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://trn.aizwys.cn

[U11] Py：生成器表达式
来源：http://nzj.xinyue.icu

(x * 2 for x in arr)
来源：http://wqm.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://zyd.zdqjudy.top

Counter(arr).most_common(3)
来源：http://jgg.jinqigufen.top

[U13] Py：固定长度队列
来源：http://yhp.xuetiantiany.cn

deque(maxlen=10)
来源：http://cow.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://hvu.ybcxt.top

defaultdict(list)
来源：http://wbc.jiagoushi.top

[U15] Py：高精度计时
来源：http://yis.guannengcc.top

t = time.perf_counter()
来源：http://icn.yueranfly.top

[U16] Py：命令行参数解析
来源：http://bbz.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fbi.yuanzhike.top

[U17] Py：初始化日志
来源：http://eim.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ajt.jyoumei.cn

[U18] Py：预编译正则
来源：http://xln.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://nkn.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://ush.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zeu.smart0.xyz

[U20] Py：缓存函数结果
来源：http://evm.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://uoa.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://qwq.nanxinkj.top

@contextlib.contextmanager
来源：http://vek.ppjwa.cn

[U22] Py：矩阵转置
来源：http://oit.zhixingplan.top

list(zip(*m))
来源：http://vuf.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://kkv.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pcp.yfazqb.com

[U24] Py：路径操作
来源：http://npn.feifeiyinyue.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://viq.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://rxl.hnqzz.top

csv.DictReader(f)
来源：http://dvl.hfpthk.cn

[U26] Py：并发下载
来源：http://tqz.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zei.bjfxy.top

[U27] Py：异步 HTTP
来源：http://wwq.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://gay.xylfe.cn

[U28] Py：类型别名
来源：http://mbm.chenzaomai.com

UserId = int
来源：http://itr.yangfankeji.com

[U29] Py：属性校验
来源：http://sgi.zhixingplan.top

@property 与 @x.setter 配合
来源：http://jbu.gotoacloud.top

[U30] Py：数据类
来源：http://ytt.yj20258.top

@dataclass(slots=True)
来源：http://uah.hesvh.cn

[U31] Py：单测
来源：http://jkb.fanxiaobao.xyz

python -m pytest -q
来源：http://bwz.bbcook.cn

[U32] Py：代码格式化
来源：http://uvv.uphjek.com

ruff format . && ruff check --fix .
来源：http://zvz.yj202588.top

[U33] Py：打包发布
来源：http://wjo.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://fpl.wangdashe.top

[U34] Py：判断编码
来源：http://kuz.daxiang520.top

chardet.detect(raw)
来源：http://rhu.uphjek.com

[U35] Py：发送邮件
来源：http://usi.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jdd.shangyingyoupin.top

[U36] Py：定时任务
来源：http://bgz.tian-w.cn

schedule.every(10).minutes.do(job)
来源：http://npz.zhongyouzk.top

[U37] Py：读写 Excel
来源：http://gax.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://suz.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://ofl.dashuyun.cn

Path(__file__).resolve().parent
来源：http://utg.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://whm.chenlongwang.top

sys.stdout.isatty()
来源：http://bka.tanke756.top

[U40] Py：打印到标准错误
来源：http://wcz.sxryk.cn

print("err", file=sys.stderr)
来源：http://vwx.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://hat.kuanghao11.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nog.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://tnn.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ixf.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://pgr.shangyingyoupin.top

namespace App\Http;
来源：http://luy.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://tkd.xziqi.cn

declare(strict_types=1);
来源：http://mhz.jinqigufen.top

[U45] PHP：类型声明与返回类型
来源：http://fhz.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sgi.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://tfq.316326.xyz

?string $name = null
来源：http://ufw.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://uwq.jqgufenzy.top

int|string $id
来源：http://xag.zycfv.cn

[U48] PHP：纯枚举
来源：http://isr.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tqv.zhaomingkeji.xyz

[U49] PHP：只读属性
来源：http://sqo.jinqigfzy.top

public readonly string $name
来源：http://fox.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://xyh.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://sdt.gaohongyu789.top

[U51] PHP：数组解构
来源：http://ewl.sufxvd.cn

[$a, $b] = $arr;
来源：http://wjr.xuanzx.com

[U52] PHP：箭头函数
来源：http://bte.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://emq.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://sjp.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://ukv.zycfv.cn

[U54] PHP：空安全调用
来源：http://mkg.xuetiantiany.cn

$obj?->method()
来源：http://qlr.xinyue.icu

[U55] PHP：match 表达式
来源：http://rrn.yanxiufei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://skt.gogol.net.cn

[U56] PHP：命名参数
来源：http://fpr.xziqi.cn

f(a: 1, b: 2)
来源：http://ptf.fehbvm.com

[U57] PHP：字符串插值
来源：http://ash.gotoacloud.top

"值: {$a}"
来源：http://nga.iojbl.cn

[U58] PHP：数组三件套
来源：http://hbr.sufxvd.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lug.quarkkingdee.top

[U59] PHP：自定义排序
来源：http://pij.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mft.tarul.cn

[U60] PHP：JSON 编解码
来源：http://boh.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qzd.feifeiyinyue.top


<!-- 参考信息 -->