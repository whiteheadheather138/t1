代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dir.feifeiyinyue.top

[S08] C：动态内存分配与释放
来源：http://woi.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qrs.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://bpw.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zup.fktsv.cn

[S10] C：指针与解引用
来源：http://xet.yonumen.top

int *p = &a;  *p = 5;
来源：http://erv.zycfv.cn

[S11] C：逐行读文件
来源：http://opm.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://rzm.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iwb.chenzaomai.com

fclose(f);
来源：http://xxv.guowangkeji.top

[S12] C：写文件
来源：http://rgm.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tnw.zhaomingkeji.xyz

[S13] C：宏定义
来源：http://cxk.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qco.dashuyun.cn

[S14] C：枚举
来源：http://tlg.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://wao.epnwcf.com

[S15] C：类型转换
来源：http://rlc.guowangkeji.top

(double) a / b
来源：http://fbf.ydzc1.top

[S16] C：位操作置位
来源：http://emk.shangyingyoupin.top

x |= (1 << 3);
来源：http://blt.quarkkingdee.top

[S17] C：安全拼接字符串
来源：http://fld.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rcs.zycfv.cn

[S18] C：命令行参数
来源：http://wuk.c1oappe.top

int main(int argc, char **argv)
来源：http://nil.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://gal.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fww.bjfxy.top

[S20] C：二分查找
来源：http://wgh.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bnt.ydjk.org.cn

[S21] C：字符类别判断
来源：http://luh.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://llb.pycfn.com

[S22] C：字符串转数字
来源：http://eel.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dqe.ppjwa.cn

[S23] C：随机数
来源：http://wov.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ylw.yuanzhike.top

[S24] C：获取本地时间
来源：http://vrv.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lmd.guowangkeji.top

[S25] C：内存拷贝
来源：http://sjh.xinyue.icu

memcpy(dst, src, n);
来源：http://zjq.xziqi.cn

[S26] C：内存清零
来源：http://hvh.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://abs.guowangkeji.top

[S27] C：定义常量
来源：http://nxx.hnxiangtu.top

const double PI = 3.14159;
来源：http://kli.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://szw.hammf.cn

static int counter = 0;
来源：http://rlg.aibaodan.cn

[S29] C：变参函数
来源：http://ogv.haohaochexian.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fwh.jiagoushi.top

[S30] C：头文件保护
来源：http://wmh.zhiwuduotai.top

#ifndef X_H
来源：http://god.havefunace.top

#define X_H
来源：http://qtu.meibo888.top

#endif
来源：http://usj.yvedp.cn

[S31] C++：Hello World
来源：http://rld.vqdsnc.cn

#include <iostream>
来源：http://ins.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://pzm.birdmap.top

[S32] C++：字符串
来源：http://ksj.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://dee.aibaodan.cn

[S33] C++：vector 增删
来源：http://kio.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vvd.svipenyu.cn

[S34] C++：遍历 vector
来源：http://udd.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://dkz.aibaodan.cn

[S35] C++：map
来源：http://xwk.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://snx.zhijiandao.cn

[S36] C++：unordered_map
来源：http://evc.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://efm.jianghu66.top

[S37] C++：set
来源：http://moi.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://csc.jinghuilouyu.cn

[S38] C++：排序
来源：http://lef.ivvv.top

std::sort(v.begin(), v.end());
来源：http://dwr.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://bps.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lks.yangfankeji.com

[S40] C++：查找元素
来源：http://gls.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xxu.shzxlz.cn

[S41] C++：类与构造函数
来源：http://zwm.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nnn.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://ulr.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://ybc.bjfxy.top

[S43] C++：智能指针
来源：http://hvc.sjlbkw.cn

auto p = std::make_unique<int>(5);
来源：http://tjn.jinqigufen.top

[S44] C++：引用传参
来源：http://zir.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://pwt.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://pgw.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://zch.sufxvd.cn

[S46] C++：函数模板
来源：http://cyw.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://equ.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://ynl.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rbt.guannengcc.top

[S48] C++：逐行读文件
来源：http://wdk.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jmi.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://yws.zhengqikj.top

[S49] C++：写文件
来源：http://gnt.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eij.0kj1m.cn

[S50] C++：格式化数字
来源：http://qar.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hby.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://fus.hesvh.cn

static_cast<double>(a) / b
来源：http://mqh.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://qim.bjfxy.top

int size() const noexcept { return n_; }
来源：http://szc.guannengcc.top

[S53] C++：移动语义
来源：http://wmd.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://aky.jinqigufen.top

[S54] C++：异常处理
来源：http://abq.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://swb.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://ish.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pys.nanxuanxn.top

[S56] C++：optional
来源：http://dib.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gbu.tarul.cn

[S57] C++：编译期常量
来源：http://tfo.yvedp.cn

constexpr int N = 10;
来源：http://epz.cdnleiting.top

[S58] C++：命名空间
来源：http://pgn.zhixingplan.top

namespace ns { int f() { return 1; } }
来源：http://pmn.wangshuangyany.cn

[S59] C++：静态断言
来源：http://eix.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fmm.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://kmz.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://odp.ivvv.top

================================================================================
来源：http://pby.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ciu.jqgfzy.top

================================================================================
来源：http://agd.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://rkk.yj20258.top

println("Hello")
来源：http://let.svipenyu.cn

[T02] Kotlin：变量
来源：http://myq.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hhz.yongpay.top

[T03] Kotlin：字符串模板
来源：http://tnc.daxiang520.top

"值: $b"
来源：http://bgm.fehbvm.com

[T04] Kotlin：空安全
来源：http://twp.zhengqikj.top

val n: String? = null;  n?.length
来源：http://pkg.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://amr.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pku.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://xyb.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hkz.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://eeh.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://exi.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://hhi.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://yfp.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://byr.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://zjb.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://krg.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mcp.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://cma.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://usc.uphjek.com

[T12] Kotlin：解构声明
来源：http://pbh.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://bal.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://myd.mhx1999.top

val m = mapOf("a" to 1)
来源：http://hnq.tanke756.top

[T14] Kotlin：循环
来源：http://dst.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://psu.jyoumei.cn

[T15] Kotlin：接口
来源：http://aak.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://xke.nwbrower.top

[T16] Swift：Hello World
来源：http://zah.dashuyun.cn

print("Hello")
来源：http://cbd.0kj1m.cn

[T17] Swift：变量与常量
来源：http://yjj.chenzaomai.com

var a = 1;  let b = 2
来源：http://nli.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://cru.0kj1m.cn

"值: \(b)"
来源：http://qfo.bbcook.cn

[T19] Swift：可选绑定
来源：http://lhp.meibo888.top

if let n = opt { print(n) }
来源：http://eoc.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://ddt.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sxv.hammf.cn

[T21] Swift：遍历
来源：http://vlo.yangfankeji.com

for x in a { print(x) }
来源：http://och.yangfankeji.com

[T22] Swift：字典
来源：http://sym.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://mgn.zhijiandao.cn

[T23] Swift：函数
来源：http://ghq.jlsjyb.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zsg.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://rxr.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ikk.jqgfzy.top

[T25] Swift：结构体
来源：http://suc.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://ioh.fehbvm.com

[T26] Swift：类与重写
来源：http://fln.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://sid.jlsjyb.cn

[T27] Swift：错误处理
来源：http://ezu.vehdjk.com

do { try f() } catch { print(error) }
来源：http://nfy.ivvv.top

[T28] Swift：枚举
来源：http://gvf.xuanzx.com

enum Color { case red, green }
来源：http://wtj.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://ypq.dashuyun.cn

guard let x = opt else { return }
来源：http://efd.vqdsnc.cn

[T30] Swift：协议
来源：http://zko.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://kyz.bbcook.cn

[T31] Lua：Hello World
来源：http://rhg.xuanzx.com

print("Hello")
来源：http://fya.shzxlz.cn

[T32] Lua：局部变量
来源：http://igp.hcnkem.com

local a = 1
来源：http://lpj.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://fmj.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sgo.ehwqpu.com

[T34] Lua：遍历表
来源：http://tcq.yonumen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wwl.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://bmc.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://kod.yj20258888.top

[T36] Lua：函数
来源：http://umx.bjfxy.top

function add(a, b) return a + b end
来源：http://exu.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://kfx.316326.xyz

"a" .. "b"
来源：http://crv.sjlbkw.cn

[T38] Lua：条件
来源：http://clo.cashguo.top

if x > 0 then print("正") end
来源：http://zbn.aizwys.cn

[T39] Lua：模式匹配
来源：http://fgk.ybcxt.top

string.find(s, "%d+")
来源：http://zgf.jiagoushi.top

[T40] Lua：元表
来源：http://sjr.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://nal.uphjek.com

[T41] Perl：Hello World
来源：http://vjq.zhoulong.xyz

print "Hello\n";
来源：http://xtu.yj20258888.top

[T42] Perl：变量类型
来源：http://xis.shanyushiyangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hqt.uphjek.com

[T43] Perl：字符串插值
来源：http://msj.daxiang520.top

"值: $a"
来源：http://zve.sufxvd.cn

[T44] Perl：条件
来源：http://ybv.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://ktm.cqqwz.cn

[T45] Perl：数组遍历
来源：http://xgv.fktsv.cn

for my $x (@arr) { print $x; }
来源：http://nvc.hesvh.cn

[T46] Perl：哈希操作
来源：http://xvx.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://onq.hfpthk.cn

[T47] Perl：正则捕获
来源：http://qbc.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bko.yfazqb.com

[T48] Perl：正则替换
来源：http://smi.yuxming.cn

$s =~ s/old/new/g;
来源：http://oox.ydjk.org.cn

[T49] Perl：函数
来源：http://gfy.epnwcf.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://icy.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://ilw.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zlf.shangyingyoupin.top

while (my $line = <$fh>) { print $line; }
来源：http://qmj.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://iqo.xuanzx.com

println("Hello")
来源：http://wki.hongshengwenyu.top

[T52] Scala：变量
来源：http://zzm.nwbrower.top

val a = 1;  var b = 2
来源：http://mmu.bjfxy.top

[T53] Scala：字符串插值
来源：http://mxn.dianchejie.cn

s"值: $b"
来源：http://trj.yangfankeji.com

[T54] Scala：集合映射
来源：http://ofh.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://poj.yongpay.top

[T55] Scala：集合过滤
来源：http://rli.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://abg.feifeiyinyue.top

[T56] Scala：样例类
来源：http://ulf.nwbrower.top

case class User(name: String, age: Int)
来源：http://kuu.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://jem.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://fub.vehdjk.com

[T58] Scala：函数定义
来源：http://hqa.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://jlb.mhx1999.top

[T59] Scala：循环
来源：http://zyy.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://dsp.sysykeji.top

[T60] Scala：折叠
来源：http://igp.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://trb.jinqigfzy.top

================================================================================
来源：http://cgi.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qyz.ywan-chungtsiang.top

================================================================================
来源：http://wyc.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://fzs.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hsy.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://zuy.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gjv.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://jiz.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://liy.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://rvi.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ywc.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://sgv.fehbvm.com

list(dict.fromkeys(arr))
来源：http://ohh.nanxinkj.top

[U06] Py：合并两个字典
来源：http://uiu.sysykeji.top

{**a, **b}
来源：http://cyh.shanyushiyangtech.top

[U07] Py：反转字典键值
来源：http://ukh.sysykeji.top

{v: k for k, v in d.items()}
来源：http://pzt.hnqzz.top

[U08] Py：展平二维列表
来源：http://mjt.sxryk.cn

[y for x in nested for y in x]
来源：http://wcd.yanxiufei.cn

[U09] Py：字典取最大值的键
来源：http://ajf.uphjek.com

max(d, key=d.get)
来源：http://qas.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://ekk.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jbr.meibo888.top

[U11] Py：生成器表达式
来源：http://ccd.iojbl.cn

(x * 2 for x in arr)
来源：http://ggf.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qzo.jqgfzy.top

Counter(arr).most_common(3)
来源：http://hbz.ehwqpu.com

[U13] Py：固定长度队列
来源：http://llv.bbcook.cn

deque(maxlen=10)
来源：http://thj.zycfv.cn

[U14] Py：分组收集到列表
来源：http://qdt.jiagoushi.top

defaultdict(list)
来源：http://cht.tarul.cn

[U15] Py：高精度计时
来源：http://hci.daria6918.cn

t = time.perf_counter()
来源：http://wec.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://lpx.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zbo.yonumen.top

[U17] Py：初始化日志
来源：http://rsr.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://zii.c1oappe.top

[U18] Py：预编译正则
来源：http://qyt.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://exm.sysykeji.top

[U19] Py：正则替换带回调
来源：http://cju.fzhhl.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dqx.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://rkv.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://qqp.ywan-chungtsiang.top

[U21] Py：自定义上下文管理器
来源：http://dzr.0kj1m.cn

@contextlib.contextmanager
来源：http://jli.haohaochexian.top

[U22] Py：矩阵转置
来源：http://arm.yuxming.cn

list(zip(*m))
来源：http://yxb.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://svf.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mvm.zhengqikj.top

[U24] Py：路径操作
来源：http://kjy.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jdi.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://bbj.fengsongda.top

csv.DictReader(f)
来源：http://woc.bjfxy.top

[U26] Py：并发下载
来源：http://erw.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tem.redwolf501.top

[U27] Py：异步 HTTP
来源：http://bvl.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://gji.pycfn.com

[U28] Py：类型别名
来源：http://zfm.yfazqb.com

UserId = int
来源：http://nyw.jlsjyb.cn

[U29] Py：属性校验
来源：http://txu.52xcode.cn

@property 与 @x.setter 配合
来源：http://wbl.wangdashe.top

[U30] Py：数据类
来源：http://kmc.tanke756.top

@dataclass(slots=True)
来源：http://zey.cdnleiting.top


<!-- 参考信息 -->