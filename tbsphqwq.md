代发 wailian999

int x; scanf("%d", &x);
来源：http://yuf.yj20258.top

[S04] C：字符串复制
来源：http://thf.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://fcv.gzhubu.top

[S05] C：字符串长度
来源：http://pxb.xingfuxueyuan.xyz

strlen(s)
来源：http://tcc.jyoumei.cn

[S06] C：字符串比较
来源：http://lfn.quarkkingdee.top

strcmp(a, b) == 0
来源：http://hcp.chenlongwang.top

[S07] C：数组遍历求和
来源：http://fty.fengsongda.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vrl.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://sxk.fehbvm.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fso.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://ggl.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oer.epnwcf.com

[S10] C：指针与解引用
来源：http://tvf.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://uht.yvedp.cn

[S11] C：逐行读文件
来源：http://txm.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://xgs.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xpl.yj20258888.top

fclose(f);
来源：http://nms.vehdjk.com

[S12] C：写文件
来源：http://wtj.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rrn.jinqigufen.top

[S13] C：宏定义
来源：http://dkx.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lup.cucudq.cn

[S14] C：枚举
来源：http://jbu.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://shc.ydzc1.top

[S15] C：类型转换
来源：http://hsz.ywan-chungtsiang.top

(double) a / b
来源：http://zrn.pengpengdd.cyou

[S16] C：位操作置位
来源：http://ixh.uphjek.com

x |= (1 << 3);
来源：http://xsf.xuetiantiany.cn

[S17] C：安全拼接字符串
来源：http://bol.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yqw.yongpay.top

[S18] C：命令行参数
来源：http://plk.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://hbp.zhongyouzk.top

[S19] C：快速排序
来源：http://ask.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://jtn.hnxiangtu.top

[S20] C：二分查找
来源：http://rhd.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qvu.yueranfly.top

[S21] C：字符类别判断
来源：http://chr.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hsj.jinqigufen.top

[S22] C：字符串转数字
来源：http://yvv.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://mxr.zdbjq.cn

[S23] C：随机数
来源：http://xkb.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lsy.cucudq.cn

[S24] C：获取本地时间
来源：http://nop.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hbs.xuanzx.com

[S25] C：内存拷贝
来源：http://enb.yfazqb.com

memcpy(dst, src, n);
来源：http://haj.cqqwz.cn

[S26] C：内存清零
来源：http://aum.tanke756.top

memset(a, 0, sizeof a);
来源：http://vks.yonumen.top

[S27] C：定义常量
来源：http://dfm.jqgfzy.top

const double PI = 3.14159;
来源：http://acc.jlsjyb.cn

[S28] C：静态变量
来源：http://cxd.bjfxy.top

static int counter = 0;
来源：http://xvr.fanxiaobao.xyz

[S29] C：变参函数
来源：http://uzu.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bvh.jianghu66.top

[S30] C：头文件保护
来源：http://jfi.chenzaomai.com

#ifndef X_H
来源：http://kde.tianlin.xyz

#define X_H
来源：http://nhw.redwolf501.top

#endif
来源：http://vpt.tian-w.cn

[S31] C++：Hello World
来源：http://tzd.yj20258888.top

#include <iostream>
来源：http://wka.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://gff.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://mdl.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://vmd.yangfankeji.com

[S33] C++：vector 增删
来源：http://dwt.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://agd.meibo888.top

[S34] C++：遍历 vector
来源：http://qpu.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://akr.jinqigufen.top

[S35] C++：map
来源：http://ohe.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://psj.jqgufenzy.top

[S36] C++：unordered_map
来源：http://wxk.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wvj.nanxinkj.top

[S37] C++：set
来源：http://lyb.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tsp.xinyue.icu

[S38] C++：排序
来源：http://jrq.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://udu.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://uam.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iac.iojbl.cn

[S40] C++：查找元素
来源：http://stf.yuxming.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rdj.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://zhs.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xpr.hnqzz.top

[S42] C++：继承与虚函数
来源：http://cwd.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://pvm.shuidangran.top

[S43] C++：智能指针
来源：http://qwt.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://auy.hnxiangtu.top

[S44] C++：引用传参
来源：http://rut.sysykeji.top

void inc(int &x) { ++x; }
来源：http://ylj.guannengcc.top

[S45] C++：lambda
来源：http://lpt.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://trc.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://ocw.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bzs.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://wck.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tgg.guannengcc.top

[S48] C++：逐行读文件
来源：http://yzh.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://lon.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://awv.0kj1m.cn

[S49] C++：写文件
来源：http://ivp.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kla.cashguo.top

[S50] C++：格式化数字
来源：http://fgs.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qir.yj20258888.top

[S51] C++：显式类型转换
来源：http://jvi.vehdjk.com

static_cast<double>(a) / b
来源：http://jit.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://svf.cheryme.top

int size() const noexcept { return n_; }
来源：http://vhd.bjfxy.top

[S53] C++：移动语义
来源：http://fgn.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://qjr.daxiang520.top

[S54] C++：异常处理
来源：http://urn.jiagoushi.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zzo.dashuyun.cn

[S55] C++：结构化绑定
来源：http://lld.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iyd.guannengcc.top

[S56] C++：optional
来源：http://akk.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jva.cucudq.cn

[S57] C++：编译期常量
来源：http://kob.sjlbkw.cn

constexpr int N = 10;
来源：http://dys.hesvh.cn

[S58] C++：命名空间
来源：http://vcc.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://cyy.fktsv.cn

[S59] C++：静态断言
来源：http://ysc.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lgk.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://wov.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lvy.chenlongwang.top

================================================================================
来源：http://ayr.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nfn.shangyingyoupin.top

================================================================================
来源：http://aco.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://jsk.guannengcc.top

println("Hello")
来源：http://nfe.zhengqikj.top

[T02] Kotlin：变量
来源：http://bcz.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hge.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://pyh.zhijiandao.cn

"值: $b"
来源：http://khm.shuidangran.top

[T04] Kotlin：空安全
来源：http://djl.ehwqpu.com

val n: String? = null;  n?.length
来源：http://dfk.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://phf.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://noh.fktsv.cn

[T06] Kotlin：集合映射
来源：http://bhy.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hsf.tarul.cn

[T07] Kotlin：集合过滤
来源：http://ran.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://cnf.0kj1m.cn

[T08] Kotlin：数据类
来源：http://vtg.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://uyu.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://pkv.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://eyv.316326.xyz

[T10] Kotlin：默认参数
来源：http://ilu.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tkp.tianlin.xyz

[T11] Kotlin：协程
来源：http://ocd.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fjz.pycfn.com

[T12] Kotlin：解构声明
来源：http://tqy.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://yjs.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://hys.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://rdt.gzhubu.top

[T14] Kotlin：循环
来源：http://djk.snrcjt.cn

for (i in 1..10) println(i)
来源：http://wep.cdnleiting.top

[T15] Kotlin：接口
来源：http://hcx.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://wgy.shzxlz.cn

[T16] Swift：Hello World
来源：http://xxl.yj20258.top

print("Hello")
来源：http://ueh.sxryk.cn

[T17] Swift：变量与常量
来源：http://kdz.cqqwz.cn

var a = 1;  let b = 2
来源：http://sdk.sweek.top

[T18] Swift：字符串插值
来源：http://ilc.fzhhl.top

"值: \(b)"
来源：http://fma.chenjidiqi.icu

[T19] Swift：可选绑定
来源：http://wul.9152youxi.cn

if let n = opt { print(n) }
来源：http://xez.gzhubu.top

[T20] Swift：数组操作
来源：http://two.xinyue.icu

var a = [1, 2, 3];  a.append(4)
来源：http://dyc.sysykeji.top

[T21] Swift：遍历
来源：http://fvr.zhongyouzk.top

for x in a { print(x) }
来源：http://xcm.ydjk.org.cn

[T22] Swift：字典
来源：http://jdf.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://utu.jiagoushi.top

[T23] Swift：函数
来源：http://qcu.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bqi.zdqjudy.top

[T24] Swift：闭包
来源：http://xhw.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qpz.zdqjudy.top

[T25] Swift：结构体
来源：http://bch.haohaochexian.top

struct P { var x: Int }
来源：http://mea.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://urs.cheryme.top

class A: Base { override func f() {} }
来源：http://kwp.nwbrower.top

[T27] Swift：错误处理
来源：http://ufy.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://znz.tianlin.xyz

[T28] Swift：枚举
来源：http://vox.tarul.cn

enum Color { case red, green }
来源：http://cqq.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://vsn.gaohongyu789.top

guard let x = opt else { return }
来源：http://bvb.zhoulong.xyz

[T30] Swift：协议
来源：http://rxx.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://ycr.jinqigfzy.top

[T31] Lua：Hello World
来源：http://ldk.shanyushiyangtech.top

print("Hello")
来源：http://qcm.shuidangran.top

[T32] Lua：局部变量
来源：http://szg.quarkkingdee.top

local a = 1
来源：http://ize.bbcook.cn

[T33] Lua：表（数组）
来源：http://gfy.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xfo.tarul.cn

[T34] Lua：遍历表
来源：http://rvy.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rof.jyoumei.cn

[T35] Lua：字典表
来源：http://old.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://ter.zhixingplan.top

[T36] Lua：函数
来源：http://jvq.sysykeji.top

function add(a, b) return a + b end
来源：http://jvq.yonumen.top

[T37] Lua：字符串拼接
来源：http://bwb.gogol.net.cn

"a" .. "b"
来源：http://ltn.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://vmk.shzxlz.cn

if x > 0 then print("正") end
来源：http://uop.bbcook.cn

[T39] Lua：模式匹配
来源：http://lez.xuanzx.com

string.find(s, "%d+")
来源：http://hbx.aibaodan.cn

[T40] Lua：元表
来源：http://rex.sxryk.cn

setmetatable({}, { __index = base })
来源：http://qrz.hywenlv.cn

[T41] Perl：Hello World
来源：http://ftb.jinqigfzy.top

print "Hello\n";
来源：http://fco.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://umb.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nub.vqdsnc.cn

[T43] Perl：字符串插值
来源：http://cue.shzxlz.cn

"值: $a"
来源：http://vpt.jinghuilouyu.cn

[T44] Perl：条件
来源：http://eog.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://fsy.9152youxi.cn

[T45] Perl：数组遍历
来源：http://grt.hfpthk.cn

for my $x (@arr) { print $x; }
来源：http://wog.nanxinkj.top

[T46] Perl：哈希操作
来源：http://gho.shanyushiyangtech.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dsl.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://pph.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ktm.hcnkem.com

[T48] Perl：正则替换
来源：http://osd.cucudq.cn

$s =~ s/old/new/g;
来源：http://ynu.zhiwuduotai.top

[T49] Perl：函数
来源：http://wyt.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jlj.guannengcc.top

[T50] Perl：逐行读文件
来源：http://ego.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://equ.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://hoy.zhongyouzk.top

[T51] Scala：Hello World
来源：http://rpc.daria6918.cn

println("Hello")
来源：http://pbo.guannengcc.top

[T52] Scala：变量
来源：http://pnl.fktsv.cn

val a = 1;  var b = 2
来源：http://osh.yueranfly.top

[T53] Scala：字符串插值
来源：http://ziq.xingfuxueyuan.xyz

s"值: $b"
来源：http://uhz.sweek.top

[T54] Scala：集合映射
来源：http://ttp.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://tav.epnwcf.com

[T55] Scala：集合过滤
来源：http://ash.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://akq.yuxming.cn

[T56] Scala：样例类
来源：http://dcv.jqgfzy.top

case class User(name: String, age: Int)
来源：http://fcb.yuxming.cn

[T57] Scala：模式匹配
来源：http://bxu.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bqz.hcnkem.com

[T58] Scala：函数定义
来源：http://yfk.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://pvd.cheryme.top

[T59] Scala：循环
来源：http://yvs.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://kaj.mhx1999.top

[T60] Scala：折叠
来源：http://gat.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aqs.dashuyun.cn

================================================================================
来源：http://mnb.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hez.ydzc1.top

================================================================================
来源：http://rog.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://hcp.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://ylh.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://ykx.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pwp.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://brt.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://hgq.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://ywp.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://akc.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://qvr.sysykeji.top

list(dict.fromkeys(arr))
来源：http://hoo.pycfn.com

[U06] Py：合并两个字典
来源：http://fhg.yueranfly.top

{**a, **b}
来源：http://ubo.pycfn.com

[U07] Py：反转字典键值
来源：http://ttx.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://tem.jqgfzy.top

[U08] Py：展平二维列表
来源：http://qbg.dianchejie.cn

[y for x in nested for y in x]
来源：http://yyk.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://qum.vehdjk.com

max(d, key=d.get)
来源：http://xxa.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://bol.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gcq.nwbrower.top

[U11] Py：生成器表达式
来源：http://rma.sxryk.cn

(x * 2 for x in arr)
来源：http://avt.hnqzz.top

[U12] Py：取出现最多的 3 个元素
来源：http://xfq.yangfankeji.com

Counter(arr).most_common(3)
来源：http://duy.jqgfzy.top

[U13] Py：固定长度队列
来源：http://zce.aibaodan.cn

deque(maxlen=10)
来源：http://qds.yj20258888.top

[U14] Py：分组收集到列表
来源：http://ifk.yuanzhike.top

defaultdict(list)
来源：http://oxp.birdmap.top

[U15] Py：高精度计时
来源：http://tvq.dashuyun.cn

t = time.perf_counter()
来源：http://dly.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://xyx.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pzc.jiagoushi.top

[U17] Py：初始化日志
来源：http://oqu.zhixingplan.top

logging.basicConfig(level=logging.INFO)
来源：http://qor.hfpthk.cn

[U18] Py：预编译正则
来源：http://pbl.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://mjk.nwbrower.top

[U19] Py：正则替换带回调
来源：http://rjk.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cal.hysaishi.cn

[U20] Py：缓存函数结果
来源：http://qeo.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://fdb.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://jbx.ehwqpu.com

@contextlib.contextmanager
来源：http://vvp.316326.xyz

[U22] Py：矩阵转置
来源：http://dou.chenzaomai.com

list(zip(*m))
来源：http://yut.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://wel.havefunace.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kad.quarkkingdee.top

[U24] Py：路径操作
来源：http://qhe.feifeiyinyue.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vxv.meibo888.top

[U25] Py：CSV 按字典读
来源：http://hmp.guowangkeji.top

csv.DictReader(f)
来源：http://fxx.cqqwz.cn

[U26] Py：并发下载
来源：http://pju.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nrs.cdnleiting.top


<!-- 参考信息 -->