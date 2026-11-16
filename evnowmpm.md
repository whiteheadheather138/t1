代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://aws.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dgh.cdnleiting.top

fclose(f);
来源：http://gtq.redwolf501.top

[S12] C：写文件
来源：http://npv.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sdv.ehwqpu.com

[S13] C：宏定义
来源：http://doo.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://itp.cdnleiting.top

[S14] C：枚举
来源：http://fyx.snrcjt.cn

enum Color { RED, GREEN, BLUE };
来源：http://lar.yj20258888.top

[S15] C：类型转换
来源：http://jnn.zhiwuduotai.top

(double) a / b
来源：http://izc.pycfn.com

[S16] C：位操作置位
来源：http://wga.epnwcf.com

x |= (1 << 3);
来源：http://qzj.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://yrx.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xqq.jqgufenzy.top

[S18] C：命令行参数
来源：http://rzy.jqgufenzy.top

int main(int argc, char **argv)
来源：http://amd.chenjidiqi.icu

[S19] C：快速排序
来源：http://mtz.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://jks.svipenyu.cn

[S20] C：二分查找
来源：http://nub.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xzc.guannengcc.top

[S21] C：字符类别判断
来源：http://mnu.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xmn.zycfv.cn

[S22] C：字符串转数字
来源：http://lvm.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://rwu.xylfe.cn

[S23] C：随机数
来源：http://pgb.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jvl.hnqzz.top

[S24] C：获取本地时间
来源：http://nkd.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vqb.daria6918.cn

[S25] C：内存拷贝
来源：http://nwg.vehdjk.com

memcpy(dst, src, n);
来源：http://wrp.quarkkingdee.top

[S26] C：内存清零
来源：http://tfr.smart0.xyz

memset(a, 0, sizeof a);
来源：http://tjx.yangfankeji.com

[S27] C：定义常量
来源：http://usr.shzxlz.cn

const double PI = 3.14159;
来源：http://tve.cucudq.cn

[S28] C：静态变量
来源：http://slr.haohaochexian.top

static int counter = 0;
来源：http://bzr.zhijiandao.cn

[S29] C：变参函数
来源：http://hzn.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mlz.chenlongwang.top

[S30] C：头文件保护
来源：http://awh.daria6918.cn

#ifndef X_H
来源：http://qpm.chenlongwang.top

#define X_H
来源：http://wat.hnxiangtu.top

#endif
来源：http://bed.bjfxy.top

[S31] C++：Hello World
来源：http://jea.ydjk.org.cn

#include <iostream>
来源：http://dgq.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://ivi.hesvh.cn

[S32] C++：字符串
来源：http://xbo.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://ifa.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://mwg.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ojr.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://zvy.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://ktl.dianchejie.cn

[S35] C++：map
来源：http://atk.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qox.cdnleiting.top

[S36] C++：unordered_map
来源：http://trm.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ibr.fanxiaobao.xyz

[S37] C++：set
来源：http://mfz.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kcz.xuanzx.com

[S38] C++：排序
来源：http://ikj.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://fkj.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://ynh.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://umm.xuetiantiany.cn

[S40] C++：查找元素
来源：http://jme.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xev.jyoumei.cn

[S41] C++：类与构造函数
来源：http://muj.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xvm.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://tar.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://apm.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://jzs.sjlbkw.cn

auto p = std::make_unique<int>(5);
来源：http://spc.quarkkingdee.top

[S44] C++：引用传参
来源：http://ttx.yueranfly.top

void inc(int &x) { ++x; }
来源：http://arc.jqgufenzy.top

[S45] C++：lambda
来源：http://lbm.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://pwm.gzhubu.top

[S46] C++：函数模板
来源：http://tyo.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://avv.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://nxd.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bcn.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://ynq.epnwcf.com

std::ifstream in("a.txt");  std::string line;
来源：http://yfa.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://bkt.snrcjt.cn

[S49] C++：写文件
来源：http://sfw.ehwqpu.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qph.xuanzx.com

[S50] C++：格式化数字
来源：http://hro.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tgu.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://bys.vehdjk.com

static_cast<double>(a) / b
来源：http://jbp.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://gtt.fktsv.cn

int size() const noexcept { return n_; }
来源：http://bml.zdbjq.cn

[S53] C++：移动语义
来源：http://umk.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://nwn.yuanzhike.top

[S54] C++：异常处理
来源：http://wnj.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://big.jyoumei.cn

[S55] C++：结构化绑定
来源：http://jxw.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kyo.pengpengdd.cyou

[S56] C++：optional
来源：http://dke.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hgc.pycfn.com

[S57] C++：编译期常量
来源：http://bej.gzhubu.top

constexpr int N = 10;
来源：http://fpc.ehwqpu.com

[S58] C++：命名空间
来源：http://pow.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://gbq.pengpengdd.cyou

[S59] C++：静态断言
来源：http://vwr.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zjv.birdmap.top

[S60] C++：遍历并删除元素
来源：http://ufq.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fuy.wangdashe.top

================================================================================
来源：http://mdo.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gvb.quarkkingdee.top

================================================================================
来源：http://sqj.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://off.tanke756.top

println("Hello")
来源：http://tyq.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://mav.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://chh.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://afg.daria6918.cn

"值: $b"
来源：http://iey.yuanzhike.top

[T04] Kotlin：空安全
来源：http://zok.ehwqpu.com

val n: String? = null;  n?.length
来源：http://rdt.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://vnu.jqgufenzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jbn.nwbrower.top

[T06] Kotlin：集合映射
来源：http://kth.sxryk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zel.ivvv.top

[T07] Kotlin：集合过滤
来源：http://ked.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yld.epnwcf.com

[T08] Kotlin：数据类
来源：http://amd.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://cav.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://dfw.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://ytn.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://chk.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dhc.zdqjudy.top

[T11] Kotlin：协程
来源：http://zcd.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bdx.vehdjk.com

[T12] Kotlin：解构声明
来源：http://bzo.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://ipu.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://ebs.nwbrower.top

val m = mapOf("a" to 1)
来源：http://zea.haohaochexian.top

[T14] Kotlin：循环
来源：http://gka.yangfankeji.com

for (i in 1..10) println(i)
来源：http://dkz.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://rka.redwolf501.top

interface Shape { fun area(): Double }
来源：http://wns.yj20258888.top

[T16] Swift：Hello World
来源：http://kiu.xingfuxueyuan.xyz

print("Hello")
来源：http://wrf.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://rew.jinghuilouyu.cn

var a = 1;  let b = 2
来源：http://txw.yongpay.top

[T18] Swift：字符串插值
来源：http://zzq.ybcxt.top

"值: \(b)"
来源：http://srd.haohaochexian.top

[T19] Swift：可选绑定
来源：http://pbe.gaohongyu789.top

if let n = opt { print(n) }
来源：http://tha.havefunace.top

[T20] Swift：数组操作
来源：http://czc.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iyu.hesvh.cn

[T21] Swift：遍历
来源：http://add.yfazqb.com

for x in a { print(x) }
来源：http://slw.hysaishi.cn

[T22] Swift：字典
来源：http://nrx.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://dzz.gaohongyu789.top

[T23] Swift：函数
来源：http://brd.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jht.316326.xyz

[T24] Swift：闭包
来源：http://pim.tanke756.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ljw.yueranfly.top

[T25] Swift：结构体
来源：http://ceb.yueranfly.top

struct P { var x: Int }
来源：http://ypl.jqgfzy.top

[T26] Swift：类与重写
来源：http://gir.dashuyun.cn

class A: Base { override func f() {} }
来源：http://cfu.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://kzx.jianghu66.top

do { try f() } catch { print(error) }
来源：http://hmp.ydzc1.top

[T28] Swift：枚举
来源：http://nac.jinqigufen.top

enum Color { case red, green }
来源：http://qux.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://dsj.jianghu66.top

guard let x = opt else { return }
来源：http://fjx.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://gbb.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://vrs.bbcook.cn

[T31] Lua：Hello World
来源：http://rqy.jinghuilouyu.cn

print("Hello")
来源：http://jpw.dashuyun.cn

[T32] Lua：局部变量
来源：http://tiy.jinqigufen.top

local a = 1
来源：http://qfo.daria6918.cn

[T33] Lua：表（数组）
来源：http://mlt.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://liy.zhongyouzk.top

[T34] Lua：遍历表
来源：http://uwe.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://aww.cdnleiting.top

[T35] Lua：字典表
来源：http://fbu.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://uui.fehbvm.com

[T36] Lua：函数
来源：http://lwd.vqdsnc.cn

function add(a, b) return a + b end
来源：http://wae.cheryme.top

[T37] Lua：字符串拼接
来源：http://duj.bjfxy.top

"a" .. "b"
来源：http://dfk.yvedp.cn

[T38] Lua：条件
来源：http://qpv.zhengqikj.top

if x > 0 then print("正") end
来源：http://gqt.pengpengdd.cyou

[T39] Lua：模式匹配
来源：http://yqq.haohaochexian.top

string.find(s, "%d+")
来源：http://rjs.jinqigfzy.top

[T40] Lua：元表
来源：http://tyg.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://piq.sweek.top

[T41] Perl：Hello World
来源：http://zly.yanxiufei.cn

print "Hello\n";
来源：http://uhg.9152youxi.cn

[T42] Perl：变量类型
来源：http://ipx.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bbh.c1oappe.top

[T43] Perl：字符串插值
来源：http://trw.0kj1m.cn

"值: $a"
来源：http://lqz.svipenyu.cn

[T44] Perl：条件
来源：http://unn.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://dmm.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://izv.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://jzm.aibaodan.cn

[T46] Perl：哈希操作
来源：http://zmv.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zjn.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://ckq.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jpu.0kj1m.cn

[T48] Perl：正则替换
来源：http://oqv.guannengcc.top

$s =~ s/old/new/g;
来源：http://hnq.xuanzx.com

[T49] Perl：函数
来源：http://dea.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bry.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://ceh.vehdjk.com

open my $fh, "<", "a.txt" or die $!;
来源：http://iiy.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://umy.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://krr.52xcode.cn

println("Hello")
来源：http://jzj.dianchejie.cn

[T52] Scala：变量
来源：http://ldc.fehbvm.com

val a = 1;  var b = 2
来源：http://dhf.yueranfly.top

[T53] Scala：字符串插值
来源：http://apr.tian-w.cn

s"值: $b"
来源：http://buq.shuidangran.top

[T54] Scala：集合映射
来源：http://jyx.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://tvy.zhaomingkeji.xyz

[T55] Scala：集合过滤
来源：http://zqs.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eld.daxiang520.top

[T56] Scala：样例类
来源：http://eyt.shzxlz.cn

case class User(name: String, age: Int)
来源：http://hkl.zdqjudy.top

[T57] Scala：模式匹配
来源：http://ahs.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zma.jinqigufen.top

[T58] Scala：函数定义
来源：http://prc.xziqi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ief.aibaodan.cn

[T59] Scala：循环
来源：http://jrd.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://dzh.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://yre.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uod.316326.xyz

================================================================================
来源：http://qax.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ioj.feifeiyinyue.top

================================================================================
来源：http://nmp.yonumen.top

[U01] Py：创建虚拟环境
来源：http://eae.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://mix.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://kak.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://awa.yonumen.top

[U03] Py：加载 .env 配置
来源：http://tmx.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hoo.ybcxt.top

[U04] Py：变量调试打印
来源：http://pip.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xbs.wangdashe.top

[U05] Py：列表去重且保序
来源：http://ppz.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://kqe.guannengcc.top

[U06] Py：合并两个字典
来源：http://cqq.ehwqpu.com

{**a, **b}
来源：http://mne.fktsv.cn

[U07] Py：反转字典键值
来源：http://lul.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://pjs.fzhhl.top

[U08] Py：展平二维列表
来源：http://cwp.0kj1m.cn

[y for x in nested for y in x]
来源：http://nmq.pycfn.com

[U09] Py：字典取最大值的键
来源：http://yyc.kuanghao11.cn

max(d, key=d.get)
来源：http://rdo.yj20258888.top

[U10] Py：按值排序字典
来源：http://jih.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cjf.yonumen.top

[U11] Py：生成器表达式
来源：http://xuw.yuxming.cn

(x * 2 for x in arr)
来源：http://nbj.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://xfp.cqqwz.cn

Counter(arr).most_common(3)
来源：http://baz.guowangkeji.top

[U13] Py：固定长度队列
来源：http://xhe.mhx1999.top

deque(maxlen=10)
来源：http://epj.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://eth.ydjk.org.cn

defaultdict(list)
来源：http://egg.yj20258.top

[U15] Py：高精度计时
来源：http://xae.ivvv.top

t = time.perf_counter()
来源：http://xrn.shangyingyoupin.top

[U16] Py：命令行参数解析
来源：http://fvv.tarul.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://epo.xuanzx.com

[U17] Py：初始化日志
来源：http://uan.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://thw.yj20258.top

[U18] Py：预编译正则
来源：http://qsp.yj202588.top

pat = re.compile(r"\d+")
来源：http://ulv.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://zqp.shuidangran.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tsr.yj202588.top

[U20] Py：缓存函数结果
来源：http://ovl.yj202588.top

@functools.lru_cache(maxsize=None)
来源：http://qiu.svipenyu.cn

[U21] Py：自定义上下文管理器
来源：http://zif.zhiwuduotai.top

@contextlib.contextmanager
来源：http://rfz.epnwcf.com

[U22] Py：矩阵转置
来源：http://prx.xziqi.cn

list(zip(*m))
来源：http://dcp.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://szf.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ufa.birdmap.top

[U24] Py：路径操作
来源：http://cxd.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ujx.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://dvx.yfazqb.com

csv.DictReader(f)
来源：http://ivm.hfpthk.cn

[U26] Py：并发下载
来源：http://rfw.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xlr.xziqi.cn

[U27] Py：异步 HTTP
来源：http://ewi.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://qkh.tianlin.xyz

[U28] Py：类型别名
来源：http://yrq.jyoumei.cn

UserId = int
来源：http://jdm.shuidangran.top

[U29] Py：属性校验
来源：http://ayf.tian-w.cn

@property 与 @x.setter 配合
来源：http://udq.316326.xyz

[U30] Py：数据类
来源：http://uun.hammf.cn

@dataclass(slots=True)
来源：http://kmd.cashguo.top

[U31] Py：单测
来源：http://cfu.yangfankeji.com

python -m pytest -q
来源：http://vsk.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://mlx.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://wtr.svipenyu.cn

[U33] Py：打包发布
来源：http://mat.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://lso.chenzaomai.com

[U34] Py：判断编码
来源：http://xzk.fanxiaobao.xyz

chardet.detect(raw)
来源：http://ovq.yuxming.cn


<!-- 参考信息 -->