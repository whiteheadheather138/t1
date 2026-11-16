代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://rez.xziqi.cn

[S15] C：类型转换
来源：http://pmh.kuanghao11.cn

(double) a / b
来源：http://jsz.chenzaomai.com

[S16] C：位操作置位
来源：http://iwt.xuanzx.com

x |= (1 << 3);
来源：http://gus.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://jol.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bop.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://kiv.nwbrower.top

int main(int argc, char **argv)
来源：http://xxz.guannengcc.top

[S19] C：快速排序
来源：http://xgv.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://sgt.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://dkl.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dym.ivvv.top

[S21] C：字符类别判断
来源：http://ych.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xac.xinyue.icu

[S22] C：字符串转数字
来源：http://okg.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://stx.0kj1m.cn

[S23] C：随机数
来源：http://fpi.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tsu.ehwqpu.com

[S24] C：获取本地时间
来源：http://cow.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ttz.bjfxy.top

[S25] C：内存拷贝
来源：http://dsq.iojbl.cn

memcpy(dst, src, n);
来源：http://epe.xuanzx.com

[S26] C：内存清零
来源：http://rxs.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://qav.yuanzhike.top

[S27] C：定义常量
来源：http://rff.cashguo.top

const double PI = 3.14159;
来源：http://rdz.chenzaomai.com

[S28] C：静态变量
来源：http://jnp.shangyingyoupin.top

static int counter = 0;
来源：http://vfb.zhoulong.xyz

[S29] C：变参函数
来源：http://ygm.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ejl.zhoulong.xyz

[S30] C：头文件保护
来源：http://rlg.birdmap.top

#ifndef X_H
来源：http://nqt.birdmap.top

#define X_H
来源：http://izm.wangshuangyany.cn

#endif
来源：http://twh.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://uik.xylfe.cn

#include <iostream>
来源：http://jgh.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://zwb.jyoumei.cn

[S32] C++：字符串
来源：http://ixd.hammf.cn

std::string s = "hi";  s += "!";
来源：http://tft.ctjpmb.com

[S33] C++：vector 增删
来源：http://etd.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://avw.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://rsh.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://pww.jianghu66.top

[S35] C++：map
来源：http://ahg.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nun.yueranfly.top

[S36] C++：unordered_map
来源：http://glq.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://myd.yuanzhike.top

[S37] C++：set
来源：http://bxz.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hxg.birdmap.top

[S38] C++：排序
来源：http://ycj.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://epc.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://yqj.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ugd.jinqigfzy.top

[S40] C++：查找元素
来源：http://yku.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xfb.cheryme.top

[S41] C++：类与构造函数
来源：http://qjg.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ubi.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://enn.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://oez.nanxuanxn.top

[S43] C++：智能指针
来源：http://elz.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://dwo.shangyingyoupin.top

[S44] C++：引用传参
来源：http://ran.mhx1999.top

void inc(int &x) { ++x; }
来源：http://ngi.nwbrower.top

[S45] C++：lambda
来源：http://abu.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vuz.hnqzz.top

[S46] C++：函数模板
来源：http://abm.cheryme.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sgz.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://ntv.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qcg.hnxiangtu.top

[S48] C++：逐行读文件
来源：http://mgx.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lkf.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://ukx.fktsv.cn

[S49] C++：写文件
来源：http://oup.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://brt.hesvh.cn

[S50] C++：格式化数字
来源：http://cpz.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://usb.guowangkeji.top

[S51] C++：显式类型转换
来源：http://jtu.ydjk.org.cn

static_cast<double>(a) / b
来源：http://lcm.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://lqy.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://jvz.yuanzhike.top

[S53] C++：移动语义
来源：http://pxl.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://hhb.havefunace.top

[S54] C++：异常处理
来源：http://klf.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tzl.316326.xyz

[S55] C++：结构化绑定
来源：http://uos.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aej.iojbl.cn

[S56] C++：optional
来源：http://dql.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rca.chenzaomai.com

[S57] C++：编译期常量
来源：http://lbf.jqgufenzy.top

constexpr int N = 10;
来源：http://kft.hnqzz.top

[S58] C++：命名空间
来源：http://qql.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://eko.dianchejie.cn

[S59] C++：静态断言
来源：http://age.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qtw.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://nwh.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sxy.bbcook.cn

================================================================================
来源：http://lbc.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mwd.xylfe.cn

================================================================================
来源：http://wsx.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://rpb.yj20258888.top

println("Hello")
来源：http://hru.ivvv.top

[T02] Kotlin：变量
来源：http://yto.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fez.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://qfq.smart0.xyz

"值: $b"
来源：http://ztp.shzxlz.cn

[T04] Kotlin：空安全
来源：http://csy.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://qua.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://srb.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iqp.316326.xyz

[T06] Kotlin：集合映射
来源：http://mac.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://chm.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://uhn.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gte.sxryk.cn

[T08] Kotlin：数据类
来源：http://qnx.hammf.cn

data class User(val name: String, val age: Int)
来源：http://fwo.zycfv.cn

[T09] Kotlin：扩展函数
来源：http://fjr.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://cwq.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://zta.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sin.zhaomingkeji.xyz

[T11] Kotlin：协程
来源：http://rsz.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://odn.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://cxz.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://bpk.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://bfm.52xcode.cn

val m = mapOf("a" to 1)
来源：http://ilg.smart0.xyz

[T14] Kotlin：循环
来源：http://ujn.sjlbkw.cn

for (i in 1..10) println(i)
来源：http://dyw.dashuyun.cn

[T15] Kotlin：接口
来源：http://llb.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://idz.tian-w.cn

[T16] Swift：Hello World
来源：http://wpp.jinqigufen.top

print("Hello")
来源：http://ytl.wangdashe.top

[T17] Swift：变量与常量
来源：http://ici.pycfn.com

var a = 1;  let b = 2
来源：http://qjl.iojbl.cn

[T18] Swift：字符串插值
来源：http://zze.sweek.top

"值: \(b)"
来源：http://rcg.wangdashe.top

[T19] Swift：可选绑定
来源：http://cjn.52xcode.cn

if let n = opt { print(n) }
来源：http://nfs.hnqzz.top

[T20] Swift：数组操作
来源：http://evd.fanxiaobao.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://xyf.feifeiyinyue.top

[T21] Swift：遍历
来源：http://cvg.hfpthk.cn

for x in a { print(x) }
来源：http://vix.jinqigufen.top

[T22] Swift：字典
来源：http://afw.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://djo.mhx1999.top

[T23] Swift：函数
来源：http://mvt.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ecq.jqgufenzy.top

[T24] Swift：闭包
来源：http://yzh.c1oappe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://inv.ydjk.org.cn

[T25] Swift：结构体
来源：http://zge.sweek.top

struct P { var x: Int }
来源：http://pit.jinyuanbaomall.cn

[T26] Swift：类与重写
来源：http://ukg.jyoumei.cn

class A: Base { override func f() {} }
来源：http://vtg.fanxiaobao.xyz

[T27] Swift：错误处理
来源：http://ual.daria6918.cn

do { try f() } catch { print(error) }
来源：http://lro.zycfv.cn

[T28] Swift：枚举
来源：http://bpo.aizwys.cn

enum Color { case red, green }
来源：http://eic.meibo888.top

[T29] Swift：guard 提前返回
来源：http://qoo.wangshuangyany.cn

guard let x = opt else { return }
来源：http://szo.hfpthk.cn

[T30] Swift：协议
来源：http://xxf.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://pzm.52xcode.cn

[T31] Lua：Hello World
来源：http://pnt.jinghuilouyu.cn

print("Hello")
来源：http://grs.hfpthk.cn

[T32] Lua：局部变量
来源：http://pmr.daxiang520.top

local a = 1
来源：http://qav.jiagoushi.top

[T33] Lua：表（数组）
来源：http://aso.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bsd.hfpthk.cn

[T34] Lua：遍历表
来源：http://pzy.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://erl.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://pwg.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://oqu.jqgfzy.top

[T36] Lua：函数
来源：http://tso.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://web.yonumen.top

[T37] Lua：字符串拼接
来源：http://fst.tarul.cn

"a" .. "b"
来源：http://boa.jlsjyb.cn

[T38] Lua：条件
来源：http://clm.zhengqikj.top

if x > 0 then print("正") end
来源：http://jcn.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://jei.chenzaomai.com

string.find(s, "%d+")
来源：http://vio.yanxiufei.cn

[T40] Lua：元表
来源：http://ekx.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://tnd.zhengqikj.top

[T41] Perl：Hello World
来源：http://oaa.jinghuilouyu.cn

print "Hello\n";
来源：http://dpm.xinyue.icu

[T42] Perl：变量类型
来源：http://vti.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jlg.ehwqpu.com

[T43] Perl：字符串插值
来源：http://zel.birdmap.top

"值: $a"
来源：http://amu.jinqigfzy.top

[T44] Perl：条件
来源：http://ssr.316326.xyz

if ($a > 0) { print "正"; }
来源：http://dvm.havefunace.top

[T45] Perl：数组遍历
来源：http://qni.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://xtx.jqgfzy.top

[T46] Perl：哈希操作
来源：http://pno.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vre.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://ayh.tanke756.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://snw.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://uso.hcnkem.com

$s =~ s/old/new/g;
来源：http://edd.dianchejie.cn

[T49] Perl：函数
来源：http://jsz.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xuj.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://ogz.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bqg.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://eku.sufxvd.cn

[T51] Scala：Hello World
来源：http://qhq.jlsjyb.cn

println("Hello")
来源：http://jzm.bbcook.cn

[T52] Scala：变量
来源：http://lbl.cashguo.top

val a = 1;  var b = 2
来源：http://clq.shzxlz.cn

[T53] Scala：字符串插值
来源：http://zhj.ppjwa.cn

s"值: $b"
来源：http://hlc.zhoulong.xyz

[T54] Scala：集合映射
来源：http://ecv.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://pai.jinyuanbaomall.cn

[T55] Scala：集合过滤
来源：http://dgr.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vdm.hywenlv.cn

[T56] Scala：样例类
来源：http://eia.chenlongwang.top

case class User(name: String, age: Int)
来源：http://dmh.redwolf501.top

[T57] Scala：模式匹配
来源：http://ejk.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nnc.gotoacloud.top

[T58] Scala：函数定义
来源：http://jhp.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zmj.52xcode.cn

[T59] Scala：循环
来源：http://yzl.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://aaz.gotoacloud.top

[T60] Scala：折叠
来源：http://xci.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yla.mhx1999.top

================================================================================
来源：http://axu.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wob.c1oappe.top

================================================================================
来源：http://bbi.jinqigufen.top

[U01] Py：创建虚拟环境
来源：http://qvo.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://hyr.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://zit.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gqg.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://uuk.aizwys.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zze.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://lsj.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://khr.xylfe.cn

[U05] Py：列表去重且保序
来源：http://vbm.ydzc1.top

list(dict.fromkeys(arr))
来源：http://fpa.guowangkeji.top

[U06] Py：合并两个字典
来源：http://wkq.epnwcf.com

{**a, **b}
来源：http://oqv.fzhhl.top

[U07] Py：反转字典键值
来源：http://faw.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://ayp.guowangkeji.top

[U08] Py：展平二维列表
来源：http://hxt.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://tei.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://lgv.fehbvm.com

max(d, key=d.get)
来源：http://rvd.0kj1m.cn

[U10] Py：按值排序字典
来源：http://xhu.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eeb.ydzc1.top

[U11] Py：生成器表达式
来源：http://jab.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://goe.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qkh.chenjidiqi.icu

Counter(arr).most_common(3)
来源：http://hmk.sxryk.cn

[U13] Py：固定长度队列
来源：http://bty.hcnkem.com

deque(maxlen=10)
来源：http://ufm.xinyue.icu

[U14] Py：分组收集到列表
来源：http://uil.pycfn.com

defaultdict(list)
来源：http://qvb.svipenyu.cn

[U15] Py：高精度计时
来源：http://psj.haohaochexian.top

t = time.perf_counter()
来源：http://vet.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://nnz.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zuy.316326.xyz

[U17] Py：初始化日志
来源：http://onu.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://buu.xinyue.icu

[U18] Py：预编译正则
来源：http://lvd.aizwys.cn

pat = re.compile(r"\d+")
来源：http://wtu.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://qfp.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://stw.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://bwj.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://ing.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://yka.guowangkeji.top

@contextlib.contextmanager
来源：http://aqi.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://gdn.jinqigfzy.top

list(zip(*m))
来源：http://iuc.cashguo.top

[U23] Py：分块读取大文件
来源：http://ecr.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://opq.cqqwz.cn

[U24] Py：路径操作
来源：http://kth.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iho.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://tbv.hysaishi.cn

csv.DictReader(f)
来源：http://aif.gotoacloud.top

[U26] Py：并发下载
来源：http://hac.jlsjyb.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oxk.guannengcc.top

[U27] Py：异步 HTTP
来源：http://czb.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://ayy.xuetiantiany.cn

[U28] Py：类型别名
来源：http://jpk.shzxlz.cn

UserId = int
来源：http://vlj.zycfv.cn

[U29] Py：属性校验
来源：http://vmg.sjlbkw.cn

@property 与 @x.setter 配合
来源：http://rgr.xuanzx.com

[U30] Py：数据类
来源：http://tlj.316326.xyz

@dataclass(slots=True)
来源：http://bpl.jinqigufen.top

[U31] Py：单测
来源：http://lxh.ehwqpu.com

python -m pytest -q
来源：http://kaw.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://nvv.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://uou.andypj.xyz

[U33] Py：打包发布
来源：http://olp.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://rjx.jyoumei.cn

[U34] Py：判断编码
来源：http://lqj.yangfankeji.com

chardet.detect(raw)
来源：http://osx.zycfv.cn

[U35] Py：发送邮件
来源：http://fsz.snrcjt.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rex.jqgufenzy.top

[U36] Py：定时任务
来源：http://kgl.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://wzz.ivvv.top

[U37] Py：读写 Excel
来源：http://fcj.shanyushiyangtech.top

pandas.read_excel / DataFrame.to_excel
来源：http://zhs.xingfuxueyuan.xyz

[U38] Py：获取脚本所在目录
来源：http://kua.hcnkem.com

Path(__file__).resolve().parent
来源：http://otf.yuxming.cn


<!-- 参考信息 -->