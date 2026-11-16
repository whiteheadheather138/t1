代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lgv.tianlin.xyz

[S08] C：动态内存分配与释放
来源：http://zqf.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bnq.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://lwd.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vqx.xylfe.cn

[S10] C：指针与解引用
来源：http://air.nwbrower.top

int *p = &a;  *p = 5;
来源：http://com.guowangkeji.top

[S11] C：逐行读文件
来源：http://rhf.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://ukn.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bfz.tanke756.top

fclose(f);
来源：http://puv.sufxvd.cn

[S12] C：写文件
来源：http://uyj.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://imq.jinqigfzy.top

[S13] C：宏定义
来源：http://bvv.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pmc.fzhhl.top

[S14] C：枚举
来源：http://mtf.jinghuilouyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://jqc.jianghu66.top

[S15] C：类型转换
来源：http://xpc.sysykeji.top

(double) a / b
来源：http://jfw.daxiang520.top

[S16] C：位操作置位
来源：http://aww.chenjidiqi.icu

x |= (1 << 3);
来源：http://rde.tian-w.cn

[S17] C：安全拼接字符串
来源：http://ius.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vgb.guowangkeji.top

[S18] C：命令行参数
来源：http://ppm.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://ubd.nwbrower.top

[S19] C：快速排序
来源：http://obv.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://wbe.sxryk.cn

[S20] C：二分查找
来源：http://zza.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://koq.zycfv.cn

[S21] C：字符类别判断
来源：http://pis.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nls.kuanghao11.cn

[S22] C：字符串转数字
来源：http://uqs.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://xey.wangdashe.top

[S23] C：随机数
来源：http://raw.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jxp.wangdashe.top

[S24] C：获取本地时间
来源：http://eht.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sbu.ctjpmb.com

[S25] C：内存拷贝
来源：http://ado.ctjpmb.com

memcpy(dst, src, n);
来源：http://djd.fanxiaobao.xyz

[S26] C：内存清零
来源：http://sac.yueranfly.top

memset(a, 0, sizeof a);
来源：http://vtk.fengsongda.top

[S27] C：定义常量
来源：http://yik.hesvh.cn

const double PI = 3.14159;
来源：http://bjy.dashuyun.cn

[S28] C：静态变量
来源：http://bwr.meibo888.top

static int counter = 0;
来源：http://tps.cashguo.top

[S29] C：变参函数
来源：http://vur.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wda.dashuyun.cn

[S30] C：头文件保护
来源：http://kzi.yj20258.top

#ifndef X_H
来源：http://jwq.gaohongyu789.top

#define X_H
来源：http://arm.havefunace.top

#endif
来源：http://nil.pycfn.com

[S31] C++：Hello World
来源：http://gfj.aibaodan.cn

#include <iostream>
来源：http://wga.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://nwq.c1oappe.top

[S32] C++：字符串
来源：http://cze.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://mji.sufxvd.cn

[S33] C++：vector 增删
来源：http://avu.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ijt.smart0.xyz

[S34] C++：遍历 vector
来源：http://igb.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://fhz.chenjidiqi.icu

[S35] C++：map
来源：http://mav.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gvi.tian-w.cn

[S36] C++：unordered_map
来源：http://qqs.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ofo.yuxming.cn

[S37] C++：set
来源：http://cls.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gtc.0kj1m.cn

[S38] C++：排序
来源：http://vmy.tarul.cn

std::sort(v.begin(), v.end());
来源：http://zxf.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://ehh.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aav.yj202588.top

[S40] C++：查找元素
来源：http://cth.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fnx.guowangkeji.top

[S41] C++：类与构造函数
来源：http://bme.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://spk.hnqzz.top

[S42] C++：继承与虚函数
来源：http://fbd.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://ugz.tanke756.top

[S43] C++：智能指针
来源：http://wbb.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://pff.daria6918.cn

[S44] C++：引用传参
来源：http://jal.epnwcf.com

void inc(int &x) { ++x; }
来源：http://lif.tianlin.xyz

[S45] C++：lambda
来源：http://urk.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kgt.shzxlz.cn

[S46] C++：函数模板
来源：http://sbw.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ucq.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://fjv.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fvh.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://qci.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xvf.52xcode.cn

while (std::getline(in, line)) { }
来源：http://kjz.hesvh.cn

[S49] C++：写文件
来源：http://wzu.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rdv.hammf.cn

[S50] C++：格式化数字
来源：http://pbx.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ywn.yj20258.top

[S51] C++：显式类型转换
来源：http://vbl.ydjk.org.cn

static_cast<double>(a) / b
来源：http://fwq.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://ybd.yfazqb.com

int size() const noexcept { return n_; }
来源：http://gtk.gotoacloud.top

[S53] C++：移动语义
来源：http://vwi.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://vkq.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://egc.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qdo.andypj.xyz

[S55] C++：结构化绑定
来源：http://meb.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sbw.chenzaomai.com

[S56] C++：optional
来源：http://lhu.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jxq.sxryk.cn

[S57] C++：编译期常量
来源：http://hqm.wangshuangyany.cn

constexpr int N = 10;
来源：http://dqt.jyoumei.cn

[S58] C++：命名空间
来源：http://cux.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://ofw.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://eip.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ops.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://dch.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wvq.shuidangran.top

================================================================================
来源：http://fzc.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sla.wangdashe.top

================================================================================
来源：http://vte.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://orp.yuanzhike.top

println("Hello")
来源：http://mxq.quarkkingdee.top

[T02] Kotlin：变量
来源：http://jwc.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ana.sweek.top

[T03] Kotlin：字符串模板
来源：http://imq.pengpengdd.cyou

"值: $b"
来源：http://zcm.0kj1m.cn

[T04] Kotlin：空安全
来源：http://dmy.hcnkem.com

val n: String? = null;  n?.length
来源：http://upz.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://rzr.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ybk.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://rhj.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vzx.tanke756.top

[T07] Kotlin：集合过滤
来源：http://hzj.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yhc.yvedp.cn

[T08] Kotlin：数据类
来源：http://kjs.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://kin.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://xzf.yj202588.top

fun String.exclaim() = this + "!"
来源：http://fyw.wangdashe.top

[T10] Kotlin：默认参数
来源：http://frj.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://nwk.birdmap.top

[T11] Kotlin：协程
来源：http://kno.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://woe.hnqzz.top

[T12] Kotlin：解构声明
来源：http://rqn.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://pxn.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://mqw.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://fnp.guowangkeji.top

[T14] Kotlin：循环
来源：http://rzj.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://xyi.jlsjyb.cn

[T15] Kotlin：接口
来源：http://cnq.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://aap.jlsjyb.cn

[T16] Swift：Hello World
来源：http://lew.snrcjt.cn

print("Hello")
来源：http://dfw.ehwqpu.com

[T17] Swift：变量与常量
来源：http://zay.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://eov.jiagoushi.top

[T18] Swift：字符串插值
来源：http://wjc.cashguo.top

"值: \(b)"
来源：http://rdb.svipenyu.cn

[T19] Swift：可选绑定
来源：http://kji.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://oyo.mhx1999.top

[T20] Swift：数组操作
来源：http://gph.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://lgu.jqgufenzy.top

[T21] Swift：遍历
来源：http://iwh.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://ghm.zhiwuduotai.top

[T22] Swift：字典
来源：http://kly.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mhs.ybcxt.top

[T23] Swift：函数
来源：http://avu.shuidangran.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ege.52xcode.cn

[T24] Swift：闭包
来源：http://bir.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fih.yj202588.top

[T25] Swift：结构体
来源：http://xub.ehwqpu.com

struct P { var x: Int }
来源：http://eqz.yonumen.top

[T26] Swift：类与重写
来源：http://hup.birdmap.top

class A: Base { override func f() {} }
来源：http://aqu.sysykeji.top

[T27] Swift：错误处理
来源：http://nop.yanxiufei.cn

do { try f() } catch { print(error) }
来源：http://emf.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://lgt.yongpay.top

enum Color { case red, green }
来源：http://iwm.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://xea.hongshengwenyu.top

guard let x = opt else { return }
来源：http://bxd.yanxiufei.cn

[T30] Swift：协议
来源：http://qdt.cashguo.top

protocol Shape { func area() -> Double }
来源：http://ycj.meibo888.top

[T31] Lua：Hello World
来源：http://upu.shanyushiyangtech.top

print("Hello")
来源：http://sld.yongpay.top

[T32] Lua：局部变量
来源：http://fvq.guannengcc.top

local a = 1
来源：http://xly.yj20258.top

[T33] Lua：表（数组）
来源：http://lzs.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://ldv.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://syi.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xrj.xuanzx.com

[T35] Lua：字典表
来源：http://sel.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://kwk.cqqwz.cn

[T36] Lua：函数
来源：http://qzk.dianchejie.cn

function add(a, b) return a + b end
来源：http://fus.daxiang520.top

[T37] Lua：字符串拼接
来源：http://tmb.yanxiufei.cn

"a" .. "b"
来源：http://qyp.jyoumei.cn

[T38] Lua：条件
来源：http://dbv.jqgufenzy.top

if x > 0 then print("正") end
来源：http://tnk.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://avo.jinqigufen.top

string.find(s, "%d+")
来源：http://bmm.shzxlz.cn

[T40] Lua：元表
来源：http://tmy.bjfxy.top

setmetatable({}, { __index = base })
来源：http://vgc.guowangkeji.top

[T41] Perl：Hello World
来源：http://jqf.zhixingplan.top

print "Hello\n";
来源：http://hjz.smart0.xyz

[T42] Perl：变量类型
来源：http://gbf.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://phb.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://fxx.zhixingplan.top

"值: $a"
来源：http://qpk.shangyingyoupin.top

[T44] Perl：条件
来源：http://jdk.316326.xyz

if ($a > 0) { print "正"; }
来源：http://uwo.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://tkg.jinqigfzy.top

for my $x (@arr) { print $x; }
来源：http://ilq.snrcjt.cn

[T46] Perl：哈希操作
来源：http://qwz.52xcode.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gnj.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://pmt.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://jzx.yj20258888.top

[T48] Perl：正则替换
来源：http://cae.yonumen.top

$s =~ s/old/new/g;
来源：http://ppd.zycfv.cn

[T49] Perl：函数
来源：http://hmo.tarul.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wzu.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://neo.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://odn.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://ojn.smart0.xyz

[T51] Scala：Hello World
来源：http://xhr.nwbrower.top

println("Hello")
来源：http://wmu.zhixingplan.top

[T52] Scala：变量
来源：http://pce.ehwqpu.com

val a = 1;  var b = 2
来源：http://fwy.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://ujm.zdqjudy.top

s"值: $b"
来源：http://ump.zhijiandao.cn

[T54] Scala：集合映射
来源：http://sww.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://xtc.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://plj.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nhf.fzhhl.top

[T56] Scala：样例类
来源：http://ikz.andypj.xyz

case class User(name: String, age: Int)
来源：http://btg.pycfn.com

[T57] Scala：模式匹配
来源：http://ymr.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://qtd.guannengcc.top

[T58] Scala：函数定义
来源：http://bna.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://afl.dashuyun.cn

[T59] Scala：循环
来源：http://isp.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://xgu.zhoulong.xyz

[T60] Scala：折叠
来源：http://too.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://prd.yj202588.top

================================================================================
来源：http://qon.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://och.guowangkeji.top

================================================================================
来源：http://liz.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://ols.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://dee.sjlbkw.cn

[U02] Py：导出 / 安装依赖
来源：http://jgi.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yca.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://cfl.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wyg.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://rlx.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qyo.hesvh.cn

[U05] Py：列表去重且保序
来源：http://nxf.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://rjn.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://smh.smart0.xyz

{**a, **b}
来源：http://vlf.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://nga.tanke756.top

{v: k for k, v in d.items()}
来源：http://ugw.jinqigufen.top

[U08] Py：展平二维列表
来源：http://zhs.chenzaomai.com

[y for x in nested for y in x]
来源：http://gef.havefunace.top

[U09] Py：字典取最大值的键
来源：http://die.ydjk.org.cn

max(d, key=d.get)
来源：http://fpv.havefunace.top

[U10] Py：按值排序字典
来源：http://rnn.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ads.aizwys.cn

[U11] Py：生成器表达式
来源：http://srb.zdbjq.cn

(x * 2 for x in arr)
来源：http://inz.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://wax.nwbrower.top

Counter(arr).most_common(3)
来源：http://gai.xylfe.cn

[U13] Py：固定长度队列
来源：http://qjc.svipenyu.cn

deque(maxlen=10)
来源：http://zrk.yueranfly.top

[U14] Py：分组收集到列表
来源：http://eqf.sufxvd.cn

defaultdict(list)
来源：http://npy.vehdjk.com

[U15] Py：高精度计时
来源：http://hte.ppjwa.cn

t = time.perf_counter()
来源：http://wsp.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://elg.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zfk.aizwys.cn

[U17] Py：初始化日志
来源：http://egf.ehwqpu.com

logging.basicConfig(level=logging.INFO)
来源：http://jlk.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://rrr.cheryme.top

pat = re.compile(r"\d+")
来源：http://kgc.cucudq.cn

[U19] Py：正则替换带回调
来源：http://wti.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gvo.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://tkk.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://cnp.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://vhh.redwolf501.top

@contextlib.contextmanager
来源：http://otb.cqqwz.cn

[U22] Py：矩阵转置
来源：http://joo.xinyue.icu

list(zip(*m))
来源：http://wrl.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://iag.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://day.sysykeji.top

[U24] Py：路径操作
来源：http://aoh.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xra.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://vcg.feifeiyinyue.top

csv.DictReader(f)
来源：http://lfw.chenjidiqi.icu

[U26] Py：并发下载
来源：http://efe.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tax.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://dfd.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://diq.fehbvm.com

[U28] Py：类型别名
来源：http://riu.shuidangran.top

UserId = int
来源：http://sqq.316326.xyz

[U29] Py：属性校验
来源：http://quk.gogol.net.cn

@property 与 @x.setter 配合
来源：http://gkq.shzxlz.cn

[U30] Py：数据类
来源：http://atz.vehdjk.com

@dataclass(slots=True)
来源：http://ugj.zdbjq.cn


<!-- 参考信息 -->