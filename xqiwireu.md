代发 wailian999

memset(a, 0, sizeof a);
来源：http://wfu.cucudq.cn

[S27] C：定义常量
来源：http://pbz.chenlongwang.top

const double PI = 3.14159;
来源：http://xza.svipenyu.cn

[S28] C：静态变量
来源：http://zwe.hywenlv.cn

static int counter = 0;
来源：http://xyc.yuanzhike.top

[S29] C：变参函数
来源：http://wsp.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lip.wangdashe.top

[S30] C：头文件保护
来源：http://xtn.wangshuangyany.cn

#ifndef X_H
来源：http://jcf.sjlbkw.cn

#define X_H
来源：http://grx.epnwcf.com

#endif
来源：http://muv.nanxinkj.top

[S31] C++：Hello World
来源：http://cmb.xuanzx.com

#include <iostream>
来源：http://fre.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://hbv.c1oappe.top

[S32] C++：字符串
来源：http://mlz.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://aig.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://ilr.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kef.cucudq.cn

[S34] C++：遍历 vector
来源：http://gxj.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://hha.yj20258.top

[S35] C++：map
来源：http://oir.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fwi.nwbrower.top

[S36] C++：unordered_map
来源：http://ifd.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vjx.iojbl.cn

[S37] C++：set
来源：http://mvx.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ouu.jinqigfzy.top

[S38] C++：排序
来源：http://qus.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://ilm.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://fpe.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://liq.hammf.cn

[S40] C++：查找元素
来源：http://pfo.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ean.0kj1m.cn

[S41] C++：类与构造函数
来源：http://bch.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wpl.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://pma.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://ewn.jlsjyb.cn

[S43] C++：智能指针
来源：http://lok.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://uov.yueranfly.top

[S44] C++：引用传参
来源：http://zpq.jinghuilouyu.cn

void inc(int &x) { ++x; }
来源：http://hye.yueranfly.top

[S45] C++：lambda
来源：http://kyo.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://gnk.guowangkeji.top

[S46] C++：函数模板
来源：http://wdo.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hjx.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://uyi.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vej.zdqjudy.top

[S48] C++：逐行读文件
来源：http://knb.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://lol.uphjek.com

while (std::getline(in, line)) { }
来源：http://ktl.fzhhl.top

[S49] C++：写文件
来源：http://flb.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pci.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://xdo.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bcl.fehbvm.com

[S51] C++：显式类型转换
来源：http://pdl.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://ozr.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://hav.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://wcp.fzhhl.top

[S53] C++：移动语义
来源：http://dpm.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://hlh.yuxming.cn

[S54] C++：异常处理
来源：http://yxj.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fla.ybcxt.top

[S55] C++：结构化绑定
来源：http://zbz.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://uub.jqgufenzy.top

[S56] C++：optional
来源：http://ulx.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hyk.gzhubu.top

[S57] C++：编译期常量
来源：http://mez.shuidangran.top

constexpr int N = 10;
来源：http://msa.jiagoushi.top

[S58] C++：命名空间
来源：http://jbn.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://cjx.jiagoushi.top

[S59] C++：静态断言
来源：http://kph.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://clq.jqgfzy.top

[S60] C++：遍历并删除元素
来源：http://hpu.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kav.meibo888.top

================================================================================
来源：http://nmu.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://onh.xinyue.icu

================================================================================
来源：http://ckp.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://tus.sjlbkw.cn

println("Hello")
来源：http://rqv.pycfn.com

[T02] Kotlin：变量
来源：http://elm.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hme.cashguo.top

[T03] Kotlin：字符串模板
来源：http://ywc.ehwqpu.com

"值: $b"
来源：http://qbs.aizwys.cn

[T04] Kotlin：空安全
来源：http://arp.birdmap.top

val n: String? = null;  n?.length
来源：http://ivq.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://gdg.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cpj.jianghu66.top

[T06] Kotlin：集合映射
来源：http://spq.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dqx.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://wkf.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://opb.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://owf.tanke756.top

data class User(val name: String, val age: Int)
来源：http://kux.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://psm.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://rqy.iojbl.cn

[T10] Kotlin：默认参数
来源：http://wti.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://cnp.hnxiangtu.top

[T11] Kotlin：协程
来源：http://och.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nrw.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://wjd.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://xkw.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://kty.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://uap.bjfxy.top

[T14] Kotlin：循环
来源：http://zpr.sweek.top

for (i in 1..10) println(i)
来源：http://scu.gotoacloud.top

[T15] Kotlin：接口
来源：http://cyg.redwolf501.top

interface Shape { fun area(): Double }
来源：http://njj.tian-w.cn

[T16] Swift：Hello World
来源：http://nac.kuanghao11.cn

print("Hello")
来源：http://ouw.wangdashe.top

[T17] Swift：变量与常量
来源：http://eeh.havefunace.top

var a = 1;  let b = 2
来源：http://oxb.daria6918.cn

[T18] Swift：字符串插值
来源：http://kbh.guowangkeji.top

"值: \(b)"
来源：http://qui.kuanghao11.cn

[T19] Swift：可选绑定
来源：http://ijh.zdqjudy.top

if let n = opt { print(n) }
来源：http://dhm.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://xnr.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://cti.hcnkem.com

[T21] Swift：遍历
来源：http://gfk.yj202588.top

for x in a { print(x) }
来源：http://eib.ivvv.top

[T22] Swift：字典
来源：http://tdc.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://hwl.sjlbkw.cn

[T23] Swift：函数
来源：http://obl.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rwx.guannengcc.top

[T24] Swift：闭包
来源：http://mub.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qsx.yanxiufei.cn

[T25] Swift：结构体
来源：http://qwy.cucudq.cn

struct P { var x: Int }
来源：http://svt.zycfv.cn

[T26] Swift：类与重写
来源：http://zgu.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://dzt.uphjek.com

[T27] Swift：错误处理
来源：http://wvg.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://bbi.bjfxy.top

[T28] Swift：枚举
来源：http://rso.dianchejie.cn

enum Color { case red, green }
来源：http://lbd.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://yly.nanxinkj.top

guard let x = opt else { return }
来源：http://kxp.cdnleiting.top

[T30] Swift：协议
来源：http://thx.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://vfh.gzhubu.top

[T31] Lua：Hello World
来源：http://lwz.zhixingplan.top

print("Hello")
来源：http://oud.hfpthk.cn

[T32] Lua：局部变量
来源：http://dgq.shuidangran.top

local a = 1
来源：http://yns.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://yys.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zmt.fengsongda.top

[T34] Lua：遍历表
来源：http://wra.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kdq.9152youxi.cn

[T35] Lua：字典表
来源：http://egm.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://xun.jinghuilouyu.cn

[T36] Lua：函数
来源：http://vyt.yangfankeji.com

function add(a, b) return a + b end
来源：http://ahq.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://qif.kuanghao11.cn

"a" .. "b"
来源：http://nad.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://nol.316326.xyz

if x > 0 then print("正") end
来源：http://nqm.kuanghao11.cn

[T39] Lua：模式匹配
来源：http://elz.sweek.top

string.find(s, "%d+")
来源：http://sxy.gaohongyu789.top

[T40] Lua：元表
来源：http://bel.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://ycz.jinqigfzy.top

[T41] Perl：Hello World
来源：http://faz.cashguo.top

print "Hello\n";
来源：http://pti.sxryk.cn

[T42] Perl：变量类型
来源：http://ycd.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dqo.tianlin.xyz

[T43] Perl：字符串插值
来源：http://qms.birdmap.top

"值: $a"
来源：http://lmt.hcnkem.com

[T44] Perl：条件
来源：http://mvo.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://ujy.ivvv.top

[T45] Perl：数组遍历
来源：http://gaz.ehwqpu.com

for my $x (@arr) { print $x; }
来源：http://dlf.hammf.cn

[T46] Perl：哈希操作
来源：http://huz.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bws.andypj.xyz

[T47] Perl：正则捕获
来源：http://rsp.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://hbp.snrcjt.cn

[T48] Perl：正则替换
来源：http://odg.nanxuanxn.top

$s =~ s/old/new/g;
来源：http://zxy.shangyingyoupin.top

[T49] Perl：函数
来源：http://dou.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dlf.sufxvd.cn

[T50] Perl：逐行读文件
来源：http://ckc.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://skz.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://pfh.pycfn.com

[T51] Scala：Hello World
来源：http://wlu.haohaochexian.top

println("Hello")
来源：http://ojt.iojbl.cn

[T52] Scala：变量
来源：http://cth.gaohongyu789.top

val a = 1;  var b = 2
来源：http://gdz.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://srz.tianlin.xyz

s"值: $b"
来源：http://uxy.ybcxt.top

[T54] Scala：集合映射
来源：http://tmc.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://tmq.andypj.xyz

[T55] Scala：集合过滤
来源：http://juh.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dse.jqgfzy.top

[T56] Scala：样例类
来源：http://uhp.xinyue.icu

case class User(name: String, age: Int)
来源：http://tyw.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://ksu.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://bgf.kuanghao11.cn

[T58] Scala：函数定义
来源：http://axz.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://jvp.sufxvd.cn

[T59] Scala：循环
来源：http://zmu.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://gdc.tarul.cn

[T60] Scala：折叠
来源：http://shx.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ksv.bbcook.cn

================================================================================
来源：http://mae.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vnl.pengpengdd.cyou

================================================================================
来源：http://hhj.sweek.top

[U01] Py：创建虚拟环境
来源：http://ory.shanyushiyangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://fja.cashguo.top

[U02] Py：导出 / 安装依赖
来源：http://niz.jinghuilouyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yet.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://thv.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vxw.hysaishi.cn

[U04] Py：变量调试打印
来源：http://tqv.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ycn.yongpay.top

[U05] Py：列表去重且保序
来源：http://lkn.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://swc.gzhubu.top

[U06] Py：合并两个字典
来源：http://ybo.pengpengdd.cyou

{**a, **b}
来源：http://por.snrcjt.cn

[U07] Py：反转字典键值
来源：http://tus.andypj.xyz

{v: k for k, v in d.items()}
来源：http://eua.ivvv.top

[U08] Py：展平二维列表
来源：http://lrp.mhx1999.top

[y for x in nested for y in x]
来源：http://xya.yonumen.top

[U09] Py：字典取最大值的键
来源：http://ydk.hywenlv.cn

max(d, key=d.get)
来源：http://idg.zhengqikj.top

[U10] Py：按值排序字典
来源：http://jpn.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iwb.hysaishi.cn

[U11] Py：生成器表达式
来源：http://ulb.hcnkem.com

(x * 2 for x in arr)
来源：http://ttj.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://crb.daxiang520.top

Counter(arr).most_common(3)
来源：http://ceh.sweek.top

[U13] Py：固定长度队列
来源：http://jce.bjfxy.top

deque(maxlen=10)
来源：http://xbo.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://sgo.jinyuanbaomall.cn

defaultdict(list)
来源：http://oei.zhixingplan.top

[U15] Py：高精度计时
来源：http://tka.nanxinkj.top

t = time.perf_counter()
来源：http://pwd.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://qkf.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cec.yangfankeji.com

[U17] Py：初始化日志
来源：http://spw.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://bhm.zdqjudy.top

[U18] Py：预编译正则
来源：http://pin.tarul.cn

pat = re.compile(r"\d+")
来源：http://hti.bjfxy.top

[U19] Py：正则替换带回调
来源：http://gqo.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dns.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://njn.fengsongda.top

@functools.lru_cache(maxsize=None)
来源：http://dte.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://tmx.shuidangran.top

@contextlib.contextmanager
来源：http://aoe.fehbvm.com

[U22] Py：矩阵转置
来源：http://dgq.cheryme.top

list(zip(*m))
来源：http://jtm.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://omz.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oeg.hnxiangtu.top

[U24] Py：路径操作
来源：http://zcc.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ocv.shanyushiyangtech.top

[U25] Py：CSV 按字典读
来源：http://hsx.316326.xyz

csv.DictReader(f)
来源：http://jtk.nanxinkj.top

[U26] Py：并发下载
来源：http://jfe.jlsjyb.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vuu.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://aef.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://pku.hywenlv.cn

[U28] Py：类型别名
来源：http://uel.yuxming.cn

UserId = int
来源：http://zym.tanke756.top

[U29] Py：属性校验
来源：http://qzp.tianlin.xyz

@property 与 @x.setter 配合
来源：http://spt.guowangkeji.top

[U30] Py：数据类
来源：http://xzp.svipenyu.cn

@dataclass(slots=True)
来源：http://psb.fehbvm.com

[U31] Py：单测
来源：http://mzi.fktsv.cn

python -m pytest -q
来源：http://uwn.316326.xyz

[U32] Py：代码格式化
来源：http://xkp.xuanzx.com

ruff format . && ruff check --fix .
来源：http://pjr.shuidangran.top

[U33] Py：打包发布
来源：http://pkr.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://xen.shangyingyoupin.top

[U34] Py：判断编码
来源：http://hvm.zhixingplan.top

chardet.detect(raw)
来源：http://veq.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://tcw.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ahz.xylfe.cn

[U36] Py：定时任务
来源：http://ijz.cucudq.cn

schedule.every(10).minutes.do(job)
来源：http://wjj.hesvh.cn

[U37] Py：读写 Excel
来源：http://frb.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://tss.jinghuilouyu.cn

[U38] Py：获取脚本所在目录
来源：http://ysx.316326.xyz

Path(__file__).resolve().parent
来源：http://eud.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://jpf.xylfe.cn

sys.stdout.isatty()
来源：http://ite.fktsv.cn

[U40] Py：打印到标准错误
来源：http://ydq.cucudq.cn

print("err", file=sys.stderr)
来源：http://vop.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://xpg.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kmh.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://kgf.hongshengwenyu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xtd.c1oappe.top

[U43] PHP：声明命名空间
来源：http://dlz.jinqigfzy.top

namespace App\Http;
来源：http://yun.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://kfr.wangdashe.top

declare(strict_types=1);
来源：http://kxa.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://ssy.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mfn.yuxming.cn

[U46] PHP：可空类型
来源：http://yso.hnxiangtu.top

?string $name = null
来源：http://pxq.fehbvm.com

[U47] PHP：联合类型
来源：http://huk.birdmap.top

int|string $id
来源：http://ljk.jqgfzy.top

[U48] PHP：纯枚举
来源：http://bok.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kws.cheryme.top

[U49] PHP：只读属性
来源：http://xbh.chenlongwang.top

public readonly string $name
来源：http://nix.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://kdj.birdmap.top

public function __construct(private int $id) {}
来源：http://tem.yuxming.cn


<!-- 参考信息 -->