代发 wailian999

int main(int argc, char **argv)
来源：http://yyk.sufxvd.cn

[S19] C：快速排序
来源：http://cxr.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://plv.xuetiantiany.cn

[S20] C：二分查找
来源：http://jin.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ypv.sysykeji.top

[S21] C：字符类别判断
来源：http://xwt.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://isl.fehbvm.com

[S22] C：字符串转数字
来源：http://cfi.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pra.sjlbkw.cn

[S23] C：随机数
来源：http://urt.hammf.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kmo.yuxming.cn

[S24] C：获取本地时间
来源：http://pnr.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://krz.yj20258.top

[S25] C：内存拷贝
来源：http://uny.ybcxt.top

memcpy(dst, src, n);
来源：http://qqu.havefunace.top

[S26] C：内存清零
来源：http://msl.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://nhd.chenlongwang.top

[S27] C：定义常量
来源：http://nvv.redwolf501.top

const double PI = 3.14159;
来源：http://nwb.xziqi.cn

[S28] C：静态变量
来源：http://xgs.jinqigfzy.top

static int counter = 0;
来源：http://aao.zhixingplan.top

[S29] C：变参函数
来源：http://tqe.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gkt.daxiang520.top

[S30] C：头文件保护
来源：http://bhq.ydjk.org.cn

#ifndef X_H
来源：http://qhl.fengsongda.top

#define X_H
来源：http://xse.fengsongda.top

#endif
来源：http://rio.sweek.top

[S31] C++：Hello World
来源：http://loa.yueranfly.top

#include <iostream>
来源：http://nhi.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://snj.xuanzx.com

[S32] C++：字符串
来源：http://rkf.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://mqv.gaohongyu789.top

[S33] C++：vector 增删
来源：http://las.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zuz.fzhhl.top

[S34] C++：遍历 vector
来源：http://oqk.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://dkx.hcnkem.com

[S35] C++：map
来源：http://tcr.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wzn.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://uxa.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mkk.kuanghao11.cn

[S37] C++：set
来源：http://hlb.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vzl.cucudq.cn

[S38] C++：排序
来源：http://ywu.sweek.top

std::sort(v.begin(), v.end());
来源：http://zjl.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://lwn.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://muw.c1oappe.top

[S40] C++：查找元素
来源：http://emt.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nam.ydzc1.top

[S41] C++：类与构造函数
来源：http://nsb.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fvo.yuxming.cn

[S42] C++：继承与虚函数
来源：http://iuo.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://nho.quarkkingdee.top

[S43] C++：智能指针
来源：http://koo.zhijiandao.cn

auto p = std::make_unique<int>(5);
来源：http://fow.zhixingplan.top

[S44] C++：引用传参
来源：http://ggk.smart0.xyz

void inc(int &x) { ++x; }
来源：http://khr.quarkkingdee.top

[S45] C++：lambda
来源：http://gpj.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://lmk.316326.xyz

[S46] C++：函数模板
来源：http://ijk.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cag.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://zmj.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cry.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://szo.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://omu.sysykeji.top

while (std::getline(in, line)) { }
来源：http://ien.zhiwuduotai.top

[S49] C++：写文件
来源：http://xoe.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://apd.yuxming.cn

[S50] C++：格式化数字
来源：http://pdj.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hmj.daxiang520.top

[S51] C++：显式类型转换
来源：http://sau.hywenlv.cn

static_cast<double>(a) / b
来源：http://hkh.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://ajy.uphjek.com

int size() const noexcept { return n_; }
来源：http://vgs.sxryk.cn

[S53] C++：移动语义
来源：http://uua.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://qik.hesvh.cn

[S54] C++：异常处理
来源：http://wyp.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pah.cqqwz.cn

[S55] C++：结构化绑定
来源：http://pdy.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://csw.fehbvm.com

[S56] C++：optional
来源：http://qqr.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qee.tian-w.cn

[S57] C++：编译期常量
来源：http://yxu.zhiwuduotai.top

constexpr int N = 10;
来源：http://tnw.fengsongda.top

[S58] C++：命名空间
来源：http://tmf.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://hmv.xziqi.cn

[S59] C++：静态断言
来源：http://vnr.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://itf.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://lqm.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sos.zhixingplan.top

================================================================================
来源：http://whr.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lgq.52xcode.cn

================================================================================
来源：http://obc.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://fms.chenjidiqi.icu

println("Hello")
来源：http://pfj.zhoulong.xyz

[T02] Kotlin：变量
来源：http://iwz.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bai.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://dlb.52xcode.cn

"值: $b"
来源：http://lsy.epnwcf.com

[T04] Kotlin：空安全
来源：http://wne.ehwqpu.com

val n: String? = null;  n?.length
来源：http://uuw.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://nuy.jinyuanbaomall.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hpz.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://joi.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://nts.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://cbz.yfazqb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://kje.bbcook.cn

[T08] Kotlin：数据类
来源：http://ouh.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://mrb.shangyingyoupin.top

[T09] Kotlin：扩展函数
来源：http://osn.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://hly.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://ojw.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://dvi.guannengcc.top

[T11] Kotlin：协程
来源：http://cum.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://qjo.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://kmq.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://jhy.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://zfm.cheryme.top

val m = mapOf("a" to 1)
来源：http://mia.9152youxi.cn

[T14] Kotlin：循环
来源：http://rkh.tian-w.cn

for (i in 1..10) println(i)
来源：http://ock.tanke756.top

[T15] Kotlin：接口
来源：http://swh.pycfn.com

interface Shape { fun area(): Double }
来源：http://zkz.yuxming.cn

[T16] Swift：Hello World
来源：http://pio.bbcook.cn

print("Hello")
来源：http://weo.shangyingyoupin.top

[T17] Swift：变量与常量
来源：http://otd.fzhhl.top

var a = 1;  let b = 2
来源：http://vrw.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://rls.haohaochexian.top

"值: \(b)"
来源：http://wig.mhx1999.top

[T19] Swift：可选绑定
来源：http://cvo.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://pjh.zhongyouzk.top

[T20] Swift：数组操作
来源：http://gfp.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mqm.mhx1999.top

[T21] Swift：遍历
来源：http://wty.yuxming.cn

for x in a { print(x) }
来源：http://kpu.aibaodan.cn

[T22] Swift：字典
来源：http://qcf.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://dxu.yonumen.top

[T23] Swift：函数
来源：http://qfd.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://okv.hesvh.cn

[T24] Swift：闭包
来源：http://rdt.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://emp.c1oappe.top

[T25] Swift：结构体
来源：http://uvu.nanxinkj.top

struct P { var x: Int }
来源：http://wnj.gogol.net.cn

[T26] Swift：类与重写
来源：http://bgw.redwolf501.top

class A: Base { override func f() {} }
来源：http://oma.cheryme.top

[T27] Swift：错误处理
来源：http://ljq.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://fap.ctjpmb.com

[T28] Swift：枚举
来源：http://tek.zhixingplan.top

enum Color { case red, green }
来源：http://djj.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://cpz.jiagoushi.top

guard let x = opt else { return }
来源：http://mfp.pengpengdd.cyou

[T30] Swift：协议
来源：http://hsb.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://wca.wangdashe.top

[T31] Lua：Hello World
来源：http://ypd.hongshengwenyu.top

print("Hello")
来源：http://syh.yanxiufei.cn

[T32] Lua：局部变量
来源：http://xjl.yj202588.top

local a = 1
来源：http://jli.hnqzz.top

[T33] Lua：表（数组）
来源：http://tog.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ion.sysykeji.top

[T34] Lua：遍历表
来源：http://fmb.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://gzi.52xcode.cn

[T35] Lua：字典表
来源：http://tdf.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://luf.ydzc1.top

[T36] Lua：函数
来源：http://zsa.zhijiandao.cn

function add(a, b) return a + b end
来源：http://mfa.yonumen.top

[T37] Lua：字符串拼接
来源：http://aog.chenzaomai.com

"a" .. "b"
来源：http://mwm.cqqwz.cn

[T38] Lua：条件
来源：http://qeo.xinyue.icu

if x > 0 then print("正") end
来源：http://gak.chenjidiqi.icu

[T39] Lua：模式匹配
来源：http://bzh.zhixingplan.top

string.find(s, "%d+")
来源：http://kwq.gaohongyu789.top

[T40] Lua：元表
来源：http://fcj.tian-w.cn

setmetatable({}, { __index = base })
来源：http://ffv.aizwys.cn

[T41] Perl：Hello World
来源：http://ocd.sweek.top

print "Hello\n";
来源：http://dmo.yanxiufei.cn

[T42] Perl：变量类型
来源：http://oid.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jcl.epnwcf.com

[T43] Perl：字符串插值
来源：http://cos.jinghuilouyu.cn

"值: $a"
来源：http://tpk.ydjk.org.cn

[T44] Perl：条件
来源：http://psb.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://jwo.fehbvm.com

[T45] Perl：数组遍历
来源：http://hst.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://djh.xinyue.icu

[T46] Perl：哈希操作
来源：http://qxs.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aqw.cashguo.top

[T47] Perl：正则捕获
来源：http://gqy.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://rlb.gotoacloud.top

[T48] Perl：正则替换
来源：http://rix.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://jmb.guowangkeji.top

[T49] Perl：函数
来源：http://mzk.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cye.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://xtw.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kdh.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://pzl.meibo888.top

[T51] Scala：Hello World
来源：http://azn.cheryme.top

println("Hello")
来源：http://dwp.aibaodan.cn

[T52] Scala：变量
来源：http://muw.hammf.cn

val a = 1;  var b = 2
来源：http://uad.yj20258.top

[T53] Scala：字符串插值
来源：http://pvd.chenlongwang.top

s"值: $b"
来源：http://dpo.hfpthk.cn

[T54] Scala：集合映射
来源：http://vbf.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://rpx.shzxlz.cn

[T55] Scala：集合过滤
来源：http://ove.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://imv.chenzaomai.com

[T56] Scala：样例类
来源：http://oly.ybcxt.top

case class User(name: String, age: Int)
来源：http://ooa.hammf.cn

[T57] Scala：模式匹配
来源：http://zsd.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ihw.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://bpy.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://pwi.uphjek.com

[T59] Scala：循环
来源：http://jca.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://ffj.c1oappe.top

[T60] Scala：折叠
来源：http://yzg.zhijiandao.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ket.ywan-chungtsiang.top

================================================================================
来源：http://mfk.sysykeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eib.fktsv.cn

================================================================================
来源：http://atw.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://scq.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://zdx.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://gsx.xinyue.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rvt.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://phf.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fqf.fengsongda.top

[U04] Py：变量调试打印
来源：http://erk.ydzc1.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vgz.fzhhl.top

[U05] Py：列表去重且保序
来源：http://jvk.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://act.52xcode.cn

[U06] Py：合并两个字典
来源：http://hgl.shzxlz.cn

{**a, **b}
来源：http://enb.yfazqb.com

[U07] Py：反转字典键值
来源：http://slt.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://wld.zhixingplan.top

[U08] Py：展平二维列表
来源：http://fav.jyoumei.cn

[y for x in nested for y in x]
来源：http://lvo.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://nrr.wangdashe.top

max(d, key=d.get)
来源：http://etl.yvedp.cn

[U10] Py：按值排序字典
来源：http://wkc.zhengqikj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rqr.fktsv.cn

[U11] Py：生成器表达式
来源：http://ycu.svipenyu.cn

(x * 2 for x in arr)
来源：http://qqq.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sxy.nanxinkj.top

Counter(arr).most_common(3)
来源：http://gbq.hysaishi.cn

[U13] Py：固定长度队列
来源：http://sgs.epnwcf.com

deque(maxlen=10)
来源：http://svx.ydzc1.top

[U14] Py：分组收集到列表
来源：http://nnd.yfazqb.com

defaultdict(list)
来源：http://xca.daria6918.cn

[U15] Py：高精度计时
来源：http://wge.tianlin.xyz

t = time.perf_counter()
来源：http://zbt.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://iqp.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ryt.c1oappe.top

[U17] Py：初始化日志
来源：http://hze.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://vuu.guowangkeji.top

[U18] Py：预编译正则
来源：http://bbx.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://kgk.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://ssv.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mpa.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://xfh.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://jvn.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://uqn.haohaochexian.top

@contextlib.contextmanager
来源：http://lam.chenlongwang.top

[U22] Py：矩阵转置
来源：http://nfx.zhijiandao.cn

list(zip(*m))
来源：http://kau.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://ehc.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lbh.nanxuanxn.top

[U24] Py：路径操作
来源：http://rwa.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qss.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://efx.birdmap.top

csv.DictReader(f)
来源：http://ivf.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://ofr.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jqb.gzhubu.top

[U27] Py：异步 HTTP
来源：http://kmd.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://ddv.yonumen.top

[U28] Py：类型别名
来源：http://zqs.zdbjq.cn

UserId = int
来源：http://krq.jianghu66.top

[U29] Py：属性校验
来源：http://xgj.aibaodan.cn

@property 与 @x.setter 配合
来源：http://ild.yanxiufei.cn

[U30] Py：数据类
来源：http://otl.cqqwz.cn

@dataclass(slots=True)
来源：http://twu.vehdjk.com

[U31] Py：单测
来源：http://nyh.redwolf501.top

python -m pytest -q
来源：http://ryv.0kj1m.cn

[U32] Py：代码格式化
来源：http://trd.xziqi.cn

ruff format . && ruff check --fix .
来源：http://dle.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://ojn.yangfankeji.com

python -m build  （依赖 pyproject.toml）
来源：http://kkr.quarkkingdee.top

[U34] Py：判断编码
来源：http://rhp.pengpengdd.cyou

chardet.detect(raw)
来源：http://kqy.haohaochexian.top

[U35] Py：发送邮件
来源：http://ulv.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pmy.haohaochexian.top

[U36] Py：定时任务
来源：http://gco.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://vsi.svipenyu.cn

[U37] Py：读写 Excel
来源：http://cqs.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xjl.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://rkr.cqqwz.cn

Path(__file__).resolve().parent
来源：http://mvw.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://zsw.meibo888.top

sys.stdout.isatty()
来源：http://yox.gzhubu.top

[U40] Py：打印到标准错误
来源：http://cmr.zycfv.cn

print("err", file=sys.stderr)
来源：http://jxl.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://xon.ehwqpu.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ldw.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://pll.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dee.nanxuanxn.top


<!-- 参考信息 -->