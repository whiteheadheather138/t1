代发 wailian999

int main(int argc, char **argv)
来源：http://kci.chenjidiqi.icu

[S19] C：快速排序
来源：http://chn.yangfankeji.com

qsort(a, n, sizeof(int), cmp);
来源：http://vlz.fzhhl.top

[S20] C：二分查找
来源：http://uyf.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://usu.zhoulong.xyz

[S21] C：字符类别判断
来源：http://tlp.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ikt.zdbjq.cn

[S22] C：字符串转数字
来源：http://nen.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://wje.redwolf501.top

[S23] C：随机数
来源：http://zct.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nhy.guowangkeji.top

[S24] C：获取本地时间
来源：http://che.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jsr.ivvv.top

[S25] C：内存拷贝
来源：http://sjz.smart0.xyz

memcpy(dst, src, n);
来源：http://wnz.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://baz.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://amz.fzhhl.top

[S27] C：定义常量
来源：http://jjg.yj20258888.top

const double PI = 3.14159;
来源：http://kmn.chenjidiqi.icu

[S28] C：静态变量
来源：http://dpz.yueranfly.top

static int counter = 0;
来源：http://pxn.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://eeq.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qon.yanxiufei.cn

[S30] C：头文件保护
来源：http://frg.cdnleiting.top

#ifndef X_H
来源：http://cfs.tanke756.top

#define X_H
来源：http://vfl.fengsongda.top

#endif
来源：http://cjz.andypj.xyz

[S31] C++：Hello World
来源：http://dft.shanyushiyangkeji.top

#include <iostream>
来源：http://amo.zhixingplan.top

int main() { std::cout << "Hello\n"; }
来源：http://zny.vehdjk.com

[S32] C++：字符串
来源：http://pci.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://awn.aibaodan.cn

[S33] C++：vector 增删
来源：http://seg.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ihh.52xcode.cn

[S34] C++：遍历 vector
来源：http://cnn.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://yrz.chenzaomai.com

[S35] C++：map
来源：http://slx.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kkm.sjlbkw.cn

[S36] C++：unordered_map
来源：http://uqj.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://erj.yanxiufei.cn

[S37] C++：set
来源：http://zej.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pih.52xcode.cn

[S38] C++：排序
来源：http://jvt.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://owh.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://bhj.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nzx.zycfv.cn

[S40] C++：查找元素
来源：http://itp.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fhm.bbcook.cn

[S41] C++：类与构造函数
来源：http://hch.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cig.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://aom.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://vjf.tanke756.top

[S43] C++：智能指针
来源：http://ofi.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://eqj.wangdashe.top

[S44] C++：引用传参
来源：http://icf.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://dpg.zhengqikj.top

[S45] C++：lambda
来源：http://kmn.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://toq.zhoulong.xyz

[S46] C++：函数模板
来源：http://twz.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hyp.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://dlj.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lhi.fzhhl.top

[S48] C++：逐行读文件
来源：http://igm.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://twy.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://qab.yj202588.top

[S49] C++：写文件
来源：http://udg.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wlb.sweek.top

[S50] C++：格式化数字
来源：http://zlx.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fbs.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://iss.kuanghao11.cn

static_cast<double>(a) / b
来源：http://asq.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://ctw.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://dih.zhiwuduotai.top

[S53] C++：移动语义
来源：http://xyb.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://elj.aibaodan.cn

[S54] C++：异常处理
来源：http://hby.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lyz.ctjpmb.com

[S55] C++：结构化绑定
来源：http://ojr.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wgf.vehdjk.com

[S56] C++：optional
来源：http://hnl.fehbvm.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yyz.gzhubu.top

[S57] C++：编译期常量
来源：http://gtm.zhixingplan.top

constexpr int N = 10;
来源：http://por.zhixingplan.top

[S58] C++：命名空间
来源：http://blm.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://vgu.xylfe.cn

[S59] C++：静态断言
来源：http://jfy.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uug.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://zai.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://exf.kuanghao11.cn

================================================================================
来源：http://goc.dianchejie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ayl.svipenyu.cn

================================================================================
来源：http://cnf.yonumen.top

[T01] Kotlin：Hello World
来源：http://opb.jiagoushi.top

println("Hello")
来源：http://uyx.epnwcf.com

[T02] Kotlin：变量
来源：http://gre.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://prf.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://api.shanyushiyangkeji.top

"值: $b"
来源：http://dih.daxiang520.top

[T04] Kotlin：空安全
来源：http://fuq.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://nxz.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://oew.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lpz.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://lve.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tsv.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://fyy.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ywq.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://fop.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://esi.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://pwi.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://pol.xuetiantiany.cn

[T10] Kotlin：默认参数
来源：http://bud.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://peb.bbcook.cn

[T11] Kotlin：协程
来源：http://qqa.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gtv.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://dse.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://bnb.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://ifm.cashguo.top

val m = mapOf("a" to 1)
来源：http://sfm.jlsjyb.cn

[T14] Kotlin：循环
来源：http://iec.svipenyu.cn

for (i in 1..10) println(i)
来源：http://ira.xziqi.cn

[T15] Kotlin：接口
来源：http://bwa.iojbl.cn

interface Shape { fun area(): Double }
来源：http://cop.aizwys.cn

[T16] Swift：Hello World
来源：http://vix.hysaishi.cn

print("Hello")
来源：http://vtw.guowangkeji.top

[T17] Swift：变量与常量
来源：http://rte.xylfe.cn

var a = 1;  let b = 2
来源：http://bqb.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://hcd.ppjwa.cn

"值: \(b)"
来源：http://mrv.fehbvm.com

[T19] Swift：可选绑定
来源：http://qnm.9152youxi.cn

if let n = opt { print(n) }
来源：http://vys.nanxinkj.top

[T20] Swift：数组操作
来源：http://hcm.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://vsp.hfpthk.cn

[T21] Swift：遍历
来源：http://bba.yfazqb.com

for x in a { print(x) }
来源：http://lan.yueranfly.top

[T22] Swift：字典
来源：http://wyz.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://qgd.pycfn.com

[T23] Swift：函数
来源：http://qxg.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uyo.ehwqpu.com

[T24] Swift：闭包
来源：http://kkw.daxiang520.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pxj.pengpengdd.cyou

[T25] Swift：结构体
来源：http://bjn.havefunace.top

struct P { var x: Int }
来源：http://kpa.cucudq.cn

[T26] Swift：类与重写
来源：http://akp.xuanzx.com

class A: Base { override func f() {} }
来源：http://mhn.vqdsnc.cn

[T27] Swift：错误处理
来源：http://piu.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://noe.vqdsnc.cn

[T28] Swift：枚举
来源：http://nxi.nwbrower.top

enum Color { case red, green }
来源：http://ikw.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://lqm.xingfuxueyuan.xyz

guard let x = opt else { return }
来源：http://pqz.uphjek.com

[T30] Swift：协议
来源：http://sqd.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://kcp.hfpthk.cn

[T31] Lua：Hello World
来源：http://gdo.zycfv.cn

print("Hello")
来源：http://sfq.zdqjudy.top

[T32] Lua：局部变量
来源：http://gfo.gogol.net.cn

local a = 1
来源：http://idh.hammf.cn

[T33] Lua：表（数组）
来源：http://wtp.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://kdv.ppjwa.cn

[T34] Lua：遍历表
来源：http://mib.hywenlv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uyx.sjlbkw.cn

[T35] Lua：字典表
来源：http://kme.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://ghb.tian-w.cn

[T36] Lua：函数
来源：http://tom.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://jer.pycfn.com

[T37] Lua：字符串拼接
来源：http://fmm.epnwcf.com

"a" .. "b"
来源：http://txw.wangdashe.top

[T38] Lua：条件
来源：http://xty.uphjek.com

if x > 0 then print("正") end
来源：http://ezd.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://unt.jqgfzy.top

string.find(s, "%d+")
来源：http://xjt.mhx1999.top

[T40] Lua：元表
来源：http://lae.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://awv.jqgfzy.top

[T41] Perl：Hello World
来源：http://lpx.jqgufenzy.top

print "Hello\n";
来源：http://ecg.zycfv.cn

[T42] Perl：变量类型
来源：http://nxe.svipenyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dja.sweek.top

[T43] Perl：字符串插值
来源：http://knf.nanxuanxn.top

"值: $a"
来源：http://dlo.shanyushiyangtech.top

[T44] Perl：条件
来源：http://adg.fehbvm.com

if ($a > 0) { print "正"; }
来源：http://hyi.tanke756.top

[T45] Perl：数组遍历
来源：http://gph.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://wdh.c1oappe.top

[T46] Perl：哈希操作
来源：http://zws.fzhhl.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nan.ppjwa.cn

[T47] Perl：正则捕获
来源：http://awg.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wqp.hnxiangtu.top

[T48] Perl：正则替换
来源：http://vhs.snrcjt.cn

$s =~ s/old/new/g;
来源：http://odp.nanxinkj.top

[T49] Perl：函数
来源：http://pqr.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://esc.jinqigfzy.top

[T50] Perl：逐行读文件
来源：http://umj.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cpe.wangshuangyany.cn

while (my $line = <$fh>) { print $line; }
来源：http://hgr.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://sou.yfazqb.com

println("Hello")
来源：http://ebp.zhongyouzk.top

[T52] Scala：变量
来源：http://hwo.kuanghao11.cn

val a = 1;  var b = 2
来源：http://mqe.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://owi.xuetiantiany.cn

s"值: $b"
来源：http://jto.bjfxy.top

[T54] Scala：集合映射
来源：http://spi.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://bng.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://flr.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lge.aizwys.cn

[T56] Scala：样例类
来源：http://nzu.zycfv.cn

case class User(name: String, age: Int)
来源：http://xsg.daxiang520.top

[T57] Scala：模式匹配
来源：http://iis.nanxinkj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ehl.cheryme.top

[T58] Scala：函数定义
来源：http://jol.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ocs.vqdsnc.cn

[T59] Scala：循环
来源：http://saw.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://bkx.yj20258.top

[T60] Scala：折叠
来源：http://mwy.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wcj.wangshuangyany.cn

================================================================================
来源：http://wpy.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lzm.yj20258.top

================================================================================
来源：http://vhz.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://zua.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://dju.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://owm.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zta.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://kxv.daria6918.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://npp.feifeiyinyue.top

[U04] Py：变量调试打印
来源：http://ueg.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kkz.xylfe.cn

[U05] Py：列表去重且保序
来源：http://lon.fktsv.cn

list(dict.fromkeys(arr))
来源：http://tun.9152youxi.cn

[U06] Py：合并两个字典
来源：http://nko.jqgufenzy.top

{**a, **b}
来源：http://sbh.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://kzg.aizwys.cn

{v: k for k, v in d.items()}
来源：http://mgm.ydjk.org.cn

[U08] Py：展平二维列表
来源：http://zxq.fehbvm.com

[y for x in nested for y in x]
来源：http://ybd.nanxinkj.top

[U09] Py：字典取最大值的键
来源：http://qbs.jinghuilouyu.cn

max(d, key=d.get)
来源：http://njn.yueranfly.top

[U10] Py：按值排序字典
来源：http://rve.hesvh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://exa.fengsongda.top

[U11] Py：生成器表达式
来源：http://zky.ehwqpu.com

(x * 2 for x in arr)
来源：http://stz.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://lxr.cucudq.cn

Counter(arr).most_common(3)
来源：http://snh.birdmap.top

[U13] Py：固定长度队列
来源：http://siu.hysaishi.cn

deque(maxlen=10)
来源：http://xyb.nwbrower.top

[U14] Py：分组收集到列表
来源：http://ozy.jqgufenzy.top

defaultdict(list)
来源：http://ori.tanke756.top

[U15] Py：高精度计时
来源：http://wtf.yanxiufei.cn

t = time.perf_counter()
来源：http://fvh.xuanzx.com

[U16] Py：命令行参数解析
来源：http://ecv.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://let.hysaishi.cn

[U17] Py：初始化日志
来源：http://rbs.zhixingplan.top

logging.basicConfig(level=logging.INFO)
来源：http://pzg.hammf.cn

[U18] Py：预编译正则
来源：http://ntv.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://qxl.gzhubu.top

[U19] Py：正则替换带回调
来源：http://ele.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://las.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://kbz.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://nhe.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://uvw.sjlbkw.cn

@contextlib.contextmanager
来源：http://nil.ydzc1.top

[U22] Py：矩阵转置
来源：http://iaz.yfazqb.com

list(zip(*m))
来源：http://ijh.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://otg.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vql.0kj1m.cn

[U24] Py：路径操作
来源：http://nlc.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zir.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://cmu.svipenyu.cn

csv.DictReader(f)
来源：http://zhy.chenjidiqi.icu

[U26] Py：并发下载
来源：http://axb.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rpo.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://ewf.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://xma.smart0.xyz

[U28] Py：类型别名
来源：http://kcq.zhaomingkeji.xyz

UserId = int
来源：http://njk.zhongyouzk.top

[U29] Py：属性校验
来源：http://uyh.daxiang520.top

@property 与 @x.setter 配合
来源：http://wob.jianghu66.top

[U30] Py：数据类
来源：http://pos.yvedp.cn

@dataclass(slots=True)
来源：http://iws.sysykeji.top

[U31] Py：单测
来源：http://hzc.tian-w.cn

python -m pytest -q
来源：http://dsn.hysaishi.cn

[U32] Py：代码格式化
来源：http://noh.yj20258888.top

ruff format . && ruff check --fix .
来源：http://gnt.xylfe.cn

[U33] Py：打包发布
来源：http://drs.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://rfu.hnxiangtu.top

[U34] Py：判断编码
来源：http://eri.xinyue.icu

chardet.detect(raw)
来源：http://inj.meibo888.top

[U35] Py：发送邮件
来源：http://vap.cheryme.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tjz.jqgufenzy.top

[U36] Py：定时任务
来源：http://lrp.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://qfa.fktsv.cn

[U37] Py：读写 Excel
来源：http://hhi.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://psz.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://dln.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://tyi.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://oel.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://qfh.vehdjk.com

[U40] Py：打印到标准错误
来源：http://gze.0kj1m.cn

print("err", file=sys.stderr)
来源：http://ela.jyoumei.cn

[U41] PHP：初始化 Composer 项目
来源：http://acq.xuanzx.com

composer init;  composer require guzzlehttp/guzzle
来源：http://xlk.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://yne.zdqjudy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gwn.yvedp.cn


<!-- 参考信息 -->