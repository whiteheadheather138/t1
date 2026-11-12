代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xjc.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://nox.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hlk.xinyue.icu

[S09] C：结构体定义与初始化
来源：http://ylz.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mej.yj20258.top

[S10] C：指针与解引用
来源：http://wuv.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://jym.cashguo.top

[S11] C：逐行读文件
来源：http://whn.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://xnu.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zse.hysaishi.cn

fclose(f);
来源：http://xlw.daria6918.cn

[S12] C：写文件
来源：http://tdi.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ucv.tian-w.cn

[S13] C：宏定义
来源：http://gip.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bzw.fehbvm.com

[S14] C：枚举
来源：http://wmq.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://dzy.tianlin.xyz

[S15] C：类型转换
来源：http://mnk.yuxming.cn

(double) a / b
来源：http://wpt.tarul.cn

[S16] C：位操作置位
来源：http://ial.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://zot.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://ewx.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cbl.shuidangran.top

[S18] C：命令行参数
来源：http://oip.zhoulong.xyz

int main(int argc, char **argv)
来源：http://jie.fanxiaobao.xyz

[S19] C：快速排序
来源：http://lft.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://duy.yangfankeji.com

[S20] C：二分查找
来源：http://xyb.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://owa.quarkkingdee.top

[S21] C：字符类别判断
来源：http://wim.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hay.zhongyouzk.top

[S22] C：字符串转数字
来源：http://fyr.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://lsk.tianlin.xyz

[S23] C：随机数
来源：http://yoc.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bmd.jqgfzy.top

[S24] C：获取本地时间
来源：http://aar.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gzg.yuanzhike.top

[S25] C：内存拷贝
来源：http://avk.hcnkem.com

memcpy(dst, src, n);
来源：http://yka.gaohongyu789.top

[S26] C：内存清零
来源：http://gag.c1oappe.top

memset(a, 0, sizeof a);
来源：http://ozj.haohaochexian.top

[S27] C：定义常量
来源：http://eju.yueranfly.top

const double PI = 3.14159;
来源：http://sqg.zdqjudy.top

[S28] C：静态变量
来源：http://uel.quarkkingdee.top

static int counter = 0;
来源：http://lqe.sjlbkw.cn

[S29] C：变参函数
来源：http://hja.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://woq.tarul.cn

[S30] C：头文件保护
来源：http://gbt.jqgufenzy.top

#ifndef X_H
来源：http://syl.316326.xyz

#define X_H
来源：http://her.kuanghao11.cn

#endif
来源：http://cpz.feifeiyinyue.top

[S31] C++：Hello World
来源：http://csr.jinghuilouyu.cn

#include <iostream>
来源：http://bej.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://jzd.hywenlv.cn

[S32] C++：字符串
来源：http://bdq.yonumen.top

std::string s = "hi";  s += "!";
来源：http://pfl.9152youxi.cn

[S33] C++：vector 增删
来源：http://rjs.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wyh.havefunace.top

[S34] C++：遍历 vector
来源：http://ujv.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://mul.ydzc1.top

[S35] C++：map
来源：http://xcy.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yvt.smart0.xyz

[S36] C++：unordered_map
来源：http://ibu.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mdp.uphjek.com

[S37] C++：set
来源：http://qfd.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kjj.shuidangran.top

[S38] C++：排序
来源：http://ptq.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://ngp.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://zvf.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cwj.gzhubu.top

[S40] C++：查找元素
来源：http://xnr.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://olo.birdmap.top

[S41] C++：类与构造函数
来源：http://ewa.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gxa.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://rof.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://fgy.xziqi.cn

[S43] C++：智能指针
来源：http://epu.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://lmb.52xcode.cn

[S44] C++：引用传参
来源：http://wkk.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://icp.pengpengdd.cyou

[S45] C++：lambda
来源：http://esc.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://opm.xziqi.cn

[S46] C++：函数模板
来源：http://nvg.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eom.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://lrh.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kfn.zhixingplan.top

[S48] C++：逐行读文件
来源：http://zbp.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://uxi.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://yxc.ydjk.org.cn

[S49] C++：写文件
来源：http://tfj.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ldu.hammf.cn

[S50] C++：格式化数字
来源：http://pjl.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zha.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://zeo.cdnleiting.top

static_cast<double>(a) / b
来源：http://qdt.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://wnp.ivvv.top

int size() const noexcept { return n_; }
来源：http://fxy.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://etk.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://khr.jianghu66.top

[S54] C++：异常处理
来源：http://ikv.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xcr.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://zht.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xdf.yongpay.top

[S56] C++：optional
来源：http://uky.chenlongwang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jzr.vehdjk.com

[S57] C++：编译期常量
来源：http://ijs.shangyingyoupin.top

constexpr int N = 10;
来源：http://iko.ehwqpu.com

[S58] C++：命名空间
来源：http://yfu.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://wgw.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://xke.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://whg.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://guv.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wwf.xinyue.icu

================================================================================
来源：http://ekc.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tow.zdbjq.cn

================================================================================
来源：http://npz.nwbrower.top

[T01] Kotlin：Hello World
来源：http://zek.xuanzx.com

println("Hello")
来源：http://vsk.zhijiandao.cn

[T02] Kotlin：变量
来源：http://ors.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vhk.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://nla.jinqigfzy.top

"值: $b"
来源：http://rfn.ehwqpu.com

[T04] Kotlin：空安全
来源：http://zuf.haohaochexian.top

val n: String? = null;  n?.length
来源：http://urr.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://rqp.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hyr.yfazqb.com

[T06] Kotlin：集合映射
来源：http://iho.redwolf501.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ohb.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://mqs.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zgl.smart0.xyz

[T08] Kotlin：数据类
来源：http://cjv.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://szh.yonumen.top

[T09] Kotlin：扩展函数
来源：http://vuh.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://rdx.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://anu.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nud.ybcxt.top

[T11] Kotlin：协程
来源：http://yff.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zku.redwolf501.top

[T12] Kotlin：解构声明
来源：http://fyk.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://fvq.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://yge.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://ptp.hammf.cn

[T14] Kotlin：循环
来源：http://fqs.nanxinkj.top

for (i in 1..10) println(i)
来源：http://rbt.yongpay.top

[T15] Kotlin：接口
来源：http://wgz.redwolf501.top

interface Shape { fun area(): Double }
来源：http://qct.jqgfzy.top

[T16] Swift：Hello World
来源：http://kce.iojbl.cn

print("Hello")
来源：http://lag.aibaodan.cn

[T17] Swift：变量与常量
来源：http://ghf.xylfe.cn

var a = 1;  let b = 2
来源：http://hnv.vehdjk.com

[T18] Swift：字符串插值
来源：http://pfj.xuanzx.com

"值: \(b)"
来源：http://nyd.c1oappe.top

[T19] Swift：可选绑定
来源：http://nnz.hnxiangtu.top

if let n = opt { print(n) }
来源：http://ruu.dashuyun.cn

[T20] Swift：数组操作
来源：http://lag.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://wal.uphjek.com

[T21] Swift：遍历
来源：http://vrk.wangshuangyany.cn

for x in a { print(x) }
来源：http://hlp.yj20258888.top

[T22] Swift：字典
来源：http://nhb.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://zbn.hfpthk.cn

[T23] Swift：函数
来源：http://tpv.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oov.vqdsnc.cn

[T24] Swift：闭包
来源：http://hji.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aus.yj202588.top

[T25] Swift：结构体
来源：http://lho.yonumen.top

struct P { var x: Int }
来源：http://cdb.ctjpmb.com

[T26] Swift：类与重写
来源：http://zaf.0kj1m.cn

class A: Base { override func f() {} }
来源：http://aqn.quarkkingdee.top

[T27] Swift：错误处理
来源：http://qmh.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://qwy.hysaishi.cn

[T28] Swift：枚举
来源：http://xkm.uphjek.com

enum Color { case red, green }
来源：http://ejy.jianghu66.top

[T29] Swift：guard 提前返回
来源：http://lch.hfpthk.cn

guard let x = opt else { return }
来源：http://rtr.yuanzhike.top

[T30] Swift：协议
来源：http://hkr.gogol.net.cn

protocol Shape { func area() -> Double }
来源：http://vqc.jyoumei.cn

[T31] Lua：Hello World
来源：http://nmk.wangdashe.top

print("Hello")
来源：http://yer.hcnkem.com

[T32] Lua：局部变量
来源：http://ngf.316326.xyz

local a = 1
来源：http://rxh.chenlongwang.top

[T33] Lua：表（数组）
来源：http://hue.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xmi.cdnleiting.top

[T34] Lua：遍历表
来源：http://vjt.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://jqj.52xcode.cn

[T35] Lua：字典表
来源：http://gke.daxiang520.top

local d = { a = 1 };  d.b = 2
来源：http://nkd.zhongyouzk.top

[T36] Lua：函数
来源：http://fbu.shuidangran.top

function add(a, b) return a + b end
来源：http://vzi.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://abv.52xcode.cn

"a" .. "b"
来源：http://tjn.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://sus.hywenlv.cn

if x > 0 then print("正") end
来源：http://ngw.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://pvn.zhijiandao.cn

string.find(s, "%d+")
来源：http://ggy.fengsongda.top

[T40] Lua：元表
来源：http://hwi.zycfv.cn

setmetatable({}, { __index = base })
来源：http://jbc.0kj1m.cn

[T41] Perl：Hello World
来源：http://tnu.gogol.net.cn

print "Hello\n";
来源：http://jti.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://srr.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nco.sxryk.cn

[T43] Perl：字符串插值
来源：http://wqe.jinqigfzy.top

"值: $a"
来源：http://ztm.daxiang520.top

[T44] Perl：条件
来源：http://gdt.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://fgm.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://jif.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://tqp.redwolf501.top

[T46] Perl：哈希操作
来源：http://fmx.pycfn.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zeb.dianchejie.cn

[T47] Perl：正则捕获
来源：http://zzb.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gtm.xuanzx.com

[T48] Perl：正则替换
来源：http://xuz.cdnleiting.top

$s =~ s/old/new/g;
来源：http://gug.tian-w.cn

[T49] Perl：函数
来源：http://bos.vqdsnc.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ywy.sufxvd.cn

[T50] Perl：逐行读文件
来源：http://dqb.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://jin.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://tam.mhx1999.top

[T51] Scala：Hello World
来源：http://gri.aibaodan.cn

println("Hello")
来源：http://qkd.hammf.cn

[T52] Scala：变量
来源：http://fqf.sxryk.cn

val a = 1;  var b = 2
来源：http://cal.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://uli.zhengqikj.top

s"值: $b"
来源：http://goc.hesvh.cn

[T54] Scala：集合映射
来源：http://cay.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://cza.xinyue.icu

[T55] Scala：集合过滤
来源：http://nsc.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://pjy.fzhhl.top

[T56] Scala：样例类
来源：http://fgp.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://mci.sufxvd.cn

[T57] Scala：模式匹配
来源：http://fvf.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jee.zhixingplan.top

[T58] Scala：函数定义
来源：http://fgn.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hnw.hammf.cn

[T59] Scala：循环
来源：http://thu.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://gbd.zhoulong.xyz

[T60] Scala：折叠
来源：http://jvx.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ium.ctjpmb.com

================================================================================
来源：http://rcn.hcnkem.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yhs.nwbrower.top

================================================================================
来源：http://nvb.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://det.xingfuxueyuan.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://cti.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://vkq.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cxf.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://eme.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://eeb.cheryme.top

[U04] Py：变量调试打印
来源：http://vzj.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://woc.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://win.gzhubu.top

list(dict.fromkeys(arr))
来源：http://xlu.iojbl.cn

[U06] Py：合并两个字典
来源：http://kvs.hammf.cn

{**a, **b}
来源：http://sly.gogol.net.cn

[U07] Py：反转字典键值
来源：http://hjv.hesvh.cn

{v: k for k, v in d.items()}
来源：http://vui.9152youxi.cn

[U08] Py：展平二维列表
来源：http://gch.sweek.top

[y for x in nested for y in x]
来源：http://tsu.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://ciw.zhiwuduotai.top

max(d, key=d.get)
来源：http://crt.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://tvs.zycfv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://axs.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://ccm.xinyue.icu

(x * 2 for x in arr)
来源：http://usq.guannengcc.top

[U12] Py：取出现最多的 3 个元素
来源：http://whl.ehwqpu.com

Counter(arr).most_common(3)
来源：http://sam.yangfankeji.com

[U13] Py：固定长度队列
来源：http://cjf.yfazqb.com

deque(maxlen=10)
来源：http://edd.daxiang520.top

[U14] Py：分组收集到列表
来源：http://ywm.xylfe.cn

defaultdict(list)
来源：http://rxj.hnxiangtu.top

[U15] Py：高精度计时
来源：http://ncv.jinghuilouyu.cn

t = time.perf_counter()
来源：http://ksb.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://yso.cheryme.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ukr.xuetiantiany.cn

[U17] Py：初始化日志
来源：http://ldx.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://xoj.fehbvm.com

[U18] Py：预编译正则
来源：http://iqp.cheryme.top

pat = re.compile(r"\d+")
来源：http://ood.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://vdf.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://asi.pycfn.com

[U20] Py：缓存函数结果
来源：http://lrd.zhiwuduotai.top

@functools.lru_cache(maxsize=None)
来源：http://pnk.ywan-chungtsiang.top

[U21] Py：自定义上下文管理器
来源：http://gaa.zdbjq.cn

@contextlib.contextmanager
来源：http://rkx.sweek.top

[U22] Py：矩阵转置
来源：http://owc.yanxiufei.cn

list(zip(*m))
来源：http://wxr.andypj.xyz

[U23] Py：分块读取大文件
来源：http://gto.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ssd.jinqigufen.top

[U24] Py：路径操作
来源：http://hmv.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://obx.kuanghao11.cn

[U25] Py：CSV 按字典读
来源：http://unt.yfazqb.com

csv.DictReader(f)
来源：http://vqd.xuanzx.com

[U26] Py：并发下载
来源：http://iwz.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://khd.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://utb.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://bbb.jqgufenzy.top

[U28] Py：类型别名
来源：http://zso.hywenlv.cn

UserId = int
来源：http://dni.316326.xyz

[U29] Py：属性校验
来源：http://ozs.sufxvd.cn

@property 与 @x.setter 配合
来源：http://bqe.uphjek.com

[U30] Py：数据类
来源：http://kpl.nanxuanxn.top

@dataclass(slots=True)
来源：http://kzd.chenzaomai.com


<!-- 参考信息 -->