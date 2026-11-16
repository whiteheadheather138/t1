代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://foi.pycfn.com

[S10] C：指针与解引用
来源：http://epo.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://txz.shangyingyoupin.top

[S11] C：逐行读文件
来源：http://jfz.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://zgg.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://euj.yueranfly.top

fclose(f);
来源：http://wrz.uphjek.com

[S12] C：写文件
来源：http://scv.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vsq.yangfankeji.com

[S13] C：宏定义
来源：http://jan.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ryr.ydzc1.top

[S14] C：枚举
来源：http://rbg.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://knd.andypj.xyz

[S15] C：类型转换
来源：http://gmt.fehbvm.com

(double) a / b
来源：http://pih.sweek.top

[S16] C：位操作置位
来源：http://ipy.snrcjt.cn

x |= (1 << 3);
来源：http://cbe.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://daq.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ynd.yongpay.top

[S18] C：命令行参数
来源：http://geg.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://odp.fktsv.cn

[S19] C：快速排序
来源：http://gjd.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://akg.smart0.xyz

[S20] C：二分查找
来源：http://spb.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dlk.cashguo.top

[S21] C：字符类别判断
来源：http://rge.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xzm.vehdjk.com

[S22] C：字符串转数字
来源：http://vhk.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://szs.ehwqpu.com

[S23] C：随机数
来源：http://khs.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xla.fengsongda.top

[S24] C：获取本地时间
来源：http://lhd.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xxp.sjlbkw.cn

[S25] C：内存拷贝
来源：http://lcv.pycfn.com

memcpy(dst, src, n);
来源：http://hsx.wangshuangyany.cn

[S26] C：内存清零
来源：http://zxq.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://vdc.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://vfd.meibo888.top

const double PI = 3.14159;
来源：http://zsn.kuanghao11.cn

[S28] C：静态变量
来源：http://pbe.cheryme.top

static int counter = 0;
来源：http://ljv.chenzaomai.com

[S29] C：变参函数
来源：http://las.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wvc.ydjk.org.cn

[S30] C：头文件保护
来源：http://vnf.xziqi.cn

#ifndef X_H
来源：http://fwi.jinqigfzy.top

#define X_H
来源：http://jer.hammf.cn

#endif
来源：http://qcy.fehbvm.com

[S31] C++：Hello World
来源：http://glw.yj20258888.top

#include <iostream>
来源：http://rwj.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://omt.vehdjk.com

[S32] C++：字符串
来源：http://bcc.shanyushiyangtech.top

std::string s = "hi";  s += "!";
来源：http://bmv.tarul.cn

[S33] C++：vector 增删
来源：http://xrh.yvedp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lpj.yuanzhike.top

[S34] C++：遍历 vector
来源：http://vqa.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://jgm.hysaishi.cn

[S35] C++：map
来源：http://wkr.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cey.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://wmj.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tax.gotoacloud.top

[S37] C++：set
来源：http://yxe.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jym.fktsv.cn

[S38] C++：排序
来源：http://qrc.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://dtg.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://lal.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xpu.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://dtw.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gho.316326.xyz

[S41] C++：类与构造函数
来源：http://zqf.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gsg.xinyue.icu

[S42] C++：继承与虚函数
来源：http://zup.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://wkj.aizwys.cn

[S43] C++：智能指针
来源：http://tap.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://bxv.xziqi.cn

[S44] C++：引用传参
来源：http://cbe.316326.xyz

void inc(int &x) { ++x; }
来源：http://ihn.uphjek.com

[S45] C++：lambda
来源：http://rgr.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://qbw.hesvh.cn

[S46] C++：函数模板
来源：http://yuo.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nze.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://hbm.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uvg.bbcook.cn

[S48] C++：逐行读文件
来源：http://efb.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://wyn.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://cnk.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://vpm.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pic.pycfn.com

[S50] C++：格式化数字
来源：http://haz.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://esu.snrcjt.cn

[S51] C++：显式类型转换
来源：http://lwh.yj20258888.top

static_cast<double>(a) / b
来源：http://pqo.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://zlf.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://zjz.kuanghao11.cn

[S53] C++：移动语义
来源：http://zcg.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://eap.jinqigfzy.top

[S54] C++：异常处理
来源：http://ahv.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nyg.tarul.cn

[S55] C++：结构化绑定
来源：http://rrg.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zyk.zhongyouzk.top

[S56] C++：optional
来源：http://onf.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xup.chenzaomai.com

[S57] C++：编译期常量
来源：http://wpf.yj202588.top

constexpr int N = 10;
来源：http://dwn.hfpthk.cn

[S58] C++：命名空间
来源：http://ebz.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://loo.cucudq.cn

[S59] C++：静态断言
来源：http://akm.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ukq.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://ank.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jka.hysaishi.cn

================================================================================
来源：http://xpq.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://auq.birdmap.top

================================================================================
来源：http://arf.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://sue.aibaodan.cn

println("Hello")
来源：http://png.yuxming.cn

[T02] Kotlin：变量
来源：http://mtq.ehwqpu.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vhi.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://njx.guannengcc.top

"值: $b"
来源：http://ixr.birdmap.top

[T04] Kotlin：空安全
来源：http://bdy.fehbvm.com

val n: String? = null;  n?.length
来源：http://toh.havefunace.top

[T05] Kotlin：when 表达式
来源：http://svm.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dup.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://yld.yfazqb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://mtw.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://suw.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://zcz.yangfankeji.com

[T08] Kotlin：数据类
来源：http://owb.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://yen.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://vdy.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://fjc.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://odx.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rfc.kuanghao11.cn

[T11] Kotlin：协程
来源：http://ynv.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kbd.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://voc.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://zoo.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://jvm.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://isi.tarul.cn

[T14] Kotlin：循环
来源：http://zyj.shuidangran.top

for (i in 1..10) println(i)
来源：http://zcs.guannengcc.top

[T15] Kotlin：接口
来源：http://rat.ybcxt.top

interface Shape { fun area(): Double }
来源：http://bbk.yuxming.cn

[T16] Swift：Hello World
来源：http://doa.hnqzz.top

print("Hello")
来源：http://tqo.shangyingyoupin.top

[T17] Swift：变量与常量
来源：http://hab.hnxiangtu.top

var a = 1;  let b = 2
来源：http://egp.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://yvo.yanxiufei.cn

"值: \(b)"
来源：http://axu.hongshengwenyu.top

[T19] Swift：可选绑定
来源：http://uoe.hywenlv.cn

if let n = opt { print(n) }
来源：http://jem.zhongyouzk.top

[T20] Swift：数组操作
来源：http://ypm.kuanghao11.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tzp.redwolf501.top

[T21] Swift：遍历
来源：http://xxl.quarkkingdee.top

for x in a { print(x) }
来源：http://dif.yj202588.top

[T22] Swift：字典
来源：http://nmp.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://qxw.hongshengwenyu.top

[T23] Swift：函数
来源：http://lpb.fktsv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nsb.fktsv.cn

[T24] Swift：闭包
来源：http://loq.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ygv.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://jyn.cucudq.cn

struct P { var x: Int }
来源：http://emz.sweek.top

[T26] Swift：类与重写
来源：http://zpz.smart0.xyz

class A: Base { override func f() {} }
来源：http://yfc.snrcjt.cn

[T27] Swift：错误处理
来源：http://ags.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://zve.epnwcf.com

[T28] Swift：枚举
来源：http://zjd.bbcook.cn

enum Color { case red, green }
来源：http://ced.tanke756.top

[T29] Swift：guard 提前返回
来源：http://ojf.ctjpmb.com

guard let x = opt else { return }
来源：http://low.hnqzz.top

[T30] Swift：协议
来源：http://lzd.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://lrh.haohaochexian.top

[T31] Lua：Hello World
来源：http://irx.gotoacloud.top

print("Hello")
来源：http://yke.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://yei.sysykeji.top

local a = 1
来源：http://bqu.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://mop.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nkx.sysykeji.top

[T34] Lua：遍历表
来源：http://vqg.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gvi.aizwys.cn

[T35] Lua：字典表
来源：http://cvu.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://ywa.hysaishi.cn

[T36] Lua：函数
来源：http://kss.xuetiantiany.cn

function add(a, b) return a + b end
来源：http://zyc.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://vfo.ydjk.org.cn

"a" .. "b"
来源：http://qfj.yuxming.cn

[T38] Lua：条件
来源：http://kpf.hysaishi.cn

if x > 0 then print("正") end
来源：http://rbr.hammf.cn

[T39] Lua：模式匹配
来源：http://ski.daxiang520.top

string.find(s, "%d+")
来源：http://akw.hongshengwenyu.top

[T40] Lua：元表
来源：http://pze.316326.xyz

setmetatable({}, { __index = base })
来源：http://cxc.iojbl.cn

[T41] Perl：Hello World
来源：http://qfz.316326.xyz

print "Hello\n";
来源：http://eav.quarkkingdee.top

[T42] Perl：变量类型
来源：http://zhm.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bfb.vehdjk.com

[T43] Perl：字符串插值
来源：http://ljs.cucudq.cn

"值: $a"
来源：http://zme.tianlin.xyz

[T44] Perl：条件
来源：http://xyv.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://joo.shzxlz.cn

[T45] Perl：数组遍历
来源：http://xyx.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://tmw.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://bfm.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ina.yfazqb.com

[T47] Perl：正则捕获
来源：http://mxq.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xnc.sjlbkw.cn

[T48] Perl：正则替换
来源：http://zqb.epnwcf.com

$s =~ s/old/new/g;
来源：http://daq.ehwqpu.com

[T49] Perl：函数
来源：http://chk.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yrs.mhx1999.top

[T50] Perl：逐行读文件
来源：http://bfz.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tqg.quarkkingdee.top

while (my $line = <$fh>) { print $line; }
来源：http://veo.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://agu.gaohongyu789.top

println("Hello")
来源：http://gts.xinyue.icu

[T52] Scala：变量
来源：http://lme.zhongyouzk.top

val a = 1;  var b = 2
来源：http://oqq.dianchejie.cn

[T53] Scala：字符串插值
来源：http://hyk.zhongyouzk.top

s"值: $b"
来源：http://plv.jinqigufen.top

[T54] Scala：集合映射
来源：http://gxg.xziqi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ulk.shanyushiyangkeji.top

[T55] Scala：集合过滤
来源：http://ipl.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://luw.daria6918.cn

[T56] Scala：样例类
来源：http://qfz.dianchejie.cn

case class User(name: String, age: Int)
来源：http://szh.svipenyu.cn

[T57] Scala：模式匹配
来源：http://mit.jqgufenzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://oxc.aibaodan.cn

[T58] Scala：函数定义
来源：http://ygs.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kfo.jinghuilouyu.cn

[T59] Scala：循环
来源：http://vsa.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://fym.yj20258.top

[T60] Scala：折叠
来源：http://udh.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rhm.zhongyouzk.top

================================================================================
来源：http://ghq.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rjp.pycfn.com

================================================================================
来源：http://ikr.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://ufd.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://plf.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://pkt.sweek.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ahk.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://zgw.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jzl.nwbrower.top

[U04] Py：变量调试打印
来源：http://yqc.quarkkingdee.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vqr.xylfe.cn

[U05] Py：列表去重且保序
来源：http://bqq.gzhubu.top

list(dict.fromkeys(arr))
来源：http://tdm.yonumen.top

[U06] Py：合并两个字典
来源：http://hnl.ydzc1.top

{**a, **b}
来源：http://ouy.cashguo.top

[U07] Py：反转字典键值
来源：http://bsx.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://xjr.jianghu66.top

[U08] Py：展平二维列表
来源：http://dul.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://xjm.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://ois.smart0.xyz

max(d, key=d.get)
来源：http://coy.fengsongda.top

[U10] Py：按值排序字典
来源：http://thc.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ybp.hfpthk.cn

[U11] Py：生成器表达式
来源：http://lrv.tarul.cn

(x * 2 for x in arr)
来源：http://dbn.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mtt.xuanzx.com

Counter(arr).most_common(3)
来源：http://lrt.quarkkingdee.top

[U13] Py：固定长度队列
来源：http://zqm.cashguo.top

deque(maxlen=10)
来源：http://rrz.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://gre.fengsongda.top

defaultdict(list)
来源：http://fyv.sxryk.cn

[U15] Py：高精度计时
来源：http://hmq.cdnleiting.top

t = time.perf_counter()
来源：http://dtr.zycfv.cn

[U16] Py：命令行参数解析
来源：http://qot.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rjw.tianlin.xyz

[U17] Py：初始化日志
来源：http://bou.havefunace.top

logging.basicConfig(level=logging.INFO)
来源：http://wqi.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://bpw.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://mmz.xziqi.cn

[U19] Py：正则替换带回调
来源：http://nzl.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ttm.52xcode.cn

[U20] Py：缓存函数结果
来源：http://isq.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://vip.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://rti.ctjpmb.com

@contextlib.contextmanager
来源：http://mil.yangfankeji.com

[U22] Py：矩阵转置
来源：http://pos.cucudq.cn

list(zip(*m))
来源：http://hdz.daria6918.cn

[U23] Py：分块读取大文件
来源：http://rtv.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ejp.svipenyu.cn

[U24] Py：路径操作
来源：http://fap.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iea.sweek.top

[U25] Py：CSV 按字典读
来源：http://izx.andypj.xyz

csv.DictReader(f)
来源：http://slu.gogol.net.cn

[U26] Py：并发下载
来源：http://jet.tarul.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xkf.epnwcf.com

[U27] Py：异步 HTTP
来源：http://ird.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://wgl.hcnkem.com

[U28] Py：类型别名
来源：http://iim.andypj.xyz

UserId = int
来源：http://cwt.hysaishi.cn

[U29] Py：属性校验
来源：http://wvd.ybcxt.top

@property 与 @x.setter 配合
来源：http://ukl.chenzaomai.com

[U30] Py：数据类
来源：http://tfg.jinqigufen.top

@dataclass(slots=True)
来源：http://ims.ehwqpu.com

[U31] Py：单测
来源：http://bye.pycfn.com

python -m pytest -q
来源：http://npu.ybcxt.top

[U32] Py：代码格式化
来源：http://wnv.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://uve.guowangkeji.top


<!-- 参考信息 -->