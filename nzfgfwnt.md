代发 wailian999

[S35] C++：map
来源：http://iwe.aibaodan.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://coi.yvedp.cn

[S36] C++：unordered_map
来源：http://lvw.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://byh.yueranfly.top

[S37] C++：set
来源：http://jol.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gmj.meibo888.top

[S38] C++：排序
来源：http://fqd.uphjek.com

std::sort(v.begin(), v.end());
来源：http://dkr.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://ipi.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gva.smart0.xyz

[S40] C++：查找元素
来源：http://ngi.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qbx.cashguo.top

[S41] C++：类与构造函数
来源：http://dcl.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://giy.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://hrr.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://qit.yonumen.top

[S43] C++：智能指针
来源：http://wef.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://plg.gaohongyu789.top

[S44] C++：引用传参
来源：http://pun.birdmap.top

void inc(int &x) { ++x; }
来源：http://rti.pengpengdd.cyou

[S45] C++：lambda
来源：http://wom.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://zar.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://zhx.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kbf.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://vzs.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jgm.zdbjq.cn

[S48] C++：逐行读文件
来源：http://wpk.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jig.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://nzz.ctjpmb.com

[S49] C++：写文件
来源：http://bfg.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://woh.hcnkem.com

[S50] C++：格式化数字
来源：http://gaf.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kmq.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://thr.hywenlv.cn

static_cast<double>(a) / b
来源：http://hqm.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://bay.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://owg.xinyue.icu

[S53] C++：移动语义
来源：http://mox.yj202588.top

std::vector<int> w = std::move(v);
来源：http://xqt.hysaishi.cn

[S54] C++：异常处理
来源：http://guk.yj20258888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sgv.snrcjt.cn

[S55] C++：结构化绑定
来源：http://kzm.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://prk.ywan-chungtsiang.top

[S56] C++：optional
来源：http://cex.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jex.cheryme.top

[S57] C++：编译期常量
来源：http://hou.ydzc1.top

constexpr int N = 10;
来源：http://cpb.redwolf501.top

[S58] C++：命名空间
来源：http://zxx.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://aza.hfpthk.cn

[S59] C++：静态断言
来源：http://aov.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://snb.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://jsr.sjlbkw.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dcm.vqdsnc.cn

================================================================================
来源：http://dfh.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vdk.tarul.cn

================================================================================
来源：http://ami.wangdashe.top

[T01] Kotlin：Hello World
来源：http://wrq.dashuyun.cn

println("Hello")
来源：http://nye.xylfe.cn

[T02] Kotlin：变量
来源：http://mps.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uxp.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://vne.sufxvd.cn

"值: $b"
来源：http://lce.yuanzhike.top

[T04] Kotlin：空安全
来源：http://rfh.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://fsl.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://pzj.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oqm.316326.xyz

[T06] Kotlin：集合映射
来源：http://jny.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://frk.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://eef.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uxi.yj202588.top

[T08] Kotlin：数据类
来源：http://lbi.yj202588.top

data class User(val name: String, val age: Int)
来源：http://yju.jianghu66.top

[T09] Kotlin：扩展函数
来源：http://hmz.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://mam.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://ssg.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://tgq.gaohongyu789.top

[T11] Kotlin：协程
来源：http://sww.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rmb.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://mvs.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://aqk.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://ozp.sxryk.cn

val m = mapOf("a" to 1)
来源：http://tlm.dashuyun.cn

[T14] Kotlin：循环
来源：http://han.havefunace.top

for (i in 1..10) println(i)
来源：http://uvc.svipenyu.cn

[T15] Kotlin：接口
来源：http://emn.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://wxg.mhx1999.top

[T16] Swift：Hello World
来源：http://rbo.xinyue.icu

print("Hello")
来源：http://lht.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://tql.cqqwz.cn

var a = 1;  let b = 2
来源：http://yrz.redwolf501.top

[T18] Swift：字符串插值
来源：http://ffa.dianchejie.cn

"值: \(b)"
来源：http://gwl.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://huu.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://qgq.gzhubu.top

[T20] Swift：数组操作
来源：http://ign.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://der.ivvv.top

[T21] Swift：遍历
来源：http://dvq.yueranfly.top

for x in a { print(x) }
来源：http://aql.xinyue.icu

[T22] Swift：字典
来源：http://skz.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://bds.chenjidiqi.icu

[T23] Swift：函数
来源：http://pcp.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eks.zhixingplan.top

[T24] Swift：闭包
来源：http://mky.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iht.meibo888.top

[T25] Swift：结构体
来源：http://qbg.haohaochexian.top

struct P { var x: Int }
来源：http://cic.wangdashe.top

[T26] Swift：类与重写
来源：http://gdd.tian-w.cn

class A: Base { override func f() {} }
来源：http://syg.jqgufenzy.top

[T27] Swift：错误处理
来源：http://uer.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://pnm.tarul.cn

[T28] Swift：枚举
来源：http://epi.hesvh.cn

enum Color { case red, green }
来源：http://zgf.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://vjc.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://bgh.zhongyouzk.top

[T30] Swift：协议
来源：http://dpa.chenjidiqi.icu

protocol Shape { func area() -> Double }
来源：http://jze.hfpthk.cn

[T31] Lua：Hello World
来源：http://abw.zhijiandao.cn

print("Hello")
来源：http://feg.c1oappe.top

[T32] Lua：局部变量
来源：http://icv.tian-w.cn

local a = 1
来源：http://uwf.smart0.xyz

[T33] Lua：表（数组）
来源：http://hyd.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://zax.fehbvm.com

[T34] Lua：遍历表
来源：http://mur.jinqigfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://skb.pycfn.com

[T35] Lua：字典表
来源：http://cud.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://iwg.dianchejie.cn

[T36] Lua：函数
来源：http://lif.ydjk.org.cn

function add(a, b) return a + b end
来源：http://fxr.zhoulong.xyz

[T37] Lua：字符串拼接
来源：http://osk.nwbrower.top

"a" .. "b"
来源：http://kjg.guowangkeji.top

[T38] Lua：条件
来源：http://yei.gotoacloud.top

if x > 0 then print("正") end
来源：http://nyf.mhx1999.top

[T39] Lua：模式匹配
来源：http://kor.xuetiantiany.cn

string.find(s, "%d+")
来源：http://gzh.0kj1m.cn

[T40] Lua：元表
来源：http://nol.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://lul.yangfankeji.com

[T41] Perl：Hello World
来源：http://wtq.hesvh.cn

print "Hello\n";
来源：http://muh.sweek.top

[T42] Perl：变量类型
来源：http://oym.daxiang520.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oki.hywenlv.cn

[T43] Perl：字符串插值
来源：http://yel.aizwys.cn

"值: $a"
来源：http://qtt.ppjwa.cn

[T44] Perl：条件
来源：http://xhs.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://mhs.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://sua.haohaochexian.top

for my $x (@arr) { print $x; }
来源：http://wsg.sufxvd.cn

[T46] Perl：哈希操作
来源：http://qxi.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dpz.nwbrower.top

[T47] Perl：正则捕获
来源：http://rza.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pce.mhx1999.top

[T48] Perl：正则替换
来源：http://tnh.hesvh.cn

$s =~ s/old/new/g;
来源：http://yig.yj20258.top

[T49] Perl：函数
来源：http://wgx.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ctl.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://ebu.52xcode.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nhu.ydzc1.top

while (my $line = <$fh>) { print $line; }
来源：http://xhj.sjlbkw.cn

[T51] Scala：Hello World
来源：http://ucx.yonumen.top

println("Hello")
来源：http://snn.epnwcf.com

[T52] Scala：变量
来源：http://lrt.jinqigufen.top

val a = 1;  var b = 2
来源：http://xhx.jianghu66.top

[T53] Scala：字符串插值
来源：http://tgk.fanxiaobao.xyz

s"值: $b"
来源：http://atz.nanxuanxn.top

[T54] Scala：集合映射
来源：http://hkr.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://dyd.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://ktx.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yvn.epnwcf.com

[T56] Scala：样例类
来源：http://eux.hammf.cn

case class User(name: String, age: Int)
来源：http://orp.dianchejie.cn

[T57] Scala：模式匹配
来源：http://zqr.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pkn.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://nyy.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fkq.hywenlv.cn

[T59] Scala：循环
来源：http://iyd.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://fip.nanxuanxn.top

[T60] Scala：折叠
来源：http://ysw.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nxs.shangyingyoupin.top

================================================================================
来源：http://gqb.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fba.c1oappe.top

================================================================================
来源：http://mde.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://kcw.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://xen.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://lwy.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hew.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://xvg.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kfm.chenlongwang.top

[U04] Py：变量调试打印
来源：http://qmh.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fgw.gzhubu.top

[U05] Py：列表去重且保序
来源：http://xav.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://wqu.redwolf501.top

[U06] Py：合并两个字典
来源：http://unw.havefunace.top

{**a, **b}
来源：http://svu.fehbvm.com

[U07] Py：反转字典键值
来源：http://gae.fzhhl.top

{v: k for k, v in d.items()}
来源：http://pno.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://bvx.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://lve.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://qdy.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://hrk.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://cuj.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ljw.zhengqikj.top

[U11] Py：生成器表达式
来源：http://kcs.xuanzx.com

(x * 2 for x in arr)
来源：http://bwd.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tek.ivvv.top

Counter(arr).most_common(3)
来源：http://ccs.andypj.xyz

[U13] Py：固定长度队列
来源：http://gao.yvedp.cn

deque(maxlen=10)
来源：http://lqp.hcnkem.com

[U14] Py：分组收集到列表
来源：http://hpa.jianghu66.top

defaultdict(list)
来源：http://hqh.zdbjq.cn

[U15] Py：高精度计时
来源：http://tik.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://wno.mhx1999.top

[U16] Py：命令行参数解析
来源：http://dae.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wkd.uphjek.com

[U17] Py：初始化日志
来源：http://uvv.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://irp.smart0.xyz

[U18] Py：预编译正则
来源：http://gxa.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://dpt.c1oappe.top

[U19] Py：正则替换带回调
来源：http://mry.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://crz.hammf.cn

[U20] Py：缓存函数结果
来源：http://bnv.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://ctk.andypj.xyz

[U21] Py：自定义上下文管理器
来源：http://cjj.ivvv.top

@contextlib.contextmanager
来源：http://slr.zhixingplan.top

[U22] Py：矩阵转置
来源：http://qcn.zhengqikj.top

list(zip(*m))
来源：http://nlf.dashuyun.cn

[U23] Py：分块读取大文件
来源：http://xft.yanxiufei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xtb.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://qbd.gogol.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qzx.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://whn.chenjidiqi.icu

csv.DictReader(f)
来源：http://qpj.ehwqpu.com

[U26] Py：并发下载
来源：http://igf.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qoe.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://gdx.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://nxt.sufxvd.cn

[U28] Py：类型别名
来源：http://esw.fehbvm.com

UserId = int
来源：http://ivj.redwolf501.top

[U29] Py：属性校验
来源：http://bdl.ybcxt.top

@property 与 @x.setter 配合
来源：http://iem.jiagoushi.top

[U30] Py：数据类
来源：http://inh.xuetiantiany.cn

@dataclass(slots=True)
来源：http://han.haohaochexian.top

[U31] Py：单测
来源：http://tly.cashguo.top

python -m pytest -q
来源：http://urf.snrcjt.cn

[U32] Py：代码格式化
来源：http://vav.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://rcj.jinqigfzy.top

[U33] Py：打包发布
来源：http://brw.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://fly.xuanzx.com

[U34] Py：判断编码
来源：http://sws.wangdashe.top

chardet.detect(raw)
来源：http://nmj.svipenyu.cn

[U35] Py：发送邮件
来源：http://mfh.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pzs.chenzaomai.com

[U36] Py：定时任务
来源：http://olb.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://ygc.iojbl.cn

[U37] Py：读写 Excel
来源：http://wns.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eio.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://gzg.bbcook.cn

Path(__file__).resolve().parent
来源：http://lsh.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://kjy.jqgufenzy.top

sys.stdout.isatty()
来源：http://kot.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://gqi.yuxming.cn

print("err", file=sys.stderr)
来源：http://czg.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://wrh.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fzw.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://ync.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dis.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://qij.hesvh.cn

namespace App\Http;
来源：http://biq.daria6918.cn

[U44] PHP：开启严格类型
来源：http://dzx.nanxinkj.top

declare(strict_types=1);
来源：http://euo.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://juz.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ypt.xylfe.cn

[U46] PHP：可空类型
来源：http://ubh.c1oappe.top

?string $name = null
来源：http://dfd.cqqwz.cn

[U47] PHP：联合类型
来源：http://efn.52xcode.cn

int|string $id
来源：http://gny.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://pcn.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qfv.yvedp.cn

[U49] PHP：只读属性
来源：http://eni.dianchejie.cn

public readonly string $name
来源：http://taj.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://zmd.hywenlv.cn

public function __construct(private int $id) {}
来源：http://erh.tarul.cn

[U51] PHP：数组解构
来源：http://mdq.chenlongwang.top

[$a, $b] = $arr;
来源：http://hie.yangfankeji.com

[U52] PHP：箭头函数
来源：http://rit.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://izt.chenjidiqi.icu

[U53] PHP：空合并运算符
来源：http://soy.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://aru.vehdjk.com

[U54] PHP：空安全调用
来源：http://zeg.quarkkingdee.top

$obj?->method()
来源：http://zug.xinyue.icu

[U55] PHP：match 表达式
来源：http://jyl.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sbi.birdmap.top

[U56] PHP：命名参数
来源：http://jrb.xylfe.cn

f(a: 1, b: 2)
来源：http://rgq.shangyingyoupin.top

[U57] PHP：字符串插值
来源：http://qnh.sweek.top

"值: {$a}"
来源：http://vsa.52xcode.cn

[U58] PHP：数组三件套
来源：http://tmc.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vxd.gogol.net.cn

[U59] PHP：自定义排序
来源：http://ggd.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iic.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://mtc.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dzq.zhaomingkeji.xyz


<!-- 参考信息 -->