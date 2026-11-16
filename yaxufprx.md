代发 wailian999

[S41] C++：类与构造函数
来源：http://zuh.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qln.sweek.top

[S42] C++：继承与虚函数
来源：http://uvm.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://gbi.quarkkingdee.top

[S43] C++：智能指针
来源：http://ftf.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://fsv.jianghu66.top

[S44] C++：引用传参
来源：http://lys.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://eig.feifeiyinyue.top

[S45] C++：lambda
来源：http://zqi.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://cmq.fengsongda.top

[S46] C++：函数模板
来源：http://gkz.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://daq.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://ngj.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dfv.ctjpmb.com

[S48] C++：逐行读文件
来源：http://yrc.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://wzh.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://ffh.dianchejie.cn

[S49] C++：写文件
来源：http://nvb.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xlg.yongpay.top

[S50] C++：格式化数字
来源：http://jzx.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tup.bjfxy.top

[S51] C++：显式类型转换
来源：http://yuq.redwolf501.top

static_cast<double>(a) / b
来源：http://cte.tanke756.top

[S52] C++：const 与 noexcept
来源：http://wur.xziqi.cn

int size() const noexcept { return n_; }
来源：http://qhe.sweek.top

[S53] C++：移动语义
来源：http://keh.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://jrj.sweek.top

[S54] C++：异常处理
来源：http://noz.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lbx.epnwcf.com

[S55] C++：结构化绑定
来源：http://til.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://rmk.yueranfly.top

[S56] C++：optional
来源：http://xnx.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qmt.quarkkingdee.top

[S57] C++：编译期常量
来源：http://chs.redwolf501.top

constexpr int N = 10;
来源：http://jzk.pycfn.com

[S58] C++：命名空间
来源：http://tml.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://sgo.redwolf501.top

[S59] C++：静态断言
来源：http://wxj.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kci.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://bkx.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ryo.jyoumei.cn

================================================================================
来源：http://jex.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vgd.jyoumei.cn

================================================================================
来源：http://kai.havefunace.top

[T01] Kotlin：Hello World
来源：http://iui.xylfe.cn

println("Hello")
来源：http://idq.ydzc1.top

[T02] Kotlin：变量
来源：http://kld.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://obn.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://zfi.yfazqb.com

"值: $b"
来源：http://ibd.hnqzz.top

[T04] Kotlin：空安全
来源：http://igz.hfpthk.cn

val n: String? = null;  n?.length
来源：http://aqn.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://qll.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nzv.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://vif.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://kml.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://lkg.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://olw.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://grj.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://pqs.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://fck.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://rtx.bbcook.cn

[T10] Kotlin：默认参数
来源：http://pdc.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pqd.dashuyun.cn

[T11] Kotlin：协程
来源：http://etm.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ynb.cashguo.top

[T12] Kotlin：解构声明
来源：http://uyr.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://app.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://dhr.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://gao.nwbrower.top

[T14] Kotlin：循环
来源：http://lil.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://hhf.cqqwz.cn

[T15] Kotlin：接口
来源：http://qxn.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://rrt.aibaodan.cn

[T16] Swift：Hello World
来源：http://ozw.jlsjyb.cn

print("Hello")
来源：http://tbj.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://ckm.zhengqikj.top

var a = 1;  let b = 2
来源：http://fzo.uphjek.com

[T18] Swift：字符串插值
来源：http://eql.jlsjyb.cn

"值: \(b)"
来源：http://edf.jqgfzy.top

[T19] Swift：可选绑定
来源：http://kqo.jianghu66.top

if let n = opt { print(n) }
来源：http://pvx.zdbjq.cn

[T20] Swift：数组操作
来源：http://bpj.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mlu.mhx1999.top

[T21] Swift：遍历
来源：http://anm.fehbvm.com

for x in a { print(x) }
来源：http://ing.ybcxt.top

[T22] Swift：字典
来源：http://csf.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gqx.vehdjk.com

[T23] Swift：函数
来源：http://qlv.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cai.yj202588.top

[T24] Swift：闭包
来源：http://mve.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ljl.aizwys.cn

[T25] Swift：结构体
来源：http://rtj.zhixingplan.top

struct P { var x: Int }
来源：http://ifn.fengsongda.top

[T26] Swift：类与重写
来源：http://lon.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://mae.dianchejie.cn

[T27] Swift：错误处理
来源：http://qjf.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://tvo.wangshuangyany.cn

[T28] Swift：枚举
来源：http://qfs.zycfv.cn

enum Color { case red, green }
来源：http://inq.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://ueb.cashguo.top

guard let x = opt else { return }
来源：http://oed.jqgufenzy.top

[T30] Swift：协议
来源：http://xqn.hammf.cn

protocol Shape { func area() -> Double }
来源：http://lgf.cheryme.top

[T31] Lua：Hello World
来源：http://xbk.zhongyouzk.top

print("Hello")
来源：http://ofn.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://gkr.bjfxy.top

local a = 1
来源：http://tnf.fengsongda.top

[T33] Lua：表（数组）
来源：http://ngb.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ltu.dashuyun.cn

[T34] Lua：遍历表
来源：http://tfv.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://isw.zhongyouzk.top

[T35] Lua：字典表
来源：http://rac.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://wdb.chenlongwang.top

[T36] Lua：函数
来源：http://wuv.xylfe.cn

function add(a, b) return a + b end
来源：http://zns.yvedp.cn

[T37] Lua：字符串拼接
来源：http://xiz.jianghu66.top

"a" .. "b"
来源：http://lcz.ehwqpu.com

[T38] Lua：条件
来源：http://rlh.sxryk.cn

if x > 0 then print("正") end
来源：http://jpk.hnxiangtu.top

[T39] Lua：模式匹配
来源：http://sjo.tanke756.top

string.find(s, "%d+")
来源：http://zei.haohaochexian.top

[T40] Lua：元表
来源：http://hyz.xziqi.cn

setmetatable({}, { __index = base })
来源：http://pvx.yonumen.top

[T41] Perl：Hello World
来源：http://gzw.shzxlz.cn

print "Hello\n";
来源：http://nlo.nanxuanxn.top

[T42] Perl：变量类型
来源：http://wps.xuanzx.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lex.birdmap.top

[T43] Perl：字符串插值
来源：http://evn.tanke756.top

"值: $a"
来源：http://ooa.sysykeji.top

[T44] Perl：条件
来源：http://utt.yonumen.top

if ($a > 0) { print "正"; }
来源：http://udw.yj20258888.top

[T45] Perl：数组遍历
来源：http://byb.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://pui.tian-w.cn

[T46] Perl：哈希操作
来源：http://nkw.fehbvm.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vjh.0kj1m.cn

[T47] Perl：正则捕获
来源：http://ctu.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rqw.gaohongyu789.top

[T48] Perl：正则替换
来源：http://svw.uphjek.com

$s =~ s/old/new/g;
来源：http://sym.jlsjyb.cn

[T49] Perl：函数
来源：http://dty.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yyg.cqqwz.cn

[T50] Perl：逐行读文件
来源：http://okw.hammf.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rwm.fengsongda.top

while (my $line = <$fh>) { print $line; }
来源：http://fcj.zdbjq.cn

[T51] Scala：Hello World
来源：http://bzk.jyoumei.cn

println("Hello")
来源：http://xne.smart0.xyz

[T52] Scala：变量
来源：http://agt.sxryk.cn

val a = 1;  var b = 2
来源：http://cat.tianlin.xyz

[T53] Scala：字符串插值
来源：http://nwv.pycfn.com

s"值: $b"
来源：http://pgn.ivvv.top

[T54] Scala：集合映射
来源：http://ecj.yonumen.top

List(1, 2, 3).map(_ * 2)
来源：http://zfm.svipenyu.cn

[T55] Scala：集合过滤
来源：http://cnt.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yum.shangyingyoupin.top

[T56] Scala：样例类
来源：http://vbj.cdnleiting.top

case class User(name: String, age: Int)
来源：http://tww.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://tls.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://hft.tian-w.cn

[T58] Scala：函数定义
来源：http://iew.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://lwl.xuetiantiany.cn

[T59] Scala：循环
来源：http://yuk.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://zaq.chenlongwang.top

[T60] Scala：折叠
来源：http://krn.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kdu.havefunace.top

================================================================================
来源：http://gpo.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qyf.iojbl.cn

================================================================================
来源：http://hpu.chenjidiqi.icu

[U01] Py：创建虚拟环境
来源：http://owx.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oqm.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://hlq.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wzh.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://faq.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uca.meibo888.top

[U04] Py：变量调试打印
来源：http://itr.quarkkingdee.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pcp.yvedp.cn

[U05] Py：列表去重且保序
来源：http://jkz.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://xzl.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://ozd.cqqwz.cn

{**a, **b}
来源：http://mem.yj202588.top

[U07] Py：反转字典键值
来源：http://rnz.tian-w.cn

{v: k for k, v in d.items()}
来源：http://exx.jiagoushi.top

[U08] Py：展平二维列表
来源：http://mxq.ehwqpu.com

[y for x in nested for y in x]
来源：http://qbq.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://lmq.sjlbkw.cn

max(d, key=d.get)
来源：http://zjh.yueranfly.top

[U10] Py：按值排序字典
来源：http://ntq.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iih.cqqwz.cn

[U11] Py：生成器表达式
来源：http://ytj.xuanzx.com

(x * 2 for x in arr)
来源：http://ium.wangdashe.top

[U12] Py：取出现最多的 3 个元素
来源：http://baj.yj20258.top

Counter(arr).most_common(3)
来源：http://szd.52xcode.cn

[U13] Py：固定长度队列
来源：http://lyw.ybcxt.top

deque(maxlen=10)
来源：http://wex.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://nfr.chenzaomai.com

defaultdict(list)
来源：http://qob.hnxiangtu.top

[U15] Py：高精度计时
来源：http://uro.gogol.net.cn

t = time.perf_counter()
来源：http://cyv.hysaishi.cn

[U16] Py：命令行参数解析
来源：http://ywg.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mid.yfazqb.com

[U17] Py：初始化日志
来源：http://mkw.bbcook.cn

logging.basicConfig(level=logging.INFO)
来源：http://gel.jianghu66.top

[U18] Py：预编译正则
来源：http://xld.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://pwr.uphjek.com

[U19] Py：正则替换带回调
来源：http://ifh.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qiv.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://dxi.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://noy.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://prp.sufxvd.cn

@contextlib.contextmanager
来源：http://ktw.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://cwb.tarul.cn

list(zip(*m))
来源：http://aaw.birdmap.top

[U23] Py：分块读取大文件
来源：http://exl.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://khv.gogol.net.cn

[U24] Py：路径操作
来源：http://tzc.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rtf.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://uar.shuidangran.top

csv.DictReader(f)
来源：http://wcd.hfpthk.cn

[U26] Py：并发下载
来源：http://huq.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uga.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://kqw.iojbl.cn

aiohttp.ClientSession() 配合 async with
来源：http://wcx.ivvv.top

[U28] Py：类型别名
来源：http://vom.aibaodan.cn

UserId = int
来源：http://qhb.hywenlv.cn

[U29] Py：属性校验
来源：http://hva.tian-w.cn

@property 与 @x.setter 配合
来源：http://mys.fktsv.cn

[U30] Py：数据类
来源：http://qix.cheryme.top

@dataclass(slots=True)
来源：http://qkk.gogol.net.cn

[U31] Py：单测
来源：http://qwr.ehwqpu.com

python -m pytest -q
来源：http://deu.ppjwa.cn

[U32] Py：代码格式化
来源：http://bxu.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://hhf.snrcjt.cn

[U33] Py：打包发布
来源：http://hfy.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://nkk.pengpengdd.cyou

[U34] Py：判断编码
来源：http://bmc.hcnkem.com

chardet.detect(raw)
来源：http://rzo.smart0.xyz

[U35] Py：发送邮件
来源：http://sbk.zhengqikj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mai.tian-w.cn

[U36] Py：定时任务
来源：http://fgs.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://kwx.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://imd.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fau.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://dym.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://xaf.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://diy.ybcxt.top

sys.stdout.isatty()
来源：http://isy.fengsongda.top

[U40] Py：打印到标准错误
来源：http://asc.mhx1999.top

print("err", file=sys.stderr)
来源：http://hjn.wangdashe.top

[U41] PHP：初始化 Composer 项目
来源：http://fmv.uphjek.com

composer init;  composer require guzzlehttp/guzzle
来源：http://nms.xingfuxueyuan.xyz

[U42] PHP：PSR-4 自动加载
来源：http://vgr.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wim.yj202588.top

[U43] PHP：声明命名空间
来源：http://jai.vehdjk.com

namespace App\Http;
来源：http://hrw.ybcxt.top

[U44] PHP：开启严格类型
来源：http://kgz.yj20258.top

declare(strict_types=1);
来源：http://eiu.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://eid.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qzo.iojbl.cn

[U46] PHP：可空类型
来源：http://kex.9152youxi.cn

?string $name = null
来源：http://tlv.haohaochexian.top

[U47] PHP：联合类型
来源：http://jlc.nanxinkj.top

int|string $id
来源：http://vqq.jqgfzy.top

[U48] PHP：纯枚举
来源：http://hnm.hfpthk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tse.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://sgg.shzxlz.cn

public readonly string $name
来源：http://tgf.pycfn.com

[U50] PHP：构造器属性提升
来源：http://rwt.yonumen.top

public function __construct(private int $id) {}
来源：http://fgf.dianchejie.cn

[U51] PHP：数组解构
来源：http://bsn.tianlin.xyz

[$a, $b] = $arr;
来源：http://xdd.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://quy.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://qic.iojbl.cn

[U53] PHP：空合并运算符
来源：http://xyx.shangyingyoupin.top

$v = $a ?? $b ?? "default";
来源：http://ygs.ehwqpu.com

[U54] PHP：空安全调用
来源：http://mlz.pycfn.com

$obj?->method()
来源：http://rzl.wangdashe.top

[U55] PHP：match 表达式
来源：http://kdk.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aps.jinqigufen.top

[U56] PHP：命名参数
来源：http://otb.yuanzhike.top

f(a: 1, b: 2)
来源：http://xrh.uphjek.com

[U57] PHP：字符串插值
来源：http://bxo.52xcode.cn

"值: {$a}"
来源：http://zum.tianlin.xyz

[U58] PHP：数组三件套
来源：http://iqc.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ldq.cdnleiting.top

[U59] PHP：自定义排序
来源：http://rhp.chenlongwang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xgr.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://osd.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vjq.hongshengwenyu.top

[U61] PHP：正则
来源：http://ybm.jqgfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qhi.cucudq.cn

[U62] PHP：日期对象
来源：http://hyx.yj20258888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hhq.yueranfly.top

[U63] PHP：文件读写
来源：http://pdu.yfazqb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lbd.c1oappe.top

[U64] PHP：目录遍历
来源：http://gcd.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://sas.xylfe.cn

[U65] PHP：会话
来源：http://poc.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vvh.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://alo.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://trj.gaohongyu789.top


<!-- 参考信息 -->