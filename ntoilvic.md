代发 wailian999

int x; scanf("%d", &x);
来源：http://weq.tian-w.cn

[S04] C：字符串复制
来源：http://hkz.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://ghr.pengpengdd.cyou

[S05] C：字符串长度
来源：http://ros.hammf.cn

strlen(s)
来源：http://unt.zhengqikj.top

[S06] C：字符串比较
来源：http://gfb.jyoumei.cn

strcmp(a, b) == 0
来源：http://ubq.ctjpmb.com

[S07] C：数组遍历求和
来源：http://tha.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lyv.tarul.cn

[S08] C：动态内存分配与释放
来源：http://dwd.yvedp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nia.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://jrp.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://apx.cucudq.cn

[S10] C：指针与解引用
来源：http://rxk.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://nyk.ivvv.top

[S11] C：逐行读文件
来源：http://wqu.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://hhw.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ykt.hesvh.cn

fclose(f);
来源：http://lbz.yj202588.top

[S12] C：写文件
来源：http://cqx.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zzy.hnqzz.top

[S13] C：宏定义
来源：http://yhq.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wta.sweek.top

[S14] C：枚举
来源：http://vym.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://vjc.ehwqpu.com

[S15] C：类型转换
来源：http://cxl.guowangkeji.top

(double) a / b
来源：http://koy.shzxlz.cn

[S16] C：位操作置位
来源：http://vsg.smart0.xyz

x |= (1 << 3);
来源：http://yee.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://sbw.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bff.hammf.cn

[S18] C：命令行参数
来源：http://qrp.xylfe.cn

int main(int argc, char **argv)
来源：http://ivl.bjfxy.top

[S19] C：快速排序
来源：http://zdp.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lif.xylfe.cn

[S20] C：二分查找
来源：http://ufz.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nqw.epnwcf.com

[S21] C：字符类别判断
来源：http://fbh.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xpw.jqgfzy.top

[S22] C：字符串转数字
来源：http://xmq.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://frm.shzxlz.cn

[S23] C：随机数
来源：http://cfo.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ptq.dianchejie.cn

[S24] C：获取本地时间
来源：http://yva.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gdf.havefunace.top

[S25] C：内存拷贝
来源：http://fqm.kuanghao11.cn

memcpy(dst, src, n);
来源：http://rco.jinqigfzy.top

[S26] C：内存清零
来源：http://fen.sysykeji.top

memset(a, 0, sizeof a);
来源：http://lml.ivvv.top

[S27] C：定义常量
来源：http://taa.zhongyouzk.top

const double PI = 3.14159;
来源：http://ops.fehbvm.com

[S28] C：静态变量
来源：http://req.shanyushiyangtech.top

static int counter = 0;
来源：http://okf.yonumen.top

[S29] C：变参函数
来源：http://qld.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zns.quarkkingdee.top

[S30] C：头文件保护
来源：http://oto.cqqwz.cn

#ifndef X_H
来源：http://zfk.hywenlv.cn

#define X_H
来源：http://ixr.nwbrower.top

#endif
来源：http://quh.nanxinkj.top

[S31] C++：Hello World
来源：http://ncw.shzxlz.cn

#include <iostream>
来源：http://hpn.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://qsk.tianlin.xyz

[S32] C++：字符串
来源：http://hvj.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://xvo.cashguo.top

[S33] C++：vector 增删
来源：http://xcp.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://teb.guannengcc.top

[S34] C++：遍历 vector
来源：http://luv.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://vvn.xingfuxueyuan.xyz

[S35] C++：map
来源：http://dfd.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zpl.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://ozj.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uwo.feifeiyinyue.top

[S37] C++：set
来源：http://kts.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nen.yfazqb.com

[S38] C++：排序
来源：http://jev.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://qzw.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://ynz.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://inv.jyoumei.cn

[S40] C++：查找元素
来源：http://qum.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vjz.hcnkem.com

[S41] C++：类与构造函数
来源：http://ccg.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eze.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://gaq.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://bml.jyoumei.cn

[S43] C++：智能指针
来源：http://qda.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://wht.gzhubu.top

[S44] C++：引用传参
来源：http://dhz.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://adc.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://wty.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rzp.dashuyun.cn

[S46] C++：函数模板
来源：http://ydb.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dig.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://kgz.52xcode.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mcf.yonumen.top

[S48] C++：逐行读文件
来源：http://yyf.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qbg.52xcode.cn

while (std::getline(in, line)) { }
来源：http://rmd.zhiwuduotai.top

[S49] C++：写文件
来源：http://cxx.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tio.hnxiangtu.top

[S50] C++：格式化数字
来源：http://ggp.tianlin.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hnt.shuidangran.top

[S51] C++：显式类型转换
来源：http://bia.sysykeji.top

static_cast<double>(a) / b
来源：http://mji.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://cpn.birdmap.top

int size() const noexcept { return n_; }
来源：http://cgh.pycfn.com

[S53] C++：移动语义
来源：http://gdo.9152youxi.cn

std::vector<int> w = std::move(v);
来源：http://xnh.svipenyu.cn

[S54] C++：异常处理
来源：http://yva.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://myu.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://agn.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eca.aizwys.cn

[S56] C++：optional
来源：http://ppq.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iqr.dashuyun.cn

[S57] C++：编译期常量
来源：http://cun.guowangkeji.top

constexpr int N = 10;
来源：http://cjq.guannengcc.top

[S58] C++：命名空间
来源：http://jwq.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://eke.guannengcc.top

[S59] C++：静态断言
来源：http://abz.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rgm.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://mvt.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lxp.ppjwa.cn

================================================================================
来源：http://kqw.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zuv.pengpengdd.cyou

================================================================================
来源：http://bhs.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://lpx.fanxiaobao.xyz

println("Hello")
来源：http://mpc.52xcode.cn

[T02] Kotlin：变量
来源：http://ikk.ehwqpu.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://knj.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://zmu.ybcxt.top

"值: $b"
来源：http://jpz.zdqjudy.top

[T04] Kotlin：空安全
来源：http://znm.tanke756.top

val n: String? = null;  n?.length
来源：http://nbi.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://xci.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ygr.tarul.cn

[T06] Kotlin：集合映射
来源：http://qpi.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://lal.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://hiy.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qck.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://tvd.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://loc.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://ppg.vqdsnc.cn

fun String.exclaim() = this + "!"
来源：http://azp.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://etj.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://daf.bbcook.cn

[T11] Kotlin：协程
来源：http://esj.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zmp.hammf.cn

[T12] Kotlin：解构声明
来源：http://dgk.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://kes.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://bss.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://mhd.xinyue.icu

[T14] Kotlin：循环
来源：http://rcj.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://njg.0kj1m.cn

[T15] Kotlin：接口
来源：http://eml.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://ope.sjlbkw.cn

[T16] Swift：Hello World
来源：http://gdf.jqgufenzy.top

print("Hello")
来源：http://xbz.nanxuanxn.top

[T17] Swift：变量与常量
来源：http://ubf.gaohongyu789.top

var a = 1;  let b = 2
来源：http://cng.zdqjudy.top

[T18] Swift：字符串插值
来源：http://ivb.fanxiaobao.xyz

"值: \(b)"
来源：http://qou.guowangkeji.top

[T19] Swift：可选绑定
来源：http://fbo.yj20258.top

if let n = opt { print(n) }
来源：http://quf.vehdjk.com

[T20] Swift：数组操作
来源：http://jip.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://bxx.jinqigfzy.top

[T21] Swift：遍历
来源：http://klo.zycfv.cn

for x in a { print(x) }
来源：http://vpi.guannengcc.top

[T22] Swift：字典
来源：http://qlm.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://adh.chenjidiqi.icu

[T23] Swift：函数
来源：http://cwh.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lef.cqqwz.cn

[T24] Swift：闭包
来源：http://lxe.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yus.gzhubu.top

[T25] Swift：结构体
来源：http://psv.sysykeji.top

struct P { var x: Int }
来源：http://gvx.yuxming.cn

[T26] Swift：类与重写
来源：http://brf.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://hyj.wangdashe.top

[T27] Swift：错误处理
来源：http://fjk.uphjek.com

do { try f() } catch { print(error) }
来源：http://clo.pycfn.com

[T28] Swift：枚举
来源：http://rzb.havefunace.top

enum Color { case red, green }
来源：http://uum.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://qqk.hywenlv.cn

guard let x = opt else { return }
来源：http://qnr.316326.xyz

[T30] Swift：协议
来源：http://eoe.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://rgh.vqdsnc.cn

[T31] Lua：Hello World
来源：http://nkh.yj20258.top

print("Hello")
来源：http://hlw.zycfv.cn

[T32] Lua：局部变量
来源：http://ddq.shuidangran.top

local a = 1
来源：http://guh.dashuyun.cn

[T33] Lua：表（数组）
来源：http://bfx.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qbl.zdqjudy.top

[T34] Lua：遍历表
来源：http://idn.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://cmj.hongshengwenyu.top

[T35] Lua：字典表
来源：http://ioc.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://elx.yuxming.cn

[T36] Lua：函数
来源：http://zdx.zdbjq.cn

function add(a, b) return a + b end
来源：http://wor.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://rku.quarkkingdee.top

"a" .. "b"
来源：http://tiq.dashuyun.cn

[T38] Lua：条件
来源：http://gvj.wangdashe.top

if x > 0 then print("正") end
来源：http://ule.jiagoushi.top

[T39] Lua：模式匹配
来源：http://ihp.yanxiufei.cn

string.find(s, "%d+")
来源：http://wed.xziqi.cn

[T40] Lua：元表
来源：http://rxy.cucudq.cn

setmetatable({}, { __index = base })
来源：http://ofj.52xcode.cn

[T41] Perl：Hello World
来源：http://zkx.aibaodan.cn

print "Hello\n";
来源：http://jje.9152youxi.cn

[T42] Perl：变量类型
来源：http://igu.ivvv.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://czg.chenzaomai.com

[T43] Perl：字符串插值
来源：http://dmy.pengpengdd.cyou

"值: $a"
来源：http://jgl.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://qve.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://auu.cqqwz.cn

[T45] Perl：数组遍历
来源：http://ski.dashuyun.cn

for my $x (@arr) { print $x; }
来源：http://vaq.aizwys.cn

[T46] Perl：哈希操作
来源：http://cyz.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kny.aizwys.cn

[T47] Perl：正则捕获
来源：http://cvq.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ebx.cashguo.top

[T48] Perl：正则替换
来源：http://huk.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://chv.cqqwz.cn

[T49] Perl：函数
来源：http://mpn.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yob.tian-w.cn

[T50] Perl：逐行读文件
来源：http://niz.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ixy.havefunace.top

while (my $line = <$fh>) { print $line; }
来源：http://mkj.daxiang520.top

[T51] Scala：Hello World
来源：http://qxd.wangdashe.top

println("Hello")
来源：http://nzp.tianlin.xyz

[T52] Scala：变量
来源：http://msx.fehbvm.com

val a = 1;  var b = 2
来源：http://kdl.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://mrv.316326.xyz

s"值: $b"
来源：http://sis.nanxinkj.top

[T54] Scala：集合映射
来源：http://nld.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://rhz.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://aij.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rss.cdnleiting.top

[T56] Scala：样例类
来源：http://xlj.zhengqikj.top

case class User(name: String, age: Int)
来源：http://ric.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://fmc.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://exm.nanxinkj.top

[T58] Scala：函数定义
来源：http://ujs.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ays.dianchejie.cn

[T59] Scala：循环
来源：http://yvm.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://msr.gotoacloud.top

[T60] Scala：折叠
来源：http://sci.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ckp.shangyingyoupin.top

================================================================================
来源：http://nnj.zhoulong.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xfq.shzxlz.cn

================================================================================
来源：http://nfi.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://ogu.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://ctd.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://cva.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tex.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://dtf.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://uyf.jianghu66.top

[U04] Py：变量调试打印
来源：http://omp.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mvw.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://dxc.bbcook.cn

list(dict.fromkeys(arr))
来源：http://dae.xuanzx.com

[U06] Py：合并两个字典
来源：http://oai.cqqwz.cn

{**a, **b}
来源：http://zhy.fengsongda.top

[U07] Py：反转字典键值
来源：http://eje.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://sco.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://lft.jianghu66.top

[y for x in nested for y in x]
来源：http://wge.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://asp.chenzaomai.com

max(d, key=d.get)
来源：http://zma.zhengqikj.top

[U10] Py：按值排序字典
来源：http://ymy.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vel.pycfn.com

[U11] Py：生成器表达式
来源：http://fvg.yongpay.top

(x * 2 for x in arr)
来源：http://rka.fengsongda.top

[U12] Py：取出现最多的 3 个元素
来源：http://bor.nanxinkj.top

Counter(arr).most_common(3)
来源：http://jwv.tarul.cn

[U13] Py：固定长度队列
来源：http://blh.cheryme.top

deque(maxlen=10)
来源：http://hin.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://jyq.vehdjk.com

defaultdict(list)
来源：http://fed.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://kgj.dianchejie.cn

t = time.perf_counter()
来源：http://gwn.fengsongda.top

[U16] Py：命令行参数解析
来源：http://zrl.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pgb.yvedp.cn

[U17] Py：初始化日志
来源：http://wrp.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://oeo.fengsongda.top

[U18] Py：预编译正则
来源：http://fsc.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://rbd.ctjpmb.com

[U19] Py：正则替换带回调
来源：http://vwt.xinyue.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://omt.gzhubu.top

[U20] Py：缓存函数结果
来源：http://bmx.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://cvh.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://jew.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://htr.tian-w.cn

[U22] Py：矩阵转置
来源：http://cbs.zdqjudy.top

list(zip(*m))
来源：http://nrp.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://nwz.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mhi.ydzc1.top

[U24] Py：路径操作
来源：http://svz.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://civ.hammf.cn

[U25] Py：CSV 按字典读
来源：http://eom.yangfankeji.com

csv.DictReader(f)
来源：http://nto.zycfv.cn

[U26] Py：并发下载
来源：http://gpw.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hzr.zhongyouzk.top


<!-- 参考信息 -->