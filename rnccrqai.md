代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vnr.iojbl.cn

[S10] C：指针与解引用
来源：http://tsg.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://xyw.pycfn.com

[S11] C：逐行读文件
来源：http://dzk.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://kbk.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vnw.hysaishi.cn

fclose(f);
来源：http://pts.zhengqikj.top

[S12] C：写文件
来源：http://zcv.xinyue.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wjc.yj20258.top

[S13] C：宏定义
来源：http://wtq.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zsm.feifeiyinyue.top

[S14] C：枚举
来源：http://yqh.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://uua.ppjwa.cn

[S15] C：类型转换
来源：http://djc.sufxvd.cn

(double) a / b
来源：http://kzm.yvedp.cn

[S16] C：位操作置位
来源：http://yfl.tarul.cn

x |= (1 << 3);
来源：http://giz.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://oqi.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jcn.yvedp.cn

[S18] C：命令行参数
来源：http://oin.9152youxi.cn

int main(int argc, char **argv)
来源：http://xve.daxiang520.top

[S19] C：快速排序
来源：http://npk.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://tcc.yj202588.top

[S20] C：二分查找
来源：http://awe.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iaf.mhx1999.top

[S21] C：字符类别判断
来源：http://vfk.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wgj.yuanzhike.top

[S22] C：字符串转数字
来源：http://glz.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://mvv.gzhubu.top

[S23] C：随机数
来源：http://sub.fehbvm.com

srand(time(NULL));  int r = rand() % 100;
来源：http://wpk.yongpay.top

[S24] C：获取本地时间
来源：http://utm.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vsm.guannengcc.top

[S25] C：内存拷贝
来源：http://uvn.yongpay.top

memcpy(dst, src, n);
来源：http://chj.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://pjy.hesvh.cn

memset(a, 0, sizeof a);
来源：http://jsr.0kj1m.cn

[S27] C：定义常量
来源：http://vig.hysaishi.cn

const double PI = 3.14159;
来源：http://xfc.cdnleiting.top

[S28] C：静态变量
来源：http://mxn.zdbjq.cn

static int counter = 0;
来源：http://ksd.ydzc1.top

[S29] C：变参函数
来源：http://xav.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ach.cheryme.top

[S30] C：头文件保护
来源：http://dap.yongpay.top

#ifndef X_H
来源：http://jvw.hfpthk.cn

#define X_H
来源：http://lof.jiagoushi.top

#endif
来源：http://zyg.shzxlz.cn

[S31] C++：Hello World
来源：http://roh.daxiang520.top

#include <iostream>
来源：http://jcv.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://egx.iojbl.cn

[S32] C++：字符串
来源：http://ngl.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://ytb.jinqigfzy.top

[S33] C++：vector 增删
来源：http://xex.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pxx.tianlin.xyz

[S34] C++：遍历 vector
来源：http://kwe.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://uno.aizwys.cn

[S35] C++：map
来源：http://btp.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tot.c1oappe.top

[S36] C++：unordered_map
来源：http://qhc.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qhi.zycfv.cn

[S37] C++：set
来源：http://rfg.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://odq.jianghu66.top

[S38] C++：排序
来源：http://wuw.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://qvw.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://koi.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zns.hysaishi.cn

[S40] C++：查找元素
来源：http://rnk.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uhe.andypj.xyz

[S41] C++：类与构造函数
来源：http://lre.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qpx.zycfv.cn

[S42] C++：继承与虚函数
来源：http://duw.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://qtb.sjlbkw.cn

[S43] C++：智能指针
来源：http://kdj.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://gps.ydjk.org.cn

[S44] C++：引用传参
来源：http://ysd.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://hab.gzhubu.top

[S45] C++：lambda
来源：http://ygh.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://nrp.feifeiyinyue.top

[S46] C++：函数模板
来源：http://trr.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vny.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://vgn.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oyq.svipenyu.cn

[S48] C++：逐行读文件
来源：http://gza.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://xpv.hesvh.cn

while (std::getline(in, line)) { }
来源：http://xhr.fzhhl.top

[S49] C++：写文件
来源：http://ccr.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wfi.xuanzx.com

[S50] C++：格式化数字
来源：http://loa.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wlt.guowangkeji.top

[S51] C++：显式类型转换
来源：http://rrd.hcnkem.com

static_cast<double>(a) / b
来源：http://nag.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://nbp.316326.xyz

int size() const noexcept { return n_; }
来源：http://uqd.ydjk.org.cn

[S53] C++：移动语义
来源：http://xep.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://vki.yanxiufei.cn

[S54] C++：异常处理
来源：http://hhz.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fnu.sweek.top

[S55] C++：结构化绑定
来源：http://jah.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bpv.zhiwuduotai.top

[S56] C++：optional
来源：http://wqu.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iej.ehwqpu.com

[S57] C++：编译期常量
来源：http://xlm.xylfe.cn

constexpr int N = 10;
来源：http://svz.jiagoushi.top

[S58] C++：命名空间
来源：http://toy.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://gzg.haohaochexian.top

[S59] C++：静态断言
来源：http://suv.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jsw.cashguo.top

[S60] C++：遍历并删除元素
来源：http://owe.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gfm.havefunace.top

================================================================================
来源：http://psr.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jhc.gzhubu.top

================================================================================
来源：http://psr.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://cit.jinyuanbaomall.cn

println("Hello")
来源：http://zxf.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://scz.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eoq.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://gsg.cdnleiting.top

"值: $b"
来源：http://izi.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://hkl.316326.xyz

val n: String? = null;  n?.length
来源：http://sst.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://szm.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jab.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://ucb.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hvt.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://goj.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mtt.mhx1999.top

[T08] Kotlin：数据类
来源：http://zbq.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://eet.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://vrs.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://ceq.jianghu66.top

[T10] Kotlin：默认参数
来源：http://xjr.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://brx.iojbl.cn

[T11] Kotlin：协程
来源：http://pzt.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://awb.pycfn.com

[T12] Kotlin：解构声明
来源：http://ute.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://rdw.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://wrw.yongpay.top

val m = mapOf("a" to 1)
来源：http://qjb.hnxiangtu.top

[T14] Kotlin：循环
来源：http://afi.bbcook.cn

for (i in 1..10) println(i)
来源：http://dwq.birdmap.top

[T15] Kotlin：接口
来源：http://uqj.shanyushiyangkeji.top

interface Shape { fun area(): Double }
来源：http://rdw.yonumen.top

[T16] Swift：Hello World
来源：http://tar.hammf.cn

print("Hello")
来源：http://aho.hammf.cn

[T17] Swift：变量与常量
来源：http://leq.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://hda.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://egk.cheryme.top

"值: \(b)"
来源：http://iyj.cucudq.cn

[T19] Swift：可选绑定
来源：http://bxf.guannengcc.top

if let n = opt { print(n) }
来源：http://seu.hnxiangtu.top

[T20] Swift：数组操作
来源：http://jsm.ybcxt.top

var a = [1, 2, 3];  a.append(4)
来源：http://rev.gzhubu.top

[T21] Swift：遍历
来源：http://ctv.hammf.cn

for x in a { print(x) }
来源：http://rsi.hywenlv.cn

[T22] Swift：字典
来源：http://lva.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://aui.bbcook.cn

[T23] Swift：函数
来源：http://rmb.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vtt.birdmap.top

[T24] Swift：闭包
来源：http://myy.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fnw.aizwys.cn

[T25] Swift：结构体
来源：http://jfk.meibo888.top

struct P { var x: Int }
来源：http://wbe.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://wyi.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://bhw.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://xry.pycfn.com

do { try f() } catch { print(error) }
来源：http://zov.0kj1m.cn

[T28] Swift：枚举
来源：http://lcx.jyoumei.cn

enum Color { case red, green }
来源：http://vah.xylfe.cn

[T29] Swift：guard 提前返回
来源：http://yvf.jqgfzy.top

guard let x = opt else { return }
来源：http://hyq.hongshengwenyu.top

[T30] Swift：协议
来源：http://eid.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://tjy.zdqjudy.top

[T31] Lua：Hello World
来源：http://fvo.ydzc1.top

print("Hello")
来源：http://tsh.yj20258888.top

[T32] Lua：局部变量
来源：http://kwq.yfazqb.com

local a = 1
来源：http://lts.gotoacloud.top

[T33] Lua：表（数组）
来源：http://msq.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ibp.hfpthk.cn

[T34] Lua：遍历表
来源：http://mue.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://emk.jqgufenzy.top

[T35] Lua：字典表
来源：http://cuh.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://aws.ybcxt.top

[T36] Lua：函数
来源：http://lng.aibaodan.cn

function add(a, b) return a + b end
来源：http://xpr.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://wfk.dashuyun.cn

"a" .. "b"
来源：http://xkf.jyoumei.cn

[T38] Lua：条件
来源：http://vzt.gzhubu.top

if x > 0 then print("正") end
来源：http://uos.pycfn.com

[T39] Lua：模式匹配
来源：http://kyf.sufxvd.cn

string.find(s, "%d+")
来源：http://ojp.jiagoushi.top

[T40] Lua：元表
来源：http://aii.tanke756.top

setmetatable({}, { __index = base })
来源：http://wmu.0kj1m.cn

[T41] Perl：Hello World
来源：http://fwq.pengpengdd.cyou

print "Hello\n";
来源：http://jrp.wangdashe.top

[T42] Perl：变量类型
来源：http://uqj.wangshuangyany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qdr.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://xrm.shuidangran.top

"值: $a"
来源：http://lfg.chenjidiqi.icu

[T44] Perl：条件
来源：http://buk.hammf.cn

if ($a > 0) { print "正"; }
来源：http://sdy.cucudq.cn

[T45] Perl：数组遍历
来源：http://bpb.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://daf.jinghuilouyu.cn

[T46] Perl：哈希操作
来源：http://orq.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eha.cucudq.cn

[T47] Perl：正则捕获
来源：http://wzt.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://acc.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://njy.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://xxj.xingfuxueyuan.xyz

[T49] Perl：函数
来源：http://hoo.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://npn.cheryme.top

[T50] Perl：逐行读文件
来源：http://csx.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rvu.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://jsk.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://wxz.cqqwz.cn

println("Hello")
来源：http://ciz.tianlin.xyz

[T52] Scala：变量
来源：http://rkf.nanxinkj.top

val a = 1;  var b = 2
来源：http://aap.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://cdu.andypj.xyz

s"值: $b"
来源：http://dvr.pengpengdd.cyou

[T54] Scala：集合映射
来源：http://htz.nanxinkj.top

List(1, 2, 3).map(_ * 2)
来源：http://ktf.xinyue.icu

[T55] Scala：集合过滤
来源：http://sng.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gxl.chenlongwang.top

[T56] Scala：样例类
来源：http://pid.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://hks.mhx1999.top

[T57] Scala：模式匹配
来源：http://xrs.tarul.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aps.ydjk.org.cn

[T58] Scala：函数定义
来源：http://fif.sysykeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://xzh.quarkkingdee.top

[T59] Scala：循环
来源：http://ruh.shanyushiyangtech.top

for (i <- 1 to 10) println(i)
来源：http://dps.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://wep.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://naj.cucudq.cn

================================================================================
来源：http://xfo.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xjy.yuanzhike.top

================================================================================
来源：http://tfg.cheryme.top

[U01] Py：创建虚拟环境
来源：http://wif.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nav.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://ftv.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dux.zycfv.cn

[U03] Py：加载 .env 配置
来源：http://rgs.yj202588.top

from dotenv import load_dotenv; load_dotenv()
来源：http://upn.zhixingplan.top

[U04] Py：变量调试打印
来源：http://ftx.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://swp.xinyue.icu

[U05] Py：列表去重且保序
来源：http://udp.bbcook.cn

list(dict.fromkeys(arr))
来源：http://yxe.gotoacloud.top

[U06] Py：合并两个字典
来源：http://hao.cdnleiting.top

{**a, **b}
来源：http://mjl.ehwqpu.com

[U07] Py：反转字典键值
来源：http://ffe.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://mjt.shuidangran.top

[U08] Py：展平二维列表
来源：http://xqc.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://xqv.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://nfd.daxiang520.top

max(d, key=d.get)
来源：http://sru.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://fjf.vehdjk.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zrg.shuidangran.top

[U11] Py：生成器表达式
来源：http://oog.shanyushiyangtech.top

(x * 2 for x in arr)
来源：http://asb.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://lbc.wangdashe.top

Counter(arr).most_common(3)
来源：http://nuh.yvedp.cn

[U13] Py：固定长度队列
来源：http://xey.c1oappe.top

deque(maxlen=10)
来源：http://qaq.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://eod.hysaishi.cn

defaultdict(list)
来源：http://rxg.yuxming.cn

[U15] Py：高精度计时
来源：http://yyw.fktsv.cn

t = time.perf_counter()
来源：http://thw.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://vdb.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yus.vehdjk.com

[U17] Py：初始化日志
来源：http://bxw.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://gep.pycfn.com

[U18] Py：预编译正则
来源：http://pmc.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://jzk.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://lae.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xth.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://dxd.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://pat.ctjpmb.com

[U21] Py：自定义上下文管理器
来源：http://umo.yj20258.top

@contextlib.contextmanager
来源：http://ott.yonumen.top

[U22] Py：矩阵转置
来源：http://hzf.yuxming.cn

list(zip(*m))
来源：http://cir.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://isn.haohaochexian.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://smm.smart0.xyz

[U24] Py：路径操作
来源：http://tgo.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jie.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://szd.fehbvm.com

csv.DictReader(f)
来源：http://dnj.hfpthk.cn

[U26] Py：并发下载
来源：http://fyp.xingfuxueyuan.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ito.yonumen.top

[U27] Py：异步 HTTP
来源：http://mek.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://moc.smart0.xyz

[U28] Py：类型别名
来源：http://hzp.jiagoushi.top

UserId = int
来源：http://mgu.bjfxy.top

[U29] Py：属性校验
来源：http://rzb.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://imr.fanxiaobao.xyz

[U30] Py：数据类
来源：http://evu.mhx1999.top

@dataclass(slots=True)
来源：http://eno.yongpay.top

[U31] Py：单测
来源：http://gvi.guowangkeji.top

python -m pytest -q
来源：http://sil.pycfn.com

[U32] Py：代码格式化
来源：http://qwb.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://ovp.snrcjt.cn


<!-- 参考信息 -->