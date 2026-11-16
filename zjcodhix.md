代发 wailian999

int main(int argc, char **argv)
来源：http://wcp.nanxuanxn.top

[S19] C：快速排序
来源：http://kxn.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ksy.aibaodan.cn

[S20] C：二分查找
来源：http://rxn.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ekk.chenjidiqi.icu

[S21] C：字符类别判断
来源：http://cag.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fyv.iojbl.cn

[S22] C：字符串转数字
来源：http://lih.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://npr.hfpthk.cn

[S23] C：随机数
来源：http://qlk.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://bvb.kuanghao11.cn

[S24] C：获取本地时间
来源：http://vid.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gct.aizwys.cn

[S25] C：内存拷贝
来源：http://hrd.birdmap.top

memcpy(dst, src, n);
来源：http://lkb.xylfe.cn

[S26] C：内存清零
来源：http://ggl.gzhubu.top

memset(a, 0, sizeof a);
来源：http://ujl.jyoumei.cn

[S27] C：定义常量
来源：http://kkn.xuanzx.com

const double PI = 3.14159;
来源：http://xbn.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://png.zdqjudy.top

static int counter = 0;
来源：http://kyi.gzhubu.top

[S29] C：变参函数
来源：http://djv.hongshengwenyu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://reo.yangfankeji.com

[S30] C：头文件保护
来源：http://vsr.sxryk.cn

#ifndef X_H
来源：http://tlt.wangshuangyany.cn

#define X_H
来源：http://emq.yuxming.cn

#endif
来源：http://btu.guowangkeji.top

[S31] C++：Hello World
来源：http://tou.xuetiantiany.cn

#include <iostream>
来源：http://emm.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://xfm.bjfxy.top

[S32] C++：字符串
来源：http://rga.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://fcz.xziqi.cn

[S33] C++：vector 增删
来源：http://hpx.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lpr.tanke756.top

[S34] C++：遍历 vector
来源：http://ugw.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://hvr.yonumen.top

[S35] C++：map
来源：http://txb.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wxl.yuanzhike.top

[S36] C++：unordered_map
来源：http://cfy.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rfx.nanxinkj.top

[S37] C++：set
来源：http://xak.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ibz.guowangkeji.top

[S38] C++：排序
来源：http://jkl.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://uuc.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://tmc.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zqi.smart0.xyz

[S40] C++：查找元素
来源：http://bdt.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lci.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://jzm.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qde.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://zlv.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://hwr.jqgufenzy.top

[S43] C++：智能指针
来源：http://whi.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://xmb.jiagoushi.top

[S44] C++：引用传参
来源：http://hee.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://env.hfpthk.cn

[S45] C++：lambda
来源：http://okm.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://moh.tianlin.xyz

[S46] C++：函数模板
来源：http://tde.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hed.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://dpz.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pfi.gogol.net.cn

[S48] C++：逐行读文件
来源：http://mbu.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://vqk.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://nay.gzhubu.top

[S49] C++：写文件
来源：http://bel.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jgu.meibo888.top

[S50] C++：格式化数字
来源：http://xfh.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dyd.tian-w.cn

[S51] C++：显式类型转换
来源：http://okf.guowangkeji.top

static_cast<double>(a) / b
来源：http://bok.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://tqq.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://krf.jqgufenzy.top

[S53] C++：移动语义
来源：http://jza.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://tgc.yongpay.top

[S54] C++：异常处理
来源：http://ohl.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eqv.ybcxt.top

[S55] C++：结构化绑定
来源：http://ltm.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://kxw.yueranfly.top

[S56] C++：optional
来源：http://wdm.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zus.dianchejie.cn

[S57] C++：编译期常量
来源：http://fgb.epnwcf.com

constexpr int N = 10;
来源：http://tvl.cucudq.cn

[S58] C++：命名空间
来源：http://npo.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://coh.yfazqb.com

[S59] C++：静态断言
来源：http://cvi.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kvd.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://yfd.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cic.dianchejie.cn

================================================================================
来源：http://dyd.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qpb.jiagoushi.top

================================================================================
来源：http://xzj.andypj.xyz

[T01] Kotlin：Hello World
来源：http://ylg.ywan-chungtsiang.top

println("Hello")
来源：http://vvt.hcnkem.com

[T02] Kotlin：变量
来源：http://sdo.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://odu.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://hzk.zhaomingkeji.xyz

"值: $b"
来源：http://ixu.fktsv.cn

[T04] Kotlin：空安全
来源：http://iex.yueranfly.top

val n: String? = null;  n?.length
来源：http://lei.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://yxx.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xcg.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://okh.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hoh.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://vek.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fnn.gogol.net.cn

[T08] Kotlin：数据类
来源：http://yhy.cheryme.top

data class User(val name: String, val age: Int)
来源：http://bsv.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://hiv.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://qix.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://fif.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pye.zhengqikj.top

[T11] Kotlin：协程
来源：http://qty.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oyz.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://alv.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://yzz.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://qwd.52xcode.cn

val m = mapOf("a" to 1)
来源：http://ylm.xingfuxueyuan.xyz

[T14] Kotlin：循环
来源：http://mru.zycfv.cn

for (i in 1..10) println(i)
来源：http://pdn.zhengqikj.top

[T15] Kotlin：接口
来源：http://jft.fengsongda.top

interface Shape { fun area(): Double }
来源：http://wvd.pycfn.com

[T16] Swift：Hello World
来源：http://ctl.xinyue.icu

print("Hello")
来源：http://pwu.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://kfz.nanxuanxn.top

var a = 1;  let b = 2
来源：http://akj.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://bjv.smart0.xyz

"值: \(b)"
来源：http://efj.cqqwz.cn

[T19] Swift：可选绑定
来源：http://utp.daxiang520.top

if let n = opt { print(n) }
来源：http://rom.zhongyouzk.top

[T20] Swift：数组操作
来源：http://ygq.cheryme.top

var a = [1, 2, 3];  a.append(4)
来源：http://xjg.sysykeji.top

[T21] Swift：遍历
来源：http://xii.yongpay.top

for x in a { print(x) }
来源：http://rxq.chenjidiqi.icu

[T22] Swift：字典
来源：http://irt.316326.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://ttc.xuetiantiany.cn

[T23] Swift：函数
来源：http://quk.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wrb.havefunace.top

[T24] Swift：闭包
来源：http://qex.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ypx.chenlongwang.top

[T25] Swift：结构体
来源：http://zar.gogol.net.cn

struct P { var x: Int }
来源：http://xhd.gotoacloud.top

[T26] Swift：类与重写
来源：http://sxp.hammf.cn

class A: Base { override func f() {} }
来源：http://sra.jqgfzy.top

[T27] Swift：错误处理
来源：http://xur.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://zar.yj202588.top

[T28] Swift：枚举
来源：http://xuh.jinqigfzy.top

enum Color { case red, green }
来源：http://kgx.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://xgr.pycfn.com

guard let x = opt else { return }
来源：http://cvz.feifeiyinyue.top

[T30] Swift：协议
来源：http://pdg.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://mba.mhx1999.top

[T31] Lua：Hello World
来源：http://rqp.ehwqpu.com

print("Hello")
来源：http://kqs.hcnkem.com

[T32] Lua：局部变量
来源：http://dhw.cashguo.top

local a = 1
来源：http://cej.tianlin.xyz

[T33] Lua：表（数组）
来源：http://lfr.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ocz.jinqigufen.top

[T34] Lua：遍历表
来源：http://bqx.shanyushiyangtech.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qoz.redwolf501.top

[T35] Lua：字典表
来源：http://ute.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://jqd.tian-w.cn

[T36] Lua：函数
来源：http://vpn.yonumen.top

function add(a, b) return a + b end
来源：http://gpt.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://lqx.ivvv.top

"a" .. "b"
来源：http://civ.kuanghao11.cn

[T38] Lua：条件
来源：http://dnd.zhijiandao.cn

if x > 0 then print("正") end
来源：http://icm.sxryk.cn

[T39] Lua：模式匹配
来源：http://owg.yangfankeji.com

string.find(s, "%d+")
来源：http://cnv.cdnleiting.top

[T40] Lua：元表
来源：http://med.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://vos.yj20258.top

[T41] Perl：Hello World
来源：http://mpp.jyoumei.cn

print "Hello\n";
来源：http://fxp.zhongyouzk.top

[T42] Perl：变量类型
来源：http://poh.zhongyouzk.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ahp.hysaishi.cn

[T43] Perl：字符串插值
来源：http://azq.sxryk.cn

"值: $a"
来源：http://gue.vehdjk.com

[T44] Perl：条件
来源：http://ysw.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://rcc.chenzaomai.com

[T45] Perl：数组遍历
来源：http://smo.tianlin.xyz

for my $x (@arr) { print $x; }
来源：http://ivl.yangfankeji.com

[T46] Perl：哈希操作
来源：http://nwi.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gkn.chenzaomai.com

[T47] Perl：正则捕获
来源：http://mzn.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jup.jqgfzy.top

[T48] Perl：正则替换
来源：http://buh.ehwqpu.com

$s =~ s/old/new/g;
来源：http://jkx.zycfv.cn

[T49] Perl：函数
来源：http://zpf.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fho.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://ljm.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kfa.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://eyr.zdbjq.cn

[T51] Scala：Hello World
来源：http://fti.pengpengdd.cyou

println("Hello")
来源：http://mqu.sufxvd.cn

[T52] Scala：变量
来源：http://gca.sufxvd.cn

val a = 1;  var b = 2
来源：http://nay.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://uci.zhengqikj.top

s"值: $b"
来源：http://skq.jinqigufen.top

[T54] Scala：集合映射
来源：http://ail.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://kyo.tian-w.cn

[T55] Scala：集合过滤
来源：http://fny.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lfd.yanxiufei.cn

[T56] Scala：样例类
来源：http://opi.hnqzz.top

case class User(name: String, age: Int)
来源：http://gny.hfpthk.cn

[T57] Scala：模式匹配
来源：http://ycr.fanxiaobao.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://kfd.ppjwa.cn

[T58] Scala：函数定义
来源：http://stg.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qjv.cqqwz.cn

[T59] Scala：循环
来源：http://xxp.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://naz.ivvv.top

[T60] Scala：折叠
来源：http://wji.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nmq.pengpengdd.cyou

================================================================================
来源：http://xxj.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kbz.jinqigfzy.top

================================================================================
来源：http://zse.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://kxo.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://dth.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://hmn.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ifc.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://lbj.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://jmd.jqgfzy.top

[U04] Py：变量调试打印
来源：http://aav.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ees.yuxming.cn

[U05] Py：列表去重且保序
来源：http://hbr.ywan-chungtsiang.top

list(dict.fromkeys(arr))
来源：http://hie.yueranfly.top

[U06] Py：合并两个字典
来源：http://pan.xylfe.cn

{**a, **b}
来源：http://sln.cashguo.top

[U07] Py：反转字典键值
来源：http://kcd.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://dog.cucudq.cn

[U08] Py：展平二维列表
来源：http://zqy.hnxiangtu.top

[y for x in nested for y in x]
来源：http://esm.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://plc.ybcxt.top

max(d, key=d.get)
来源：http://wee.snrcjt.cn

[U10] Py：按值排序字典
来源：http://nbb.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gkt.andypj.xyz

[U11] Py：生成器表达式
来源：http://nmm.jinqigfzy.top

(x * 2 for x in arr)
来源：http://kdp.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oyd.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://uht.sysykeji.top

[U13] Py：固定长度队列
来源：http://egf.dianchejie.cn

deque(maxlen=10)
来源：http://ugr.shanyushiyangtech.top

[U14] Py：分组收集到列表
来源：http://lyp.shanyushiyangtech.top

defaultdict(list)
来源：http://ihw.smart0.xyz

[U15] Py：高精度计时
来源：http://xrn.nanxinkj.top

t = time.perf_counter()
来源：http://xil.mhx1999.top

[U16] Py：命令行参数解析
来源：http://euv.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pvj.sufxvd.cn

[U17] Py：初始化日志
来源：http://ajj.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://cfs.cashguo.top

[U18] Py：预编译正则
来源：http://bxx.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://zpr.smart0.xyz

[U19] Py：正则替换带回调
来源：http://enr.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lte.vehdjk.com

[U20] Py：缓存函数结果
来源：http://orr.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://dhd.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://xye.hongshengwenyu.top

@contextlib.contextmanager
来源：http://hmw.tarul.cn

[U22] Py：矩阵转置
来源：http://bgu.pycfn.com

list(zip(*m))
来源：http://kho.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://dbd.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lqx.jqgufenzy.top

[U24] Py：路径操作
来源：http://doh.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cvq.52xcode.cn

[U25] Py：CSV 按字典读
来源：http://jqt.shuidangran.top

csv.DictReader(f)
来源：http://nej.havefunace.top

[U26] Py：并发下载
来源：http://fsc.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://neu.tian-w.cn

[U27] Py：异步 HTTP
来源：http://odc.ctjpmb.com

aiohttp.ClientSession() 配合 async with
来源：http://tdr.ydjk.org.cn

[U28] Py：类型别名
来源：http://dig.fktsv.cn

UserId = int
来源：http://mnz.vehdjk.com

[U29] Py：属性校验
来源：http://foo.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://aat.guowangkeji.top

[U30] Py：数据类
来源：http://wwp.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://mrg.bjfxy.top

[U31] Py：单测
来源：http://nyy.vqdsnc.cn

python -m pytest -q
来源：http://pbe.redwolf501.top

[U32] Py：代码格式化
来源：http://sho.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://zxf.tianlin.xyz

[U33] Py：打包发布
来源：http://wqn.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://mda.sweek.top

[U34] Py：判断编码
来源：http://fmx.hysaishi.cn

chardet.detect(raw)
来源：http://ftc.haohaochexian.top

[U35] Py：发送邮件
来源：http://ecs.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://omd.jinqigufen.top

[U36] Py：定时任务
来源：http://sjl.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://nbs.cucudq.cn

[U37] Py：读写 Excel
来源：http://ynv.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://ypy.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://dgh.uphjek.com

Path(__file__).resolve().parent
来源：http://tyk.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://vlr.xuanzx.com

sys.stdout.isatty()
来源：http://uba.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://ecw.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://znt.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://xqo.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zbn.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://yop.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://syp.jinqigufen.top


<!-- 参考信息 -->