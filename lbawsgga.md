代发 wailian999

[S33] C++：vector 增删
来源：http://ucp.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qhi.meibo888.top

[S34] C++：遍历 vector
来源：http://uld.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://dpb.316326.xyz

[S35] C++：map
来源：http://jer.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fsj.ybcxt.top

[S36] C++：unordered_map
来源：http://tul.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mdy.dianchejie.cn

[S37] C++：set
来源：http://ezu.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vbg.chenzaomai.com

[S38] C++：排序
来源：http://axb.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://tsf.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://grn.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://arb.fehbvm.com

[S40] C++：查找元素
来源：http://rws.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sxt.ehwqpu.com

[S41] C++：类与构造函数
来源：http://xbc.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rwl.cucudq.cn

[S42] C++：继承与虚函数
来源：http://vvs.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://tiu.zhixingplan.top

[S43] C++：智能指针
来源：http://bec.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://los.0kj1m.cn

[S44] C++：引用传参
来源：http://kyi.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://pdn.haohaochexian.top

[S45] C++：lambda
来源：http://abh.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://tlq.jinqigufen.top

[S46] C++：函数模板
来源：http://edx.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zoz.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://zor.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pev.hnqzz.top

[S48] C++：逐行读文件
来源：http://rgd.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jnm.vehdjk.com

while (std::getline(in, line)) { }
来源：http://cdf.shangyingyoupin.top

[S49] C++：写文件
来源：http://kkn.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xjh.sjlbkw.cn

[S50] C++：格式化数字
来源：http://vcp.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://trk.gzhubu.top

[S51] C++：显式类型转换
来源：http://mge.jlsjyb.cn

static_cast<double>(a) / b
来源：http://ehz.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://piy.xylfe.cn

int size() const noexcept { return n_; }
来源：http://vmk.gogol.net.cn

[S53] C++：移动语义
来源：http://atr.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://kws.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://rhl.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mef.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://cln.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://irb.ydjk.org.cn

[S56] C++：optional
来源：http://mvw.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ney.birdmap.top

[S57] C++：编译期常量
来源：http://dys.zdbjq.cn

constexpr int N = 10;
来源：http://qml.yongpay.top

[S58] C++：命名空间
来源：http://gyp.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://bhh.yanxiufei.cn

[S59] C++：静态断言
来源：http://asc.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lre.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://sdk.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sxc.pengpengdd.cyou

================================================================================
来源：http://lzb.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://loo.gaohongyu789.top

================================================================================
来源：http://hcm.yj20258.top

[T01] Kotlin：Hello World
来源：http://uqa.snrcjt.cn

println("Hello")
来源：http://vjz.guannengcc.top

[T02] Kotlin：变量
来源：http://vwy.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iok.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://dtc.xingfuxueyuan.xyz

"值: $b"
来源：http://imk.jyoumei.cn

[T04] Kotlin：空安全
来源：http://psf.jinqigufen.top

val n: String? = null;  n?.length
来源：http://aog.uphjek.com

[T05] Kotlin：when 表达式
来源：http://eqa.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kgx.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://daa.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://nkq.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://iho.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://scb.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://yzs.ivvv.top

data class User(val name: String, val age: Int)
来源：http://iap.tarul.cn

[T09] Kotlin：扩展函数
来源：http://gtu.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://udm.cashguo.top

[T10] Kotlin：默认参数
来源：http://djj.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://htt.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://emm.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wya.cucudq.cn

[T12] Kotlin：解构声明
来源：http://sja.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://vdr.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://tzv.jianghu66.top

val m = mapOf("a" to 1)
来源：http://kbb.shuidangran.top

[T14] Kotlin：循环
来源：http://fyq.yueranfly.top

for (i in 1..10) println(i)
来源：http://zec.cashguo.top

[T15] Kotlin：接口
来源：http://nze.bjfxy.top

interface Shape { fun area(): Double }
来源：http://cmq.chenlongwang.top

[T16] Swift：Hello World
来源：http://ygk.meibo888.top

print("Hello")
来源：http://fuq.hammf.cn

[T17] Swift：变量与常量
来源：http://env.meibo888.top

var a = 1;  let b = 2
来源：http://jme.chenlongwang.top

[T18] Swift：字符串插值
来源：http://ify.hongshengwenyu.top

"值: \(b)"
来源：http://fpt.ivvv.top

[T19] Swift：可选绑定
来源：http://dpn.nanxuanxn.top

if let n = opt { print(n) }
来源：http://phc.gotoacloud.top

[T20] Swift：数组操作
来源：http://kky.jinqigfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://idq.gzhubu.top

[T21] Swift：遍历
来源：http://med.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://teq.epnwcf.com

[T22] Swift：字典
来源：http://qrb.tianlin.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://evb.uphjek.com

[T23] Swift：函数
来源：http://qsc.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lao.yj202588.top

[T24] Swift：闭包
来源：http://czc.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ojr.zhixingplan.top

[T25] Swift：结构体
来源：http://qru.zhixingplan.top

struct P { var x: Int }
来源：http://ipp.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://eql.redwolf501.top

class A: Base { override func f() {} }
来源：http://rsv.gzhubu.top

[T27] Swift：错误处理
来源：http://tyv.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://wms.yueranfly.top

[T28] Swift：枚举
来源：http://izt.fehbvm.com

enum Color { case red, green }
来源：http://iuh.dashuyun.cn

[T29] Swift：guard 提前返回
来源：http://nec.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://wfi.aizwys.cn

[T30] Swift：协议
来源：http://vbz.aizwys.cn

protocol Shape { func area() -> Double }
来源：http://zaa.ydzc1.top

[T31] Lua：Hello World
来源：http://afc.jinyuanbaomall.cn

print("Hello")
来源：http://lzd.jyoumei.cn

[T32] Lua：局部变量
来源：http://xfr.cdnleiting.top

local a = 1
来源：http://xsp.yuanzhike.top

[T33] Lua：表（数组）
来源：http://dci.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zdr.guowangkeji.top

[T34] Lua：遍历表
来源：http://hqw.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nni.zhijiandao.cn

[T35] Lua：字典表
来源：http://vjr.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://jrb.yanxiufei.cn

[T36] Lua：函数
来源：http://ejf.jyoumei.cn

function add(a, b) return a + b end
来源：http://rsh.ivvv.top

[T37] Lua：字符串拼接
来源：http://uxh.yuxming.cn

"a" .. "b"
来源：http://ryy.shuidangran.top

[T38] Lua：条件
来源：http://zoa.sweek.top

if x > 0 then print("正") end
来源：http://jpb.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://chq.nanxinkj.top

string.find(s, "%d+")
来源：http://era.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://dba.yuxming.cn

setmetatable({}, { __index = base })
来源：http://zjk.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://hsr.yuanzhike.top

print "Hello\n";
来源：http://dhx.guannengcc.top

[T42] Perl：变量类型
来源：http://ogj.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jcj.yvedp.cn

[T43] Perl：字符串插值
来源：http://tht.bjfxy.top

"值: $a"
来源：http://odd.316326.xyz

[T44] Perl：条件
来源：http://pkt.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://gdl.cheryme.top

[T45] Perl：数组遍历
来源：http://xgh.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://inh.ehwqpu.com

[T46] Perl：哈希操作
来源：http://xpj.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jwp.yangfankeji.com

[T47] Perl：正则捕获
来源：http://lgc.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://kud.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://jbr.fzhhl.top

$s =~ s/old/new/g;
来源：http://hsk.nanxuanxn.top

[T49] Perl：函数
来源：http://tpl.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qed.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://pcv.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dfi.gogol.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://mbt.gaohongyu789.top

[T51] Scala：Hello World
来源：http://fhf.zhoulong.xyz

println("Hello")
来源：http://cjx.chenlongwang.top

[T52] Scala：变量
来源：http://yzh.cucudq.cn

val a = 1;  var b = 2
来源：http://uog.cucudq.cn

[T53] Scala：字符串插值
来源：http://gsz.cashguo.top

s"值: $b"
来源：http://xhz.yueranfly.top

[T54] Scala：集合映射
来源：http://tuk.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://oxe.tanke756.top

[T55] Scala：集合过滤
来源：http://xbe.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://ctc.ybcxt.top

[T56] Scala：样例类
来源：http://bmd.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://kbw.smart0.xyz

[T57] Scala：模式匹配
来源：http://rfn.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yuk.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://xfv.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://pvc.jianghu66.top

[T59] Scala：循环
来源：http://rwl.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://jhf.hesvh.cn

[T60] Scala：折叠
来源：http://ttc.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uex.xinyue.icu

================================================================================
来源：http://zvr.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://klc.smart0.xyz

================================================================================
来源：http://cjs.fanxiaobao.xyz

[U01] Py：创建虚拟环境
来源：http://djb.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://edk.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://bmy.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wif.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://xnt.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ndb.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://eaf.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lat.fktsv.cn

[U05] Py：列表去重且保序
来源：http://lol.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://mtq.zycfv.cn

[U06] Py：合并两个字典
来源：http://wsh.yvedp.cn

{**a, **b}
来源：http://kdt.cashguo.top

[U07] Py：反转字典键值
来源：http://fdc.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://tck.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://xnu.wangdashe.top

[y for x in nested for y in x]
来源：http://uvy.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://emj.kuanghao11.cn

max(d, key=d.get)
来源：http://hks.vehdjk.com

[U10] Py：按值排序字典
来源：http://bhd.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jjz.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://lkr.sxryk.cn

(x * 2 for x in arr)
来源：http://djs.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kne.jinqigfzy.top

Counter(arr).most_common(3)
来源：http://wne.tian-w.cn

[U13] Py：固定长度队列
来源：http://ust.sufxvd.cn

deque(maxlen=10)
来源：http://rng.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://fem.hnxiangtu.top

defaultdict(list)
来源：http://ywe.c1oappe.top

[U15] Py：高精度计时
来源：http://qzw.ctjpmb.com

t = time.perf_counter()
来源：http://stt.quarkkingdee.top

[U16] Py：命令行参数解析
来源：http://sih.cheryme.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rvl.xuanzx.com

[U17] Py：初始化日志
来源：http://gbe.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://odp.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://kvx.mhx1999.top

pat = re.compile(r"\d+")
来源：http://udz.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://pfz.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jhq.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://gto.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://fpj.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://qjp.guowangkeji.top

@contextlib.contextmanager
来源：http://amu.birdmap.top

[U22] Py：矩阵转置
来源：http://cak.shzxlz.cn

list(zip(*m))
来源：http://stx.yuxming.cn

[U23] Py：分块读取大文件
来源：http://sty.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pgg.redwolf501.top

[U24] Py：路径操作
来源：http://kdk.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://shx.xylfe.cn

[U25] Py：CSV 按字典读
来源：http://jlm.hywenlv.cn

csv.DictReader(f)
来源：http://kyx.hnxiangtu.top

[U26] Py：并发下载
来源：http://swv.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vju.pycfn.com

[U27] Py：异步 HTTP
来源：http://ney.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://tqq.zhixingplan.top

[U28] Py：类型别名
来源：http://nmz.jianghu66.top

UserId = int
来源：http://hqw.jiagoushi.top

[U29] Py：属性校验
来源：http://bck.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://gsq.shangyingyoupin.top

[U30] Py：数据类
来源：http://pte.cucudq.cn

@dataclass(slots=True)
来源：http://uce.ywan-chungtsiang.top

[U31] Py：单测
来源：http://wfv.jqgufenzy.top

python -m pytest -q
来源：http://zjc.ehwqpu.com

[U32] Py：代码格式化
来源：http://jcv.fengsongda.top

ruff format . && ruff check --fix .
来源：http://ihs.gaohongyu789.top

[U33] Py：打包发布
来源：http://vlw.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://dkx.redwolf501.top

[U34] Py：判断编码
来源：http://rvx.sxryk.cn

chardet.detect(raw)
来源：http://lrk.ydjk.org.cn

[U35] Py：发送邮件
来源：http://ulk.yongpay.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cev.bjfxy.top

[U36] Py：定时任务
来源：http://yxk.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://ell.yangfankeji.com

[U37] Py：读写 Excel
来源：http://lpy.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://gup.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://vkk.xziqi.cn

Path(__file__).resolve().parent
来源：http://mws.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://oxe.epnwcf.com

sys.stdout.isatty()
来源：http://pzh.havefunace.top

[U40] Py：打印到标准错误
来源：http://xrt.smart0.xyz

print("err", file=sys.stderr)
来源：http://crb.ydjk.org.cn

[U41] PHP：初始化 Composer 项目
来源：http://fhy.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xxp.fanxiaobao.xyz

[U42] PHP：PSR-4 自动加载
来源：http://lad.shuidangran.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zuk.yanxiufei.cn

[U43] PHP：声明命名空间
来源：http://bgg.bbcook.cn

namespace App\Http;
来源：http://ktw.jianghu66.top

[U44] PHP：开启严格类型
来源：http://ysz.zdbjq.cn

declare(strict_types=1);
来源：http://jff.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://wdq.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://qau.feifeiyinyue.top

[U46] PHP：可空类型
来源：http://qzj.nwbrower.top

?string $name = null
来源：http://gvd.yangfankeji.com

[U47] PHP：联合类型
来源：http://wll.cdnleiting.top

int|string $id
来源：http://vof.fanxiaobao.xyz

[U48] PHP：纯枚举
来源：http://zkz.tianlin.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cfl.ybcxt.top

[U49] PHP：只读属性
来源：http://dbi.shanyushiyangkeji.top

public readonly string $name
来源：http://bmn.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://kzt.hfpthk.cn

public function __construct(private int $id) {}
来源：http://eze.smart0.xyz

[U51] PHP：数组解构
来源：http://hpr.gaohongyu789.top

[$a, $b] = $arr;
来源：http://tff.smart0.xyz

[U52] PHP：箭头函数
来源：http://vlk.ivvv.top

$double = fn($x) => $x * 2;
来源：http://ifw.ydzc1.top

[U53] PHP：空合并运算符
来源：http://zxq.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://gno.xinyue.icu

[U54] PHP：空安全调用
来源：http://nrg.sufxvd.cn

$obj?->method()
来源：http://zkd.yvedp.cn

[U55] PHP：match 表达式
来源：http://lle.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mxl.jlsjyb.cn

[U56] PHP：命名参数
来源：http://jwl.sufxvd.cn

f(a: 1, b: 2)
来源：http://bpa.pycfn.com

[U57] PHP：字符串插值
来源：http://kwr.gogol.net.cn

"值: {$a}"
来源：http://bql.zhengqikj.top

[U58] PHP：数组三件套
来源：http://lbt.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hpb.bbcook.cn


<!-- 参考信息 -->