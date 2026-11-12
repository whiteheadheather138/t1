代发 wailian999

strlen(s)
来源：http://epo.tanke756.top

[S06] C：字符串比较
来源：http://zrx.svipenyu.cn

strcmp(a, b) == 0
来源：http://ssb.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://obx.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ivi.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://rsi.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dvi.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://faa.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tdc.hcnkem.com

[S10] C：指针与解引用
来源：http://njz.mhx1999.top

int *p = &a;  *p = 5;
来源：http://rsu.iojbl.cn

[S11] C：逐行读文件
来源：http://xub.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://ahq.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rwl.andypj.xyz

fclose(f);
来源：http://xbw.tianlin.xyz

[S12] C：写文件
来源：http://hct.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hdn.snrcjt.cn

[S13] C：宏定义
来源：http://cfq.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kjj.zhongyouzk.top

[S14] C：枚举
来源：http://osc.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://dcd.vqdsnc.cn

[S15] C：类型转换
来源：http://exz.chenzaomai.com

(double) a / b
来源：http://oyq.jiagoushi.top

[S16] C：位操作置位
来源：http://eox.jiagoushi.top

x |= (1 << 3);
来源：http://bso.sxryk.cn

[S17] C：安全拼接字符串
来源：http://quv.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sbj.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://xwz.andypj.xyz

int main(int argc, char **argv)
来源：http://fdh.gaohongyu789.top

[S19] C：快速排序
来源：http://alq.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yel.shuidangran.top

[S20] C：二分查找
来源：http://lue.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eom.epnwcf.com

[S21] C：字符类别判断
来源：http://xqk.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dhu.hnxiangtu.top

[S22] C：字符串转数字
来源：http://vvg.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://ank.yfazqb.com

[S23] C：随机数
来源：http://ihl.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jvq.zdbjq.cn

[S24] C：获取本地时间
来源：http://sjs.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mes.cheryme.top

[S25] C：内存拷贝
来源：http://daz.jiagoushi.top

memcpy(dst, src, n);
来源：http://vyw.hfpthk.cn

[S26] C：内存清零
来源：http://ohx.c1oappe.top

memset(a, 0, sizeof a);
来源：http://xyk.xylfe.cn

[S27] C：定义常量
来源：http://nlt.sufxvd.cn

const double PI = 3.14159;
来源：http://hrj.0kj1m.cn

[S28] C：静态变量
来源：http://aqa.yj20258888.top

static int counter = 0;
来源：http://cyh.hammf.cn

[S29] C：变参函数
来源：http://uow.hongshengwenyu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://htj.yuanzhike.top

[S30] C：头文件保护
来源：http://gzv.snrcjt.cn

#ifndef X_H
来源：http://rbw.nwbrower.top

#define X_H
来源：http://fqi.smart0.xyz

#endif
来源：http://qvi.jiagoushi.top

[S31] C++：Hello World
来源：http://ftk.xingfuxueyuan.xyz

#include <iostream>
来源：http://gkb.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://xwd.jqgufenzy.top

[S32] C++：字符串
来源：http://gyq.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://xps.svipenyu.cn

[S33] C++：vector 增删
来源：http://avi.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xag.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://wop.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://xir.gaohongyu789.top

[S35] C++：map
来源：http://kif.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qrc.c1oappe.top

[S36] C++：unordered_map
来源：http://hqu.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cdw.chenlongwang.top

[S37] C++：set
来源：http://ajq.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zsf.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://lyl.hfpthk.cn

std::sort(v.begin(), v.end());
来源：http://ltr.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://etc.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cpa.jyoumei.cn

[S40] C++：查找元素
来源：http://rre.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zgs.guannengcc.top

[S41] C++：类与构造函数
来源：http://tvw.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://euc.uphjek.com

[S42] C++：继承与虚函数
来源：http://knp.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://kiw.sxryk.cn

[S43] C++：智能指针
来源：http://csk.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://szk.zhijiandao.cn

[S44] C++：引用传参
来源：http://lwd.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://fyg.aizwys.cn

[S45] C++：lambda
来源：http://qks.zycfv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zbp.zycfv.cn

[S46] C++：函数模板
来源：http://zfe.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wax.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://ljf.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mxg.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://fay.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://mla.sysykeji.top

while (std::getline(in, line)) { }
来源：http://tkm.quarkkingdee.top

[S49] C++：写文件
来源：http://bzn.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://myq.daxiang520.top

[S50] C++：格式化数字
来源：http://lif.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oxk.0kj1m.cn

[S51] C++：显式类型转换
来源：http://qaj.dianchejie.cn

static_cast<double>(a) / b
来源：http://yde.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://oaz.birdmap.top

int size() const noexcept { return n_; }
来源：http://gms.yuxming.cn

[S53] C++：移动语义
来源：http://yqw.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://xto.yanxiufei.cn

[S54] C++：异常处理
来源：http://qyd.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zfw.yuanzhike.top

[S55] C++：结构化绑定
来源：http://mjr.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aad.jyoumei.cn

[S56] C++：optional
来源：http://lrv.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hdk.zhoulong.xyz

[S57] C++：编译期常量
来源：http://wou.jlsjyb.cn

constexpr int N = 10;
来源：http://lmh.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://his.daria6918.cn

namespace ns { int f() { return 1; } }
来源：http://dsf.jinqigufen.top

[S59] C++：静态断言
来源：http://hhv.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tbv.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://chb.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://edm.dashuyun.cn

================================================================================
来源：http://yos.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rzc.zhiwuduotai.top

================================================================================
来源：http://mlj.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://uck.redwolf501.top

println("Hello")
来源：http://laq.andypj.xyz

[T02] Kotlin：变量
来源：http://lgk.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hav.zhiwuduotai.top

[T03] Kotlin：字符串模板
来源：http://lis.havefunace.top

"值: $b"
来源：http://iwi.yj202588.top

[T04] Kotlin：空安全
来源：http://ljw.zhixingplan.top

val n: String? = null;  n?.length
来源：http://bxo.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://gwy.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fwq.yuxming.cn

[T06] Kotlin：集合映射
来源：http://ejx.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://inq.hywenlv.cn

[T07] Kotlin：集合过滤
来源：http://dpd.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aai.zhixingplan.top

[T08] Kotlin：数据类
来源：http://rgj.ivvv.top

data class User(val name: String, val age: Int)
来源：http://lsg.ivvv.top

[T09] Kotlin：扩展函数
来源：http://vjd.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://zzs.tian-w.cn

[T10] Kotlin：默认参数
来源：http://lmd.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ift.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://ltb.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fwr.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://oes.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://bla.yj202588.top

[T13] Kotlin：只读 Map
来源：http://kvs.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://nwg.hnqzz.top

[T14] Kotlin：循环
来源：http://tad.sweek.top

for (i in 1..10) println(i)
来源：http://rvq.snrcjt.cn

[T15] Kotlin：接口
来源：http://mrp.smart0.xyz

interface Shape { fun area(): Double }
来源：http://kkw.redwolf501.top

[T16] Swift：Hello World
来源：http://pqk.xingfuxueyuan.xyz

print("Hello")
来源：http://uyv.aibaodan.cn

[T17] Swift：变量与常量
来源：http://oyw.jqgufenzy.top

var a = 1;  let b = 2
来源：http://cnh.andypj.xyz

[T18] Swift：字符串插值
来源：http://vvf.pycfn.com

"值: \(b)"
来源：http://xpy.sweek.top

[T19] Swift：可选绑定
来源：http://awa.andypj.xyz

if let n = opt { print(n) }
来源：http://awg.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://ptj.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://hjj.316326.xyz

[T21] Swift：遍历
来源：http://gqz.daxiang520.top

for x in a { print(x) }
来源：http://zqb.gaohongyu789.top

[T22] Swift：字典
来源：http://veb.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://xdj.snrcjt.cn

[T23] Swift：函数
来源：http://iye.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://psz.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://wnz.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aer.ehwqpu.com

[T25] Swift：结构体
来源：http://nyw.jlsjyb.cn

struct P { var x: Int }
来源：http://ual.xylfe.cn

[T26] Swift：类与重写
来源：http://cct.fzhhl.top

class A: Base { override func f() {} }
来源：http://mgy.52xcode.cn

[T27] Swift：错误处理
来源：http://frh.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://vwg.zhijiandao.cn

[T28] Swift：枚举
来源：http://rzo.zdbjq.cn

enum Color { case red, green }
来源：http://enw.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://iyq.hnqzz.top

guard let x = opt else { return }
来源：http://hnc.cashguo.top

[T30] Swift：协议
来源：http://fuz.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://zcy.hysaishi.cn

[T31] Lua：Hello World
来源：http://zzj.yonumen.top

print("Hello")
来源：http://fpk.shzxlz.cn

[T32] Lua：局部变量
来源：http://vnn.xuetiantiany.cn

local a = 1
来源：http://pjp.jinqigufen.top

[T33] Lua：表（数组）
来源：http://zzh.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hmm.ivvv.top

[T34] Lua：遍历表
来源：http://uam.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://jbq.dianchejie.cn

[T35] Lua：字典表
来源：http://ltw.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://qkb.zhixingplan.top

[T36] Lua：函数
来源：http://iee.9152youxi.cn

function add(a, b) return a + b end
来源：http://zje.tarul.cn

[T37] Lua：字符串拼接
来源：http://ylf.hysaishi.cn

"a" .. "b"
来源：http://gat.yuanzhike.top

[T38] Lua：条件
来源：http://lkj.yueranfly.top

if x > 0 then print("正") end
来源：http://fnu.xziqi.cn

[T39] Lua：模式匹配
来源：http://pzj.gzhubu.top

string.find(s, "%d+")
来源：http://sgw.tian-w.cn

[T40] Lua：元表
来源：http://ubs.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://jbr.hfpthk.cn

[T41] Perl：Hello World
来源：http://ozw.epnwcf.com

print "Hello\n";
来源：http://fqf.yvedp.cn

[T42] Perl：变量类型
来源：http://qux.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tuv.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://mwa.yangfankeji.com

"值: $a"
来源：http://ocw.ydzc1.top

[T44] Perl：条件
来源：http://xuz.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://uzk.fengsongda.top

[T45] Perl：数组遍历
来源：http://hjt.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://jgj.zhengqikj.top

[T46] Perl：哈希操作
来源：http://fth.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bra.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://eaw.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eqb.fzhhl.top

[T48] Perl：正则替换
来源：http://eog.guowangkeji.top

$s =~ s/old/new/g;
来源：http://hdi.gotoacloud.top

[T49] Perl：函数
来源：http://nxb.xinyue.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iqf.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://hfl.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://msm.nanxinkj.top

while (my $line = <$fh>) { print $line; }
来源：http://qvu.chenzaomai.com

[T51] Scala：Hello World
来源：http://gxq.vqdsnc.cn

println("Hello")
来源：http://vwz.fehbvm.com

[T52] Scala：变量
来源：http://lfe.hesvh.cn

val a = 1;  var b = 2
来源：http://xne.fzhhl.top

[T53] Scala：字符串插值
来源：http://exn.tanke756.top

s"值: $b"
来源：http://ylk.sysykeji.top

[T54] Scala：集合映射
来源：http://stx.nanxinkj.top

List(1, 2, 3).map(_ * 2)
来源：http://jht.cheryme.top

[T55] Scala：集合过滤
来源：http://iry.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://agv.ehwqpu.com

[T56] Scala：样例类
来源：http://ocx.ctjpmb.com

case class User(name: String, age: Int)
来源：http://sdz.yj20258888.top

[T57] Scala：模式匹配
来源：http://vzm.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jsq.epnwcf.com

[T58] Scala：函数定义
来源：http://kvg.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tbh.jianghu66.top

[T59] Scala：循环
来源：http://oqc.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://gez.yonumen.top

[T60] Scala：折叠
来源：http://ryz.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tjc.chenjidiqi.icu

================================================================================
来源：http://rxm.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ttm.smart0.xyz

================================================================================
来源：http://kpu.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://yiw.shangyingyoupin.top

python -m venv .venv && source .venv/bin/activate
来源：http://eox.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://vqx.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://auk.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://vbv.yuanzhike.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mhm.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://qmw.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bng.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://aei.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://dkc.chenzaomai.com

[U06] Py：合并两个字典
来源：http://clq.ydzc1.top

{**a, **b}
来源：http://cvq.jlsjyb.cn

[U07] Py：反转字典键值
来源：http://rcv.epnwcf.com

{v: k for k, v in d.items()}
来源：http://udy.smart0.xyz

[U08] Py：展平二维列表
来源：http://wpo.birdmap.top

[y for x in nested for y in x]
来源：http://gvr.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://pci.ydzc1.top

max(d, key=d.get)
来源：http://jvn.jqgfzy.top

[U10] Py：按值排序字典
来源：http://rzl.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sli.fzhhl.top

[U11] Py：生成器表达式
来源：http://xej.chenzaomai.com

(x * 2 for x in arr)
来源：http://jge.ppjwa.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ksn.yj20258888.top

Counter(arr).most_common(3)
来源：http://xut.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://zpz.wangdashe.top

deque(maxlen=10)
来源：http://qth.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://tlt.chenlongwang.top

defaultdict(list)
来源：http://zvm.mhx1999.top

[U15] Py：高精度计时
来源：http://skr.jinqigufen.top

t = time.perf_counter()
来源：http://kfi.hammf.cn

[U16] Py：命令行参数解析
来源：http://rni.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mve.tanke756.top

[U17] Py：初始化日志
来源：http://nye.smart0.xyz

logging.basicConfig(level=logging.INFO)
来源：http://mvy.xuanzx.com

[U18] Py：预编译正则
来源：http://gba.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://fev.hysaishi.cn

[U19] Py：正则替换带回调
来源：http://kic.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wje.xuanzx.com

[U20] Py：缓存函数结果
来源：http://btt.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://xar.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://owd.zycfv.cn

@contextlib.contextmanager
来源：http://jrm.uphjek.com

[U22] Py：矩阵转置
来源：http://czj.birdmap.top

list(zip(*m))
来源：http://nys.ydzc1.top

[U23] Py：分块读取大文件
来源：http://bsk.havefunace.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://igq.haohaochexian.top

[U24] Py：路径操作
来源：http://tyq.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gbv.jqgfzy.top

[U25] Py：CSV 按字典读
来源：http://zld.tianlin.xyz

csv.DictReader(f)
来源：http://ohh.zhongyouzk.top

[U26] Py：并发下载
来源：http://zff.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://axh.sweek.top

[U27] Py：异步 HTTP
来源：http://igp.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://fnl.smart0.xyz

[U28] Py：类型别名
来源：http://iag.yueranfly.top

UserId = int
来源：http://yam.jinqigfzy.top


<!-- 参考信息 -->