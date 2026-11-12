代发 wailian999

[S33] C++：vector 增删
来源：http://jye.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tpa.cashguo.top

[S34] C++：遍历 vector
来源：http://aem.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://zuo.hesvh.cn

[S35] C++：map
来源：http://hks.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dke.guannengcc.top

[S36] C++：unordered_map
来源：http://mzp.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wlq.sweek.top

[S37] C++：set
来源：http://roq.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fty.0kj1m.cn

[S38] C++：排序
来源：http://vif.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://nqf.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://soe.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bsv.hammf.cn

[S40] C++：查找元素
来源：http://sye.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cad.fehbvm.com

[S41] C++：类与构造函数
来源：http://kdt.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vwm.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://pml.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://pkm.bbcook.cn

[S43] C++：智能指针
来源：http://sdl.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://hgd.yj202588.top

[S44] C++：引用传参
来源：http://czg.iojbl.cn

void inc(int &x) { ++x; }
来源：http://agi.iojbl.cn

[S45] C++：lambda
来源：http://all.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://tkr.chenlongwang.top

[S46] C++：函数模板
来源：http://npw.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xdu.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://ggg.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dnz.shzxlz.cn

[S48] C++：逐行读文件
来源：http://inn.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://rle.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://uhg.gogol.net.cn

[S49] C++：写文件
来源：http://gns.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dty.chenzaomai.com

[S50] C++：格式化数字
来源：http://rqp.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aeg.xuanzx.com

[S51] C++：显式类型转换
来源：http://cke.yj20258.top

static_cast<double>(a) / b
来源：http://zfc.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://laq.yj20258888.top

int size() const noexcept { return n_; }
来源：http://bzk.yfazqb.com

[S53] C++：移动语义
来源：http://fjf.birdmap.top

std::vector<int> w = std::move(v);
来源：http://bip.guannengcc.top

[S54] C++：异常处理
来源：http://qfx.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bmu.yuxming.cn

[S55] C++：结构化绑定
来源：http://ytp.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ojx.jinqigufen.top

[S56] C++：optional
来源：http://qmq.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qrx.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://jhd.pycfn.com

constexpr int N = 10;
来源：http://zdz.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://fis.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://qkc.52xcode.cn

[S59] C++：静态断言
来源：http://ubf.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ivh.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://mws.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://smj.jqgufenzy.top

================================================================================
来源：http://bmy.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zfx.fehbvm.com

================================================================================
来源：http://jcv.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://cdc.smart0.xyz

println("Hello")
来源：http://nmx.daxiang520.top

[T02] Kotlin：变量
来源：http://did.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zzq.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://yqn.shanyushiyangkeji.top

"值: $b"
来源：http://dkm.daxiang520.top

[T04] Kotlin：空安全
来源：http://ahp.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://dhl.cheryme.top

[T05] Kotlin：when 表达式
来源：http://nvx.andypj.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rsc.xziqi.cn

[T06] Kotlin：集合映射
来源：http://rvw.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pvl.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://hvr.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ora.sxryk.cn

[T08] Kotlin：数据类
来源：http://wip.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://gzr.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://bxn.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://ahc.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://zhr.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://phd.nanxuanxn.top

[T11] Kotlin：协程
来源：http://cyc.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pow.gzhubu.top

[T12] Kotlin：解构声明
来源：http://bsx.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://qgg.316326.xyz

[T13] Kotlin：只读 Map
来源：http://knc.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://ieu.tanke756.top

[T14] Kotlin：循环
来源：http://ets.snrcjt.cn

for (i in 1..10) println(i)
来源：http://gjo.zhixingplan.top

[T15] Kotlin：接口
来源：http://mmc.meibo888.top

interface Shape { fun area(): Double }
来源：http://hac.bbcook.cn

[T16] Swift：Hello World
来源：http://pfc.feifeiyinyue.top

print("Hello")
来源：http://bvk.zdqjudy.top

[T17] Swift：变量与常量
来源：http://eew.hesvh.cn

var a = 1;  let b = 2
来源：http://tbg.guannengcc.top

[T18] Swift：字符串插值
来源：http://niu.yueranfly.top

"值: \(b)"
来源：http://yph.ivvv.top

[T19] Swift：可选绑定
来源：http://hqh.c1oappe.top

if let n = opt { print(n) }
来源：http://urw.zycfv.cn

[T20] Swift：数组操作
来源：http://oij.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://xoi.hongshengwenyu.top

[T21] Swift：遍历
来源：http://nmq.ydjk.org.cn

for x in a { print(x) }
来源：http://lio.nanxinkj.top

[T22] Swift：字典
来源：http://cph.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://ssz.iojbl.cn

[T23] Swift：函数
来源：http://jaw.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bzq.hammf.cn

[T24] Swift：闭包
来源：http://ylu.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cse.cucudq.cn

[T25] Swift：结构体
来源：http://luw.yueranfly.top

struct P { var x: Int }
来源：http://zfj.bbcook.cn

[T26] Swift：类与重写
来源：http://abt.havefunace.top

class A: Base { override func f() {} }
来源：http://ffv.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://oem.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://mmz.haohaochexian.top

[T28] Swift：枚举
来源：http://gty.mhx1999.top

enum Color { case red, green }
来源：http://xrk.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://zbu.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://bmm.xylfe.cn

[T30] Swift：协议
来源：http://wya.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://cah.yanxiufei.cn

[T31] Lua：Hello World
来源：http://syr.hfpthk.cn

print("Hello")
来源：http://htg.dianchejie.cn

[T32] Lua：局部变量
来源：http://bqq.hammf.cn

local a = 1
来源：http://epz.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://mzm.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gpt.cheryme.top

[T34] Lua：遍历表
来源：http://qgo.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mof.smart0.xyz

[T35] Lua：字典表
来源：http://skq.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://frz.yvedp.cn

[T36] Lua：函数
来源：http://jhq.quarkkingdee.top

function add(a, b) return a + b end
来源：http://hhv.yonumen.top

[T37] Lua：字符串拼接
来源：http://bbu.jqgufenzy.top

"a" .. "b"
来源：http://kgb.hywenlv.cn

[T38] Lua：条件
来源：http://nux.jqgfzy.top

if x > 0 then print("正") end
来源：http://btx.yj20258888.top

[T39] Lua：模式匹配
来源：http://nac.pycfn.com

string.find(s, "%d+")
来源：http://ijm.zhijiandao.cn

[T40] Lua：元表
来源：http://gff.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://ypv.yj202588.top

[T41] Perl：Hello World
来源：http://svp.fktsv.cn

print "Hello\n";
来源：http://qhr.hcnkem.com

[T42] Perl：变量类型
来源：http://ggz.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ezm.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://rum.zhoulong.xyz

"值: $a"
来源：http://kyf.c1oappe.top

[T44] Perl：条件
来源：http://hwr.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://wwz.yfazqb.com

[T45] Perl：数组遍历
来源：http://lcz.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://vhj.shzxlz.cn

[T46] Perl：哈希操作
来源：http://pql.hammf.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cgr.quarkkingdee.top

[T47] Perl：正则捕获
来源：http://jzi.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zml.cheryme.top

[T48] Perl：正则替换
来源：http://hgr.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://yth.yongpay.top

[T49] Perl：函数
来源：http://dud.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://soj.guannengcc.top

[T50] Perl：逐行读文件
来源：http://epp.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://oxi.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://nza.redwolf501.top

[T51] Scala：Hello World
来源：http://qsj.sweek.top

println("Hello")
来源：http://sdy.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://pin.sxryk.cn

val a = 1;  var b = 2
来源：http://oji.ctjpmb.com

[T53] Scala：字符串插值
来源：http://roq.fanxiaobao.xyz

s"值: $b"
来源：http://txw.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://hec.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://mlh.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://bwm.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://kul.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://oiy.fengsongda.top

case class User(name: String, age: Int)
来源：http://pwh.jyoumei.cn

[T57] Scala：模式匹配
来源：http://ins.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://swb.yongpay.top

[T58] Scala：函数定义
来源：http://lno.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yvu.shzxlz.cn

[T59] Scala：循环
来源：http://dmp.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://zrz.jlsjyb.cn

[T60] Scala：折叠
来源：http://kkp.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nrj.shanyushiyangtech.top

================================================================================
来源：http://cwd.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rzv.xuanzx.com

================================================================================
来源：http://hzn.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://vcm.andypj.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://iiq.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://vql.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aji.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://rtf.sweek.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mkf.ybcxt.top

[U04] Py：变量调试打印
来源：http://zmp.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cfe.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://owm.sweek.top

list(dict.fromkeys(arr))
来源：http://mlf.hywenlv.cn

[U06] Py：合并两个字典
来源：http://par.jiagoushi.top

{**a, **b}
来源：http://dhk.vehdjk.com

[U07] Py：反转字典键值
来源：http://nmk.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://jhn.sysykeji.top

[U08] Py：展平二维列表
来源：http://fsn.xylfe.cn

[y for x in nested for y in x]
来源：http://oee.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://qbh.shzxlz.cn

max(d, key=d.get)
来源：http://qta.snrcjt.cn

[U10] Py：按值排序字典
来源：http://hfe.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tqm.yuxming.cn

[U11] Py：生成器表达式
来源：http://qah.yongpay.top

(x * 2 for x in arr)
来源：http://rzv.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://joh.dianchejie.cn

Counter(arr).most_common(3)
来源：http://iaw.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://evl.ppjwa.cn

deque(maxlen=10)
来源：http://xsk.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://zjt.dianchejie.cn

defaultdict(list)
来源：http://tzt.meibo888.top

[U15] Py：高精度计时
来源：http://wld.yj20258888.top

t = time.perf_counter()
来源：http://cpl.yj20258888.top

[U16] Py：命令行参数解析
来源：http://zrn.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wbv.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://jvi.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://tew.ivvv.top

[U18] Py：预编译正则
来源：http://gmf.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://mvy.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://iiz.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bus.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://inp.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://ffc.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://vnn.feifeiyinyue.top

@contextlib.contextmanager
来源：http://pjc.shuidangran.top

[U22] Py：矩阵转置
来源：http://qiv.316326.xyz

list(zip(*m))
来源：http://afb.yangfankeji.com

[U23] Py：分块读取大文件
来源：http://wzc.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wzp.fktsv.cn

[U24] Py：路径操作
来源：http://myi.jinqigfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fnf.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://meu.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://zwl.bjfxy.top

[U26] Py：并发下载
来源：http://bef.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uug.yonumen.top

[U27] Py：异步 HTTP
来源：http://rcw.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://dek.aizwys.cn

[U28] Py：类型别名
来源：http://zwo.hywenlv.cn

UserId = int
来源：http://cga.zhiwuduotai.top

[U29] Py：属性校验
来源：http://gyi.bbcook.cn

@property 与 @x.setter 配合
来源：http://ebg.tianlin.xyz

[U30] Py：数据类
来源：http://chp.guannengcc.top

@dataclass(slots=True)
来源：http://ziw.nanxuanxn.top

[U31] Py：单测
来源：http://dkd.jinqigfzy.top

python -m pytest -q
来源：http://cgy.sjlbkw.cn

[U32] Py：代码格式化
来源：http://eff.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://rlb.ybcxt.top

[U33] Py：打包发布
来源：http://dwq.aizwys.cn

python -m build  （依赖 pyproject.toml）
来源：http://nte.andypj.xyz

[U34] Py：判断编码
来源：http://brb.tanke756.top

chardet.detect(raw)
来源：http://vfv.ivvv.top

[U35] Py：发送邮件
来源：http://jqc.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lyk.zdbjq.cn

[U36] Py：定时任务
来源：http://vxu.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://rmt.shzxlz.cn

[U37] Py：读写 Excel
来源：http://moy.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://ewx.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://rkl.52xcode.cn

Path(__file__).resolve().parent
来源：http://wzx.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://axc.tarul.cn

sys.stdout.isatty()
来源：http://nro.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://aqz.gotoacloud.top

print("err", file=sys.stderr)
来源：http://bjl.fzhhl.top

[U41] PHP：初始化 Composer 项目
来源：http://dhj.shangyingyoupin.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nyw.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://rmp.haohaochexian.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://syp.nanxinkj.top

[U43] PHP：声明命名空间
来源：http://jqd.hysaishi.cn

namespace App\Http;
来源：http://zjt.tarul.cn

[U44] PHP：开启严格类型
来源：http://elb.yangfankeji.com

declare(strict_types=1);
来源：http://xfb.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://xhk.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jht.smart0.xyz

[U46] PHP：可空类型
来源：http://wuf.jqgufenzy.top

?string $name = null
来源：http://qvr.yvedp.cn

[U47] PHP：联合类型
来源：http://yly.jinyuanbaomall.cn

int|string $id
来源：http://vvu.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://soo.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nju.hesvh.cn

[U49] PHP：只读属性
来源：http://dje.cdnleiting.top

public readonly string $name
来源：http://gzj.ctjpmb.com

[U50] PHP：构造器属性提升
来源：http://efz.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://zig.yanxiufei.cn

[U51] PHP：数组解构
来源：http://oba.snrcjt.cn

[$a, $b] = $arr;
来源：http://bha.daria6918.cn

[U52] PHP：箭头函数
来源：http://cyi.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://kiw.daxiang520.top

[U53] PHP：空合并运算符
来源：http://mnn.jinqigfzy.top

$v = $a ?? $b ?? "default";
来源：http://yir.haohaochexian.top

[U54] PHP：空安全调用
来源：http://cwc.aibaodan.cn

$obj?->method()
来源：http://kmc.dashuyun.cn

[U55] PHP：match 表达式
来源：http://dow.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vqn.fengsongda.top

[U56] PHP：命名参数
来源：http://glb.52xcode.cn

f(a: 1, b: 2)
来源：http://ikl.yonumen.top

[U57] PHP：字符串插值
来源：http://nea.xziqi.cn

"值: {$a}"
来源：http://eyq.fanxiaobao.xyz

[U58] PHP：数组三件套
来源：http://hgo.9152youxi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rhd.bbcook.cn


<!-- 参考信息 -->