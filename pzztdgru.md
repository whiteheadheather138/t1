代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://afd.zhengqikj.top

[S10] C：指针与解引用
来源：http://afe.ybcxt.top

int *p = &a;  *p = 5;
来源：http://pab.fehbvm.com

[S11] C：逐行读文件
来源：http://seq.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://gug.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ruq.dashuyun.cn

fclose(f);
来源：http://sym.xuanzx.com

[S12] C：写文件
来源：http://nqw.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zff.cheryme.top

[S13] C：宏定义
来源：http://zbc.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eub.wangshuangyany.cn

[S14] C：枚举
来源：http://fhi.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://hbc.vqdsnc.cn

[S15] C：类型转换
来源：http://yef.nanxuanxn.top

(double) a / b
来源：http://cii.nwbrower.top

[S16] C：位操作置位
来源：http://wlo.gotoacloud.top

x |= (1 << 3);
来源：http://dum.52xcode.cn

[S17] C：安全拼接字符串
来源：http://cjj.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gyb.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://tez.ydzc1.top

int main(int argc, char **argv)
来源：http://vva.52xcode.cn

[S19] C：快速排序
来源：http://xrr.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ufo.zdqjudy.top

[S20] C：二分查找
来源：http://wkk.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vbo.9152youxi.cn

[S21] C：字符类别判断
来源：http://ffc.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jba.ctjpmb.com

[S22] C：字符串转数字
来源：http://smb.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mfk.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://dko.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ijk.gaohongyu789.top

[S24] C：获取本地时间
来源：http://omt.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://raz.zhijiandao.cn

[S25] C：内存拷贝
来源：http://kak.hcnkem.com

memcpy(dst, src, n);
来源：http://glm.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://mha.yueranfly.top

memset(a, 0, sizeof a);
来源：http://pss.yj20258.top

[S27] C：定义常量
来源：http://eyu.zhixingplan.top

const double PI = 3.14159;
来源：http://scz.zhengqikj.top

[S28] C：静态变量
来源：http://rvq.jinghuilouyu.cn

static int counter = 0;
来源：http://ygr.hysaishi.cn

[S29] C：变参函数
来源：http://hvs.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vyo.yuanzhike.top

[S30] C：头文件保护
来源：http://yed.jlsjyb.cn

#ifndef X_H
来源：http://dgh.jinqigfzy.top

#define X_H
来源：http://ezd.meibo888.top

#endif
来源：http://tiz.0kj1m.cn

[S31] C++：Hello World
来源：http://lve.zhoulong.xyz

#include <iostream>
来源：http://hmi.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://aoi.jinghuilouyu.cn

[S32] C++：字符串
来源：http://rnb.yongpay.top

std::string s = "hi";  s += "!";
来源：http://oth.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://mva.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qpf.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://deg.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://aha.andypj.xyz

[S35] C++：map
来源：http://iyq.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ltu.tian-w.cn

[S36] C++：unordered_map
来源：http://eui.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://peb.zhengqikj.top

[S37] C++：set
来源：http://pom.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xly.jqgufenzy.top

[S38] C++：排序
来源：http://ihy.yj202588.top

std::sort(v.begin(), v.end());
来源：http://vlc.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://kux.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qhw.fengsongda.top

[S40] C++：查找元素
来源：http://fwo.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vgb.yueranfly.top

[S41] C++：类与构造函数
来源：http://zzt.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://upz.mhx1999.top

[S42] C++：继承与虚函数
来源：http://sff.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://okz.sxryk.cn

[S43] C++：智能指针
来源：http://llu.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://jee.jlsjyb.cn

[S44] C++：引用传参
来源：http://kem.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://qpa.feifeiyinyue.top

[S45] C++：lambda
来源：http://olq.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://url.gaohongyu789.top

[S46] C++：函数模板
来源：http://gvh.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://moq.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://bsy.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kbl.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://wbe.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://pit.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://koe.xziqi.cn

[S49] C++：写文件
来源：http://wjx.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pdq.daxiang520.top

[S50] C++：格式化数字
来源：http://jym.jlsjyb.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rlf.jianghu66.top

[S51] C++：显式类型转换
来源：http://tmv.tanke756.top

static_cast<double>(a) / b
来源：http://wbr.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://olx.hammf.cn

int size() const noexcept { return n_; }
来源：http://pmz.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://swa.cheryme.top

std::vector<int> w = std::move(v);
来源：http://csi.zhengqikj.top

[S54] C++：异常处理
来源：http://ral.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rsr.jyoumei.cn

[S55] C++：结构化绑定
来源：http://why.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ggo.hnxiangtu.top

[S56] C++：optional
来源：http://iuq.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ins.cdnleiting.top

[S57] C++：编译期常量
来源：http://ztt.hammf.cn

constexpr int N = 10;
来源：http://xgm.fktsv.cn

[S58] C++：命名空间
来源：http://cxg.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://hcs.wangshuangyany.cn

[S59] C++：静态断言
来源：http://ckn.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jmz.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://voh.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xfv.daria6918.cn

================================================================================
来源：http://wzv.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rgf.yangfankeji.com

================================================================================
来源：http://zpi.yongpay.top

[T01] Kotlin：Hello World
来源：http://snc.zhaomingkeji.xyz

println("Hello")
来源：http://dtn.vehdjk.com

[T02] Kotlin：变量
来源：http://exl.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iav.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://qyf.hysaishi.cn

"值: $b"
来源：http://btx.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://buw.nwbrower.top

val n: String? = null;  n?.length
来源：http://nkm.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://auo.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ikh.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://dqg.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fbr.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://gfd.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pqi.yueranfly.top

[T08] Kotlin：数据类
来源：http://emd.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://lvp.pengpengdd.cyou

[T09] Kotlin：扩展函数
来源：http://bif.hywenlv.cn

fun String.exclaim() = this + "!"
来源：http://nhd.andypj.xyz

[T10] Kotlin：默认参数
来源：http://rpf.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://dvt.pycfn.com

[T11] Kotlin：协程
来源：http://wff.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vio.pycfn.com

[T12] Kotlin：解构声明
来源：http://ofw.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://zeh.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://kjf.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://noo.dianchejie.cn

[T14] Kotlin：循环
来源：http://pen.yj20258888.top

for (i in 1..10) println(i)
来源：http://sbh.tianlin.xyz

[T15] Kotlin：接口
来源：http://tiz.yuxming.cn

interface Shape { fun area(): Double }
来源：http://eeg.c1oappe.top

[T16] Swift：Hello World
来源：http://rai.vehdjk.com

print("Hello")
来源：http://wti.iojbl.cn

[T17] Swift：变量与常量
来源：http://rwu.jlsjyb.cn

var a = 1;  let b = 2
来源：http://dnj.xuanzx.com

[T18] Swift：字符串插值
来源：http://kev.yuanzhike.top

"值: \(b)"
来源：http://aat.yuxming.cn

[T19] Swift：可选绑定
来源：http://dei.aizwys.cn

if let n = opt { print(n) }
来源：http://rck.hcnkem.com

[T20] Swift：数组操作
来源：http://mfc.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://qbl.jinghuilouyu.cn

[T21] Swift：遍历
来源：http://ksj.dashuyun.cn

for x in a { print(x) }
来源：http://wrm.bbcook.cn

[T22] Swift：字典
来源：http://oxd.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://czj.hywenlv.cn

[T23] Swift：函数
来源：http://yqn.zhaomingkeji.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://njs.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://okf.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jnr.hesvh.cn

[T25] Swift：结构体
来源：http://etm.zdbjq.cn

struct P { var x: Int }
来源：http://hia.0kj1m.cn

[T26] Swift：类与重写
来源：http://tmn.shanyushiyangtech.top

class A: Base { override func f() {} }
来源：http://qyl.yangfankeji.com

[T27] Swift：错误处理
来源：http://gkp.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://bha.tianlin.xyz

[T28] Swift：枚举
来源：http://kzu.wangshuangyany.cn

enum Color { case red, green }
来源：http://fbv.pycfn.com

[T29] Swift：guard 提前返回
来源：http://vbx.tian-w.cn

guard let x = opt else { return }
来源：http://nva.52xcode.cn

[T30] Swift：协议
来源：http://bcn.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://msf.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://hea.yueranfly.top

print("Hello")
来源：http://ngb.chenlongwang.top

[T32] Lua：局部变量
来源：http://lkc.kuanghao11.cn

local a = 1
来源：http://smw.yanxiufei.cn

[T33] Lua：表（数组）
来源：http://ovj.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nzr.havefunace.top

[T34] Lua：遍历表
来源：http://vwz.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hso.shzxlz.cn

[T35] Lua：字典表
来源：http://pdg.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://qmr.guannengcc.top

[T36] Lua：函数
来源：http://qwb.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://dpl.hammf.cn

[T37] Lua：字符串拼接
来源：http://mfz.ydjk.org.cn

"a" .. "b"
来源：http://nvv.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://aub.c1oappe.top

if x > 0 then print("正") end
来源：http://gqg.tianlin.xyz

[T39] Lua：模式匹配
来源：http://kxz.wangdashe.top

string.find(s, "%d+")
来源：http://qei.xuanzx.com

[T40] Lua：元表
来源：http://lvl.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://xna.kuanghao11.cn

[T41] Perl：Hello World
来源：http://bov.redwolf501.top

print "Hello\n";
来源：http://emg.kuanghao11.cn

[T42] Perl：变量类型
来源：http://mdp.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zrl.aibaodan.cn

[T43] Perl：字符串插值
来源：http://zda.tarul.cn

"值: $a"
来源：http://sbg.jqgfzy.top

[T44] Perl：条件
来源：http://wyz.cheryme.top

if ($a > 0) { print "正"; }
来源：http://snm.jqgfzy.top

[T45] Perl：数组遍历
来源：http://kgw.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://jnu.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://hhh.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oay.xinyue.icu

[T47] Perl：正则捕获
来源：http://mhx.hongshengwenyu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://awe.fktsv.cn

[T48] Perl：正则替换
来源：http://xzs.cdnleiting.top

$s =~ s/old/new/g;
来源：http://cvi.ydzc1.top

[T49] Perl：函数
来源：http://ido.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ars.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://jff.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zrr.jqgufenzy.top

while (my $line = <$fh>) { print $line; }
来源：http://vpi.vqdsnc.cn

[T51] Scala：Hello World
来源：http://lnr.bbcook.cn

println("Hello")
来源：http://kfb.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://nsf.aizwys.cn

val a = 1;  var b = 2
来源：http://lto.shzxlz.cn

[T53] Scala：字符串插值
来源：http://tvh.feifeiyinyue.top

s"值: $b"
来源：http://xdx.fzhhl.top

[T54] Scala：集合映射
来源：http://yhf.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://glv.hfpthk.cn

[T55] Scala：集合过滤
来源：http://txe.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://shg.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://xov.yj202588.top

case class User(name: String, age: Int)
来源：http://yuc.gogol.net.cn

[T57] Scala：模式匹配
来源：http://dwz.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://won.yj20258888.top

[T58] Scala：函数定义
来源：http://dlb.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://meq.birdmap.top

[T59] Scala：循环
来源：http://emd.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://giz.guowangkeji.top

[T60] Scala：折叠
来源：http://ajw.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yee.shuidangran.top

================================================================================
来源：http://jjx.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rdl.shuidangran.top

================================================================================
来源：http://qxz.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://xrh.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vyv.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://zxi.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jbq.guowangkeji.top

[U03] Py：加载 .env 配置
来源：http://nwo.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lgn.xylfe.cn

[U04] Py：变量调试打印
来源：http://ckt.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bwc.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://epk.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://obv.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://fuk.gogol.net.cn

{**a, **b}
来源：http://ndl.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://vnr.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://ojs.sysykeji.top

[U08] Py：展平二维列表
来源：http://dzs.ydzc1.top

[y for x in nested for y in x]
来源：http://ulq.ivvv.top

[U09] Py：字典取最大值的键
来源：http://zwc.yj20258888.top

max(d, key=d.get)
来源：http://got.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://mlc.zdbjq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rhj.shuidangran.top

[U11] Py：生成器表达式
来源：http://ynf.hywenlv.cn

(x * 2 for x in arr)
来源：http://ppu.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://luq.aibaodan.cn

Counter(arr).most_common(3)
来源：http://cfk.daxiang520.top

[U13] Py：固定长度队列
来源：http://vhg.ppjwa.cn

deque(maxlen=10)
来源：http://fvi.fehbvm.com

[U14] Py：分组收集到列表
来源：http://zgr.xylfe.cn

defaultdict(list)
来源：http://lwv.redwolf501.top

[U15] Py：高精度计时
来源：http://ucz.fanxiaobao.xyz

t = time.perf_counter()
来源：http://mlr.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://lxg.cqqwz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://leu.iojbl.cn

[U17] Py：初始化日志
来源：http://xec.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://maj.cheryme.top

[U18] Py：预编译正则
来源：http://wgt.sxryk.cn

pat = re.compile(r"\d+")
来源：http://fbh.xinyue.icu

[U19] Py：正则替换带回调
来源：http://ybk.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qyd.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://hdl.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://ypx.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://ucq.aizwys.cn

@contextlib.contextmanager
来源：http://jjh.hammf.cn

[U22] Py：矩阵转置
来源：http://tyk.feifeiyinyue.top

list(zip(*m))
来源：http://qwo.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://tkl.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ibq.xuanzx.com

[U24] Py：路径操作
来源：http://xzl.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lcp.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://dgq.fktsv.cn

csv.DictReader(f)
来源：http://uzu.jyoumei.cn

[U26] Py：并发下载
来源：http://kdk.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ebo.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://khz.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://rzj.iojbl.cn

[U28] Py：类型别名
来源：http://ixk.0kj1m.cn

UserId = int
来源：http://apv.yj20258888.top

[U29] Py：属性校验
来源：http://fal.yanxiufei.cn

@property 与 @x.setter 配合
来源：http://wvn.xinyue.icu

[U30] Py：数据类
来源：http://stw.andypj.xyz

@dataclass(slots=True)
来源：http://zxp.meibo888.top

[U31] Py：单测
来源：http://jbt.xziqi.cn

python -m pytest -q
来源：http://oto.0kj1m.cn

[U32] Py：代码格式化
来源：http://dto.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://lzs.zhiwuduotai.top


<!-- 参考信息 -->