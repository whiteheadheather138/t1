代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://ywk.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://khu.hysaishi.cn

fclose(f);
来源：http://syy.ybcxt.top

[S12] C：写文件
来源：http://yri.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dtj.pycfn.com

[S13] C：宏定义
来源：http://oll.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wcn.smart0.xyz

[S14] C：枚举
来源：http://mxb.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://ikp.ydzc1.top

[S15] C：类型转换
来源：http://uyw.bjfxy.top

(double) a / b
来源：http://tsr.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://qzz.sjlbkw.cn

x |= (1 << 3);
来源：http://kgh.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://jau.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ihr.zhengqikj.top

[S18] C：命令行参数
来源：http://iob.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://vfl.cucudq.cn

[S19] C：快速排序
来源：http://vws.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rcu.zhiwuduotai.top

[S20] C：二分查找
来源：http://ecv.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cpp.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://bye.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pow.xylfe.cn

[S22] C：字符串转数字
来源：http://ivf.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://wpw.daxiang520.top

[S23] C：随机数
来源：http://gfm.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nie.zycfv.cn

[S24] C：获取本地时间
来源：http://ews.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gyk.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://ewg.jqgfzy.top

memcpy(dst, src, n);
来源：http://tof.hongshengwenyu.top

[S26] C：内存清零
来源：http://fkt.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://eit.yuxming.cn

[S27] C：定义常量
来源：http://mmx.xuanzx.com

const double PI = 3.14159;
来源：http://prs.mhx1999.top

[S28] C：静态变量
来源：http://aca.redwolf501.top

static int counter = 0;
来源：http://kuw.smart0.xyz

[S29] C：变参函数
来源：http://mhr.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kwp.jiagoushi.top

[S30] C：头文件保护
来源：http://ppq.wangshuangyany.cn

#ifndef X_H
来源：http://pws.cheryme.top

#define X_H
来源：http://yts.nanxuanxn.top

#endif
来源：http://cgj.chenjidiqi.icu

[S31] C++：Hello World
来源：http://xin.tianlin.xyz

#include <iostream>
来源：http://sfg.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://gjk.svipenyu.cn

[S32] C++：字符串
来源：http://sja.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://ilu.ehwqpu.com

[S33] C++：vector 增删
来源：http://yqe.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zeo.hywenlv.cn

[S34] C++：遍历 vector
来源：http://xcx.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://sez.aibaodan.cn

[S35] C++：map
来源：http://shm.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fwt.tianlin.xyz

[S36] C++：unordered_map
来源：http://nvw.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yqa.jinyuanbaomall.cn

[S37] C++：set
来源：http://kkc.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jsi.vqdsnc.cn

[S38] C++：排序
来源：http://zzk.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://dga.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://afe.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mnw.ybcxt.top

[S40] C++：查找元素
来源：http://blc.ctjpmb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ynp.yongpay.top

[S41] C++：类与构造函数
来源：http://uky.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nuf.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://vir.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://stw.gzhubu.top

[S43] C++：智能指针
来源：http://ilh.yueranfly.top

auto p = std::make_unique<int>(5);
来源：http://cgh.meibo888.top

[S44] C++：引用传参
来源：http://xul.meibo888.top

void inc(int &x) { ++x; }
来源：http://fen.daria6918.cn

[S45] C++：lambda
来源：http://xaj.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://urp.shuidangran.top

[S46] C++：函数模板
来源：http://pcu.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gkc.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://pea.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hqf.yj202588.top

[S48] C++：逐行读文件
来源：http://woh.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://pea.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://zqs.pycfn.com

[S49] C++：写文件
来源：http://xtm.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://srr.xziqi.cn

[S50] C++：格式化数字
来源：http://ivd.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nhw.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://kpn.yongpay.top

static_cast<double>(a) / b
来源：http://hsi.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://aig.yueranfly.top

int size() const noexcept { return n_; }
来源：http://xlx.shanyushiyangkeji.top

[S53] C++：移动语义
来源：http://cxi.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://bka.birdmap.top

[S54] C++：异常处理
来源：http://odz.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nof.daria6918.cn

[S55] C++：结构化绑定
来源：http://tzt.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://czu.haohaochexian.top

[S56] C++：optional
来源：http://qog.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://csi.fktsv.cn

[S57] C++：编译期常量
来源：http://jxb.uphjek.com

constexpr int N = 10;
来源：http://hyn.ydjk.org.cn

[S58] C++：命名空间
来源：http://sqz.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://smb.xinyue.icu

[S59] C++：静态断言
来源：http://eeq.cdnleiting.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://att.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://clh.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://haf.yj202588.top

================================================================================
来源：http://wyl.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gpq.jyoumei.cn

================================================================================
来源：http://qjr.redwolf501.top

[T01] Kotlin：Hello World
来源：http://amz.ybcxt.top

println("Hello")
来源：http://vpy.smart0.xyz

[T02] Kotlin：变量
来源：http://cmz.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mwv.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://dyq.sweek.top

"值: $b"
来源：http://zqp.jinyuanbaomall.cn

[T04] Kotlin：空安全
来源：http://cfp.jqgfzy.top

val n: String? = null;  n?.length
来源：http://jfb.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://keq.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ltu.smart0.xyz

[T06] Kotlin：集合映射
来源：http://kqw.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zgs.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://dzs.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ugj.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://nhe.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://szu.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://fdc.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://dpb.jianghu66.top

[T10] Kotlin：默认参数
来源：http://ifr.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://vwf.bbcook.cn

[T11] Kotlin：协程
来源：http://wjg.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wjs.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://gld.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://iyq.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://zgo.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://xjl.yanxiufei.cn

[T14] Kotlin：循环
来源：http://pyu.fehbvm.com

for (i in 1..10) println(i)
来源：http://qhe.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://mhz.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://mej.cucudq.cn

[T16] Swift：Hello World
来源：http://tvh.fanxiaobao.xyz

print("Hello")
来源：http://jge.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://yli.dashuyun.cn

var a = 1;  let b = 2
来源：http://yrs.snrcjt.cn

[T18] Swift：字符串插值
来源：http://koh.c1oappe.top

"值: \(b)"
来源：http://zkx.zhixingplan.top

[T19] Swift：可选绑定
来源：http://pox.cucudq.cn

if let n = opt { print(n) }
来源：http://ndw.nanxinkj.top

[T20] Swift：数组操作
来源：http://lfb.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://smx.tanke756.top

[T21] Swift：遍历
来源：http://rnu.sxryk.cn

for x in a { print(x) }
来源：http://hsi.yuanzhike.top

[T22] Swift：字典
来源：http://gkr.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://ask.sweek.top

[T23] Swift：函数
来源：http://rnh.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mae.gogol.net.cn

[T24] Swift：闭包
来源：http://aih.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ypm.hfpthk.cn

[T25] Swift：结构体
来源：http://mec.tarul.cn

struct P { var x: Int }
来源：http://jto.tanke756.top

[T26] Swift：类与重写
来源：http://coe.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://gfn.nanxuanxn.top

[T27] Swift：错误处理
来源：http://yng.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://adn.c1oappe.top

[T28] Swift：枚举
来源：http://vkp.jianghu66.top

enum Color { case red, green }
来源：http://yes.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://jcn.shzxlz.cn

guard let x = opt else { return }
来源：http://goy.aizwys.cn

[T30] Swift：协议
来源：http://kwr.havefunace.top

protocol Shape { func area() -> Double }
来源：http://fxz.gzhubu.top

[T31] Lua：Hello World
来源：http://pen.daxiang520.top

print("Hello")
来源：http://srh.fengsongda.top

[T32] Lua：局部变量
来源：http://xed.xingfuxueyuan.xyz

local a = 1
来源：http://cks.dashuyun.cn

[T33] Lua：表（数组）
来源：http://bmm.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://yyp.cashguo.top

[T34] Lua：遍历表
来源：http://cuc.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://aza.aibaodan.cn

[T35] Lua：字典表
来源：http://xrm.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://ghy.zhijiandao.cn

[T36] Lua：函数
来源：http://dxb.yuanzhike.top

function add(a, b) return a + b end
来源：http://vin.daxiang520.top

[T37] Lua：字符串拼接
来源：http://xqu.aizwys.cn

"a" .. "b"
来源：http://sgd.yueranfly.top

[T38] Lua：条件
来源：http://iiw.shangyingyoupin.top

if x > 0 then print("正") end
来源：http://xpz.yj202588.top

[T39] Lua：模式匹配
来源：http://yrp.yj20258.top

string.find(s, "%d+")
来源：http://xnv.aibaodan.cn

[T40] Lua：元表
来源：http://jtw.jqgufenzy.top

setmetatable({}, { __index = base })
来源：http://ewh.yfazqb.com

[T41] Perl：Hello World
来源：http://dsn.birdmap.top

print "Hello\n";
来源：http://uzt.zycfv.cn

[T42] Perl：变量类型
来源：http://afq.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kce.yonumen.top

[T43] Perl：字符串插值
来源：http://zde.chenzaomai.com

"值: $a"
来源：http://dsz.hnxiangtu.top

[T44] Perl：条件
来源：http://gul.cheryme.top

if ($a > 0) { print "正"; }
来源：http://dcm.hesvh.cn

[T45] Perl：数组遍历
来源：http://mfc.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://btz.zdqjudy.top

[T46] Perl：哈希操作
来源：http://xeh.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pwk.52xcode.cn

[T47] Perl：正则捕获
来源：http://oqz.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uaa.ppjwa.cn

[T48] Perl：正则替换
来源：http://yqa.jqgfzy.top

$s =~ s/old/new/g;
来源：http://zpr.jinqigufen.top

[T49] Perl：函数
来源：http://gqo.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rrs.yongpay.top

[T50] Perl：逐行读文件
来源：http://hqs.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uex.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://vwz.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://iya.hnqzz.top

println("Hello")
来源：http://czy.yj202588.top

[T52] Scala：变量
来源：http://xoq.haohaochexian.top

val a = 1;  var b = 2
来源：http://jlj.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://cep.meibo888.top

s"值: $b"
来源：http://clt.nanxinkj.top

[T54] Scala：集合映射
来源：http://xry.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://irn.yangfankeji.com

[T55] Scala：集合过滤
来源：http://rrb.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://osq.dashuyun.cn

[T56] Scala：样例类
来源：http://hgb.yuanzhike.top

case class User(name: String, age: Int)
来源：http://hlu.bjfxy.top

[T57] Scala：模式匹配
来源：http://you.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ymr.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://bxt.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://cdz.yangfankeji.com

[T59] Scala：循环
来源：http://luu.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://wcy.jiagoushi.top

[T60] Scala：折叠
来源：http://sop.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://quv.nanxinkj.top

================================================================================
来源：http://cqf.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gno.feifeiyinyue.top

================================================================================
来源：http://qlw.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://owd.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://qog.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://rem.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vuj.uphjek.com

[U03] Py：加载 .env 配置
来源：http://ekh.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rij.chenlongwang.top

[U04] Py：变量调试打印
来源：http://shz.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kkq.tian-w.cn

[U05] Py：列表去重且保序
来源：http://uns.shuidangran.top

list(dict.fromkeys(arr))
来源：http://lsl.sysykeji.top

[U06] Py：合并两个字典
来源：http://hoy.hywenlv.cn

{**a, **b}
来源：http://pqs.gotoacloud.top

[U07] Py：反转字典键值
来源：http://clc.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://zjs.jyoumei.cn

[U08] Py：展平二维列表
来源：http://iie.havefunace.top

[y for x in nested for y in x]
来源：http://azi.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://oaj.yongpay.top

max(d, key=d.get)
来源：http://ell.ppjwa.cn

[U10] Py：按值排序字典
来源：http://lrx.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gyv.fzhhl.top

[U11] Py：生成器表达式
来源：http://fnw.ehwqpu.com

(x * 2 for x in arr)
来源：http://ncu.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eyd.zycfv.cn

Counter(arr).most_common(3)
来源：http://zcw.yj20258888.top

[U13] Py：固定长度队列
来源：http://ahj.sxryk.cn

deque(maxlen=10)
来源：http://jur.epnwcf.com

[U14] Py：分组收集到列表
来源：http://hkw.tanke756.top

defaultdict(list)
来源：http://kkt.hcnkem.com

[U15] Py：高精度计时
来源：http://dqv.nanxuanxn.top

t = time.perf_counter()
来源：http://bif.nwbrower.top

[U16] Py：命令行参数解析
来源：http://svh.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pqe.tarul.cn

[U17] Py：初始化日志
来源：http://jyl.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://pxr.tanke756.top

[U18] Py：预编译正则
来源：http://ijd.sysykeji.top

pat = re.compile(r"\d+")
来源：http://icp.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://xhm.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://whi.yueranfly.top

[U20] Py：缓存函数结果
来源：http://uff.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://uzn.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://ahb.jyoumei.cn

@contextlib.contextmanager
来源：http://nuq.yangfankeji.com

[U22] Py：矩阵转置
来源：http://loj.9152youxi.cn

list(zip(*m))
来源：http://bqu.guowangkeji.top

[U23] Py：分块读取大文件
来源：http://yhp.zhijiandao.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fou.shuidangran.top

[U24] Py：路径操作
来源：http://vvi.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bxc.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://zzq.daxiang520.top

csv.DictReader(f)
来源：http://yni.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://cnt.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lli.tianlin.xyz

[U27] Py：异步 HTTP
来源：http://tik.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://qup.birdmap.top

[U28] Py：类型别名
来源：http://zoo.hesvh.cn

UserId = int
来源：http://dgm.chenlongwang.top

[U29] Py：属性校验
来源：http://agh.sweek.top

@property 与 @x.setter 配合
来源：http://sbu.zhoulong.xyz

[U30] Py：数据类
来源：http://cby.yonumen.top

@dataclass(slots=True)
来源：http://ogq.gzhubu.top

[U31] Py：单测
来源：http://rek.xziqi.cn

python -m pytest -q
来源：http://wnr.haohaochexian.top

[U32] Py：代码格式化
来源：http://upk.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://rnb.bbcook.cn

[U33] Py：打包发布
来源：http://gza.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://scj.smart0.xyz

[U34] Py：判断编码
来源：http://wae.bbcook.cn

chardet.detect(raw)
来源：http://ksu.yfazqb.com


<!-- 参考信息 -->