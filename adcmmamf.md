代发 wailian999

int main(int argc, char **argv)
来源：http://dyn.smart0.xyz

[S19] C：快速排序
来源：http://uhd.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gbk.jinqigufen.top

[S20] C：二分查找
来源：http://znn.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qky.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://fcr.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qzt.yonumen.top

[S22] C：字符串转数字
来源：http://rwz.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://kdz.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://ltv.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bcq.fzhhl.top

[S24] C：获取本地时间
来源：http://dwq.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://puj.nwbrower.top

[S25] C：内存拷贝
来源：http://pbr.mhx1999.top

memcpy(dst, src, n);
来源：http://wam.aibaodan.cn

[S26] C：内存清零
来源：http://kxx.hesvh.cn

memset(a, 0, sizeof a);
来源：http://poa.smart0.xyz

[S27] C：定义常量
来源：http://unp.hcnkem.com

const double PI = 3.14159;
来源：http://pnd.aibaodan.cn

[S28] C：静态变量
来源：http://nwl.daria6918.cn

static int counter = 0;
来源：http://qje.gzhubu.top

[S29] C：变参函数
来源：http://onp.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zqw.yj20258.top

[S30] C：头文件保护
来源：http://shd.ctjpmb.com

#ifndef X_H
来源：http://dnx.yuanzhike.top

#define X_H
来源：http://hhy.zycfv.cn

#endif
来源：http://zfz.zdbjq.cn

[S31] C++：Hello World
来源：http://lmh.hnqzz.top

#include <iostream>
来源：http://hfz.sufxvd.cn

int main() { std::cout << "Hello\n"; }
来源：http://mux.zhixingplan.top

[S32] C++：字符串
来源：http://wqv.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://dae.zdbjq.cn

[S33] C++：vector 增删
来源：http://jmp.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vol.tian-w.cn

[S34] C++：遍历 vector
来源：http://eid.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://xio.guowangkeji.top

[S35] C++：map
来源：http://gpc.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yuh.ydzc1.top

[S36] C++：unordered_map
来源：http://ggq.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://neg.zdqjudy.top

[S37] C++：set
来源：http://dpx.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cqi.haohaochexian.top

[S38] C++：排序
来源：http://vds.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://ugw.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://gdm.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hoz.pengpengdd.cyou

[S40] C++：查找元素
来源：http://zdi.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://amc.gogol.net.cn

[S41] C++：类与构造函数
来源：http://gpo.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oxa.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://ykk.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://vkg.haohaochexian.top

[S43] C++：智能指针
来源：http://lxh.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://eql.zhongyouzk.top

[S44] C++：引用传参
来源：http://nfx.smart0.xyz

void inc(int &x) { ++x; }
来源：http://qft.cucudq.cn

[S45] C++：lambda
来源：http://nws.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://owk.svipenyu.cn

[S46] C++：函数模板
来源：http://kob.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bbo.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://sln.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yxe.jiagoushi.top

[S48] C++：逐行读文件
来源：http://rqn.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://wan.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://rax.wangshuangyany.cn

[S49] C++：写文件
来源：http://qmf.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pru.zhijiandao.cn

[S50] C++：格式化数字
来源：http://tle.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eyv.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://erb.zycfv.cn

static_cast<double>(a) / b
来源：http://mcx.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://hvc.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://tbb.yj20258888.top

[S53] C++：移动语义
来源：http://tst.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://mxd.yanxiufei.cn

[S54] C++：异常处理
来源：http://awa.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ybi.jianghu66.top

[S55] C++：结构化绑定
来源：http://tgv.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eib.ydzc1.top

[S56] C++：optional
来源：http://nnd.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tef.vqdsnc.cn

[S57] C++：编译期常量
来源：http://eno.shzxlz.cn

constexpr int N = 10;
来源：http://dyz.andypj.xyz

[S58] C++：命名空间
来源：http://ngm.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://xcq.yj202588.top

[S59] C++：静态断言
来源：http://lde.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fxc.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://bwc.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dty.52xcode.cn

================================================================================
来源：http://kyg.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kbd.yangfankeji.com

================================================================================
来源：http://cjj.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://jtb.aibaodan.cn

println("Hello")
来源：http://evt.52xcode.cn

[T02] Kotlin：变量
来源：http://fon.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://feo.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://sqk.iojbl.cn

"值: $b"
来源：http://yio.xinyue.icu

[T04] Kotlin：空安全
来源：http://ebj.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://jjm.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://ewh.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mth.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://wht.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mhh.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://tqv.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eft.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://sff.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://hwc.hammf.cn

[T09] Kotlin：扩展函数
来源：http://twl.zhongyouzk.top

fun String.exclaim() = this + "!"
来源：http://orz.xuanzx.com

[T10] Kotlin：默认参数
来源：http://jkf.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nlu.shuidangran.top

[T11] Kotlin：协程
来源：http://onm.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yrq.meibo888.top

[T12] Kotlin：解构声明
来源：http://ifm.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://ooq.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://gxl.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://dqx.ppjwa.cn

[T14] Kotlin：循环
来源：http://aqi.fanxiaobao.xyz

for (i in 1..10) println(i)
来源：http://atd.52xcode.cn

[T15] Kotlin：接口
来源：http://ong.hysaishi.cn

interface Shape { fun area(): Double }
来源：http://mje.ctjpmb.com

[T16] Swift：Hello World
来源：http://tgv.yj202588.top

print("Hello")
来源：http://irr.dashuyun.cn

[T17] Swift：变量与常量
来源：http://uzn.fengsongda.top

var a = 1;  let b = 2
来源：http://qnb.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://trb.epnwcf.com

"值: \(b)"
来源：http://emx.birdmap.top

[T19] Swift：可选绑定
来源：http://itk.bjfxy.top

if let n = opt { print(n) }
来源：http://mcx.cqqwz.cn

[T20] Swift：数组操作
来源：http://imk.birdmap.top

var a = [1, 2, 3];  a.append(4)
来源：http://ega.tianlin.xyz

[T21] Swift：遍历
来源：http://kdm.bjfxy.top

for x in a { print(x) }
来源：http://nuc.316326.xyz

[T22] Swift：字典
来源：http://zxm.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ytk.hywenlv.cn

[T23] Swift：函数
来源：http://wet.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oml.cqqwz.cn

[T24] Swift：闭包
来源：http://lsy.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yhk.yj20258.top

[T25] Swift：结构体
来源：http://mmr.havefunace.top

struct P { var x: Int }
来源：http://ddf.birdmap.top

[T26] Swift：类与重写
来源：http://rfs.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://fet.zdbjq.cn

[T27] Swift：错误处理
来源：http://ihm.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://ntj.hfpthk.cn

[T28] Swift：枚举
来源：http://wgs.smart0.xyz

enum Color { case red, green }
来源：http://qzb.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://ujb.xziqi.cn

guard let x = opt else { return }
来源：http://xax.dianchejie.cn

[T30] Swift：协议
来源：http://ujq.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://ssr.gogol.net.cn

[T31] Lua：Hello World
来源：http://qap.yangfankeji.com

print("Hello")
来源：http://gfg.yongpay.top

[T32] Lua：局部变量
来源：http://wir.yuxming.cn

local a = 1
来源：http://hdt.epnwcf.com

[T33] Lua：表（数组）
来源：http://cxb.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://mmu.xziqi.cn

[T34] Lua：遍历表
来源：http://iko.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://htg.gogol.net.cn

[T35] Lua：字典表
来源：http://gxm.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://paq.pycfn.com

[T36] Lua：函数
来源：http://gtz.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://gcq.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://ida.jinqigufen.top

"a" .. "b"
来源：http://fnd.ybcxt.top

[T38] Lua：条件
来源：http://xbv.yanxiufei.cn

if x > 0 then print("正") end
来源：http://ieo.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://yow.zhengqikj.top

string.find(s, "%d+")
来源：http://agf.gotoacloud.top

[T40] Lua：元表
来源：http://vow.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://rlf.hnqzz.top

[T41] Perl：Hello World
来源：http://pew.tarul.cn

print "Hello\n";
来源：http://ghz.yvedp.cn

[T42] Perl：变量类型
来源：http://qav.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://npb.cashguo.top

[T43] Perl：字符串插值
来源：http://luv.hcnkem.com

"值: $a"
来源：http://oqb.jinqigfzy.top

[T44] Perl：条件
来源：http://onj.0kj1m.cn

if ($a > 0) { print "正"; }
来源：http://ufn.gotoacloud.top

[T45] Perl：数组遍历
来源：http://ivc.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://cst.xinyue.icu

[T46] Perl：哈希操作
来源：http://jmw.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ouv.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://pec.sxryk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dgh.tarul.cn

[T48] Perl：正则替换
来源：http://vgr.ctjpmb.com

$s =~ s/old/new/g;
来源：http://clc.yueranfly.top

[T49] Perl：函数
来源：http://kzs.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qbn.tian-w.cn

[T50] Perl：逐行读文件
来源：http://vca.vehdjk.com

open my $fh, "<", "a.txt" or die $!;
来源：http://tpj.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://nhg.sweek.top

[T51] Scala：Hello World
来源：http://lch.bjfxy.top

println("Hello")
来源：http://ykd.shzxlz.cn

[T52] Scala：变量
来源：http://jcs.andypj.xyz

val a = 1;  var b = 2
来源：http://agx.yuxming.cn

[T53] Scala：字符串插值
来源：http://qcz.ywan-chungtsiang.top

s"值: $b"
来源：http://nws.cucudq.cn

[T54] Scala：集合映射
来源：http://hel.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://fbk.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://ggr.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://lmw.hfpthk.cn

[T56] Scala：样例类
来源：http://jyb.meibo888.top

case class User(name: String, age: Int)
来源：http://ipl.c1oappe.top

[T57] Scala：模式匹配
来源：http://jwm.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rle.yfazqb.com

[T58] Scala：函数定义
来源：http://bdo.haohaochexian.top

def add(a: Int, b: Int): Int = a + b
来源：http://ygb.xziqi.cn

[T59] Scala：循环
来源：http://ips.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://aiq.hnxiangtu.top

[T60] Scala：折叠
来源：http://hiq.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iet.ybcxt.top

================================================================================
来源：http://bdg.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://flj.dashuyun.cn

================================================================================
来源：http://sbg.zhaomingkeji.xyz

[U01] Py：创建虚拟环境
来源：http://sxd.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://acn.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://qlr.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ayz.yueranfly.top

[U03] Py：加载 .env 配置
来源：http://nrf.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gcl.hnqzz.top

[U04] Py：变量调试打印
来源：http://tvq.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nhm.sufxvd.cn

[U05] Py：列表去重且保序
来源：http://tvh.hesvh.cn

list(dict.fromkeys(arr))
来源：http://tbz.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://xta.tianlin.xyz

{**a, **b}
来源：http://btf.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://gmg.c1oappe.top

{v: k for k, v in d.items()}
来源：http://ori.yvedp.cn

[U08] Py：展平二维列表
来源：http://piw.chenlongwang.top

[y for x in nested for y in x]
来源：http://dbj.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://hvn.hcnkem.com

max(d, key=d.get)
来源：http://lss.gzhubu.top

[U10] Py：按值排序字典
来源：http://iqg.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cig.vehdjk.com

[U11] Py：生成器表达式
来源：http://ign.guowangkeji.top

(x * 2 for x in arr)
来源：http://jqp.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kwf.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://ooy.nwbrower.top

[U13] Py：固定长度队列
来源：http://dcl.jianghu66.top

deque(maxlen=10)
来源：http://iry.cucudq.cn

[U14] Py：分组收集到列表
来源：http://ckx.cashguo.top

defaultdict(list)
来源：http://qwn.yfazqb.com

[U15] Py：高精度计时
来源：http://qpr.9152youxi.cn

t = time.perf_counter()
来源：http://acj.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://dod.316326.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vfs.jianghu66.top

[U17] Py：初始化日志
来源：http://yzv.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://mrv.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://del.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://usy.havefunace.top

[U19] Py：正则替换带回调
来源：http://mks.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eqc.pycfn.com

[U20] Py：缓存函数结果
来源：http://lfu.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://rog.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://ihh.fengsongda.top

@contextlib.contextmanager
来源：http://odn.ppjwa.cn

[U22] Py：矩阵转置
来源：http://dfy.vqdsnc.cn

list(zip(*m))
来源：http://gkx.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://zub.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dgv.ydzc1.top

[U24] Py：路径操作
来源：http://dkq.bjfxy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aai.wangshuangyany.cn

[U25] Py：CSV 按字典读
来源：http://cqc.daria6918.cn

csv.DictReader(f)
来源：http://wjj.zhengqikj.top

[U26] Py：并发下载
来源：http://ygm.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jxx.iojbl.cn

[U27] Py：异步 HTTP
来源：http://bes.iojbl.cn

aiohttp.ClientSession() 配合 async with
来源：http://quo.haohaochexian.top

[U28] Py：类型别名
来源：http://ivv.ydjk.org.cn

UserId = int
来源：http://pij.gaohongyu789.top

[U29] Py：属性校验
来源：http://gzv.sweek.top

@property 与 @x.setter 配合
来源：http://fop.kuanghao11.cn

[U30] Py：数据类
来源：http://zxa.guannengcc.top

@dataclass(slots=True)
来源：http://wrg.hnqzz.top

[U31] Py：单测
来源：http://hdk.jianghu66.top

python -m pytest -q
来源：http://ntk.aizwys.cn

[U32] Py：代码格式化
来源：http://bbq.sysykeji.top

ruff format . && ruff check --fix .
来源：http://dvm.meibo888.top

[U33] Py：打包发布
来源：http://mic.havefunace.top

python -m build  （依赖 pyproject.toml）
来源：http://yit.hnxiangtu.top

[U34] Py：判断编码
来源：http://hnr.tanke756.top

chardet.detect(raw)
来源：http://ocv.zhixingplan.top

[U35] Py：发送邮件
来源：http://whu.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pot.zhongyouzk.top

[U36] Py：定时任务
来源：http://rlj.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://xfr.fengsongda.top

[U37] Py：读写 Excel
来源：http://djt.vqdsnc.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bkp.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://lku.zycfv.cn

Path(__file__).resolve().parent
来源：http://arj.gzhubu.top

[U39] Py：判断是否在交互环境
来源：http://fah.shuidangran.top

sys.stdout.isatty()
来源：http://wup.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://abs.mhx1999.top

print("err", file=sys.stderr)
来源：http://frr.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://gsv.hongshengwenyu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rbs.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://fcy.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bwe.0kj1m.cn


<!-- 参考信息 -->