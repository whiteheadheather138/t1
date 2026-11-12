代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rqq.zycfv.cn

[S10] C：指针与解引用
来源：http://npf.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://khj.andypj.xyz

[S11] C：逐行读文件
来源：http://rmx.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://rvt.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hgj.sxryk.cn

fclose(f);
来源：http://fjy.bjfxy.top

[S12] C：写文件
来源：http://fly.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ypb.wangshuangyany.cn

[S13] C：宏定义
来源：http://ort.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ioh.jianghu66.top

[S14] C：枚举
来源：http://dtv.tian-w.cn

enum Color { RED, GREEN, BLUE };
来源：http://rbl.fengsongda.top

[S15] C：类型转换
来源：http://jox.yangfankeji.com

(double) a / b
来源：http://qpx.ybcxt.top

[S16] C：位操作置位
来源：http://tmg.xuanzx.com

x |= (1 << 3);
来源：http://wqi.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://jgf.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cxo.jinqigfzy.top

[S18] C：命令行参数
来源：http://jho.xylfe.cn

int main(int argc, char **argv)
来源：http://yxp.jyoumei.cn

[S19] C：快速排序
来源：http://zrw.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://pkl.ydzc1.top

[S20] C：二分查找
来源：http://tgm.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://owq.nanxuanxn.top

[S21] C：字符类别判断
来源：http://jhl.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gbp.pengpengdd.cyou

[S22] C：字符串转数字
来源：http://elf.hfpthk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jrk.zhengqikj.top

[S23] C：随机数
来源：http://wmv.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sui.pycfn.com

[S24] C：获取本地时间
来源：http://xhl.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cdw.wangdashe.top

[S25] C：内存拷贝
来源：http://cvh.316326.xyz

memcpy(dst, src, n);
来源：http://ddy.hammf.cn

[S26] C：内存清零
来源：http://jio.vehdjk.com

memset(a, 0, sizeof a);
来源：http://vlf.mhx1999.top

[S27] C：定义常量
来源：http://qly.gaohongyu789.top

const double PI = 3.14159;
来源：http://kbs.tianlin.xyz

[S28] C：静态变量
来源：http://zjr.hysaishi.cn

static int counter = 0;
来源：http://mvy.chenjidiqi.icu

[S29] C：变参函数
来源：http://jhr.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wjd.chenzaomai.com

[S30] C：头文件保护
来源：http://cvu.birdmap.top

#ifndef X_H
来源：http://xxn.sysykeji.top

#define X_H
来源：http://aoj.shanyushiyangkeji.top

#endif
来源：http://ujt.mhx1999.top

[S31] C++：Hello World
来源：http://fmx.pengpengdd.cyou

#include <iostream>
来源：http://sae.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://xvt.chenjidiqi.icu

[S32] C++：字符串
来源：http://pja.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://zmi.iojbl.cn

[S33] C++：vector 增删
来源：http://qsh.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://llq.mhx1999.top

[S34] C++：遍历 vector
来源：http://epe.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://ojb.bbcook.cn

[S35] C++：map
来源：http://jxp.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hox.sweek.top

[S36] C++：unordered_map
来源：http://dyx.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hka.yj20258888.top

[S37] C++：set
来源：http://tvj.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zvf.daria6918.cn

[S38] C++：排序
来源：http://sdo.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://gbz.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://fhk.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eva.ydjk.org.cn

[S40] C++：查找元素
来源：http://ijx.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uqw.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://goc.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rxy.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://bng.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://pjv.yuxming.cn

[S43] C++：智能指针
来源：http://ifl.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://mcn.daxiang520.top

[S44] C++：引用传参
来源：http://pcw.uphjek.com

void inc(int &x) { ++x; }
来源：http://cie.cashguo.top

[S45] C++：lambda
来源：http://gnp.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://viw.jiagoushi.top

[S46] C++：函数模板
来源：http://guq.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lld.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://jxo.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kvt.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://cvh.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://cyj.xziqi.cn

while (std::getline(in, line)) { }
来源：http://cro.meibo888.top

[S49] C++：写文件
来源：http://tok.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vqo.gaohongyu789.top

[S50] C++：格式化数字
来源：http://pwl.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qcn.shzxlz.cn

[S51] C++：显式类型转换
来源：http://fnh.316326.xyz

static_cast<double>(a) / b
来源：http://ize.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://yuq.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://hyk.shzxlz.cn

[S53] C++：移动语义
来源：http://nsk.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://wve.birdmap.top

[S54] C++：异常处理
来源：http://fbe.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kil.bjfxy.top

[S55] C++：结构化绑定
来源：http://lsu.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ena.uphjek.com

[S56] C++：optional
来源：http://jwe.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ily.yj20258888.top

[S57] C++：编译期常量
来源：http://fam.9152youxi.cn

constexpr int N = 10;
来源：http://kos.fehbvm.com

[S58] C++：命名空间
来源：http://vrb.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://pfs.jiagoushi.top

[S59] C++：静态断言
来源：http://laf.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lcz.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://dly.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://srd.tianlin.xyz

================================================================================
来源：http://oro.ybcxt.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kya.yongpay.top

================================================================================
来源：http://jge.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://vjv.zhijiandao.cn

println("Hello")
来源：http://qtb.jiagoushi.top

[T02] Kotlin：变量
来源：http://ckt.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gbm.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://xdu.birdmap.top

"值: $b"
来源：http://sgk.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://qln.cucudq.cn

val n: String? = null;  n?.length
来源：http://anq.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://kwt.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cnu.daxiang520.top

[T06] Kotlin：集合映射
来源：http://cbg.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vnt.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://vnd.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mrh.hesvh.cn

[T08] Kotlin：数据类
来源：http://dol.tanke756.top

data class User(val name: String, val age: Int)
来源：http://ghg.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://luj.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://sag.fengsongda.top

[T10] Kotlin：默认参数
来源：http://rii.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sep.sjlbkw.cn

[T11] Kotlin：协程
来源：http://pqo.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rlx.jianghu66.top

[T12] Kotlin：解构声明
来源：http://sko.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://nlk.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://rpi.sweek.top

val m = mapOf("a" to 1)
来源：http://lju.gzhubu.top

[T14] Kotlin：循环
来源：http://pct.mhx1999.top

for (i in 1..10) println(i)
来源：http://hcv.smart0.xyz

[T15] Kotlin：接口
来源：http://qlg.xuanzx.com

interface Shape { fun area(): Double }
来源：http://lhq.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://vti.jqgfzy.top

print("Hello")
来源：http://uzw.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://shr.yvedp.cn

var a = 1;  let b = 2
来源：http://sai.redwolf501.top

[T18] Swift：字符串插值
来源：http://sui.ctjpmb.com

"值: \(b)"
来源：http://usp.shuidangran.top

[T19] Swift：可选绑定
来源：http://oif.sufxvd.cn

if let n = opt { print(n) }
来源：http://hfe.yj202588.top

[T20] Swift：数组操作
来源：http://kbt.fehbvm.com

var a = [1, 2, 3];  a.append(4)
来源：http://tgm.fehbvm.com

[T21] Swift：遍历
来源：http://jdm.zdqjudy.top

for x in a { print(x) }
来源：http://hld.feifeiyinyue.top

[T22] Swift：字典
来源：http://ukd.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bkn.shanyushiyangkeji.top

[T23] Swift：函数
来源：http://wix.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tdw.cdnleiting.top

[T24] Swift：闭包
来源：http://wyk.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://suq.jinqigufen.top

[T25] Swift：结构体
来源：http://khk.ydzc1.top

struct P { var x: Int }
来源：http://hfs.zhixingplan.top

[T26] Swift：类与重写
来源：http://bet.xylfe.cn

class A: Base { override func f() {} }
来源：http://vph.hywenlv.cn

[T27] Swift：错误处理
来源：http://wgq.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://cdk.haohaochexian.top

[T28] Swift：枚举
来源：http://bdd.aibaodan.cn

enum Color { case red, green }
来源：http://pqq.sweek.top

[T29] Swift：guard 提前返回
来源：http://nkc.gotoacloud.top

guard let x = opt else { return }
来源：http://fqp.ybcxt.top

[T30] Swift：协议
来源：http://xuy.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://wgi.hfpthk.cn

[T31] Lua：Hello World
来源：http://ifq.birdmap.top

print("Hello")
来源：http://ujf.sweek.top

[T32] Lua：局部变量
来源：http://bjy.vqdsnc.cn

local a = 1
来源：http://gmn.xinyue.icu

[T33] Lua：表（数组）
来源：http://zkk.ydzc1.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zoj.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://ujn.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vzt.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://mwn.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://mti.yueranfly.top

[T36] Lua：函数
来源：http://qyl.chenjidiqi.icu

function add(a, b) return a + b end
来源：http://mvf.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://ycz.jqgfzy.top

"a" .. "b"
来源：http://tyd.meibo888.top

[T38] Lua：条件
来源：http://hvv.xziqi.cn

if x > 0 then print("正") end
来源：http://uum.guowangkeji.top

[T39] Lua：模式匹配
来源：http://glv.aibaodan.cn

string.find(s, "%d+")
来源：http://evs.gzhubu.top

[T40] Lua：元表
来源：http://aob.andypj.xyz

setmetatable({}, { __index = base })
来源：http://uga.pycfn.com

[T41] Perl：Hello World
来源：http://srg.sufxvd.cn

print "Hello\n";
来源：http://rgg.jinqigfzy.top

[T42] Perl：变量类型
来源：http://yza.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bfh.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://pzq.yanxiufei.cn

"值: $a"
来源：http://jhz.xuetiantiany.cn

[T44] Perl：条件
来源：http://ygr.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://rbj.hnqzz.top

[T45] Perl：数组遍历
来源：http://oek.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://vul.ehwqpu.com

[T46] Perl：哈希操作
来源：http://fgg.hongshengwenyu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://maq.bjfxy.top

[T47] Perl：正则捕获
来源：http://faz.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cfx.ybcxt.top

[T48] Perl：正则替换
来源：http://icr.cashguo.top

$s =~ s/old/new/g;
来源：http://hpo.jinqigufen.top

[T49] Perl：函数
来源：http://owp.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dtk.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://kay.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://amm.uphjek.com

while (my $line = <$fh>) { print $line; }
来源：http://aej.yueranfly.top

[T51] Scala：Hello World
来源：http://war.mhx1999.top

println("Hello")
来源：http://hrz.tianlin.xyz

[T52] Scala：变量
来源：http://kxk.meibo888.top

val a = 1;  var b = 2
来源：http://lta.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://qhf.cqqwz.cn

s"值: $b"
来源：http://gfy.316326.xyz

[T54] Scala：集合映射
来源：http://taz.ehwqpu.com

List(1, 2, 3).map(_ * 2)
来源：http://yrv.zhixingplan.top

[T55] Scala：集合过滤
来源：http://xoy.nanxinkj.top

List(1, 2, 3).filter(_ > 1)
来源：http://ufc.aizwys.cn

[T56] Scala：样例类
来源：http://zzm.cucudq.cn

case class User(name: String, age: Int)
来源：http://jcs.yj202588.top

[T57] Scala：模式匹配
来源：http://ixe.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sbc.aizwys.cn

[T58] Scala：函数定义
来源：http://sbq.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://aki.zycfv.cn

[T59] Scala：循环
来源：http://gtd.nwbrower.top

for (i <- 1 to 10) println(i)
来源：http://vyh.jlsjyb.cn

[T60] Scala：折叠
来源：http://kss.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xww.zhaomingkeji.xyz

================================================================================
来源：http://str.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bkg.c1oappe.top

================================================================================
来源：http://nkj.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://fzy.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://xvh.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://czd.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yrw.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://dym.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rzd.pycfn.com

[U04] Py：变量调试打印
来源：http://och.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fgw.wangshuangyany.cn

[U05] Py：列表去重且保序
来源：http://pzb.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://cxx.dashuyun.cn

[U06] Py：合并两个字典
来源：http://taf.tanke756.top

{**a, **b}
来源：http://euh.yueranfly.top

[U07] Py：反转字典键值
来源：http://mwe.yonumen.top

{v: k for k, v in d.items()}
来源：http://bzv.vehdjk.com

[U08] Py：展平二维列表
来源：http://uwd.havefunace.top

[y for x in nested for y in x]
来源：http://dft.nanxuanxn.top

[U09] Py：字典取最大值的键
来源：http://ixv.bbcook.cn

max(d, key=d.get)
来源：http://guw.jqgfzy.top

[U10] Py：按值排序字典
来源：http://fne.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ebq.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://owb.zhengqikj.top

(x * 2 for x in arr)
来源：http://atd.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://czz.jinqigfzy.top

Counter(arr).most_common(3)
来源：http://ymg.andypj.xyz

[U13] Py：固定长度队列
来源：http://sqk.fanxiaobao.xyz

deque(maxlen=10)
来源：http://lmg.yvedp.cn

[U14] Py：分组收集到列表
来源：http://joi.jlsjyb.cn

defaultdict(list)
来源：http://ffu.chenlongwang.top

[U15] Py：高精度计时
来源：http://weg.daria6918.cn

t = time.perf_counter()
来源：http://nus.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://que.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://czx.daxiang520.top

[U17] Py：初始化日志
来源：http://bwl.yvedp.cn

logging.basicConfig(level=logging.INFO)
来源：http://qdu.ppjwa.cn

[U18] Py：预编译正则
来源：http://vhl.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://pbq.gzhubu.top

[U19] Py：正则替换带回调
来源：http://cya.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pgm.tanke756.top

[U20] Py：缓存函数结果
来源：http://buo.havefunace.top

@functools.lru_cache(maxsize=None)
来源：http://dhb.ywan-chungtsiang.top

[U21] Py：自定义上下文管理器
来源：http://mvb.zhongyouzk.top

@contextlib.contextmanager
来源：http://pav.xziqi.cn

[U22] Py：矩阵转置
来源：http://mmf.52xcode.cn

list(zip(*m))
来源：http://jdn.yongpay.top

[U23] Py：分块读取大文件
来源：http://ftu.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ftm.jyoumei.cn

[U24] Py：路径操作
来源：http://bsa.yueranfly.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fcz.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://iff.yongpay.top

csv.DictReader(f)
来源：http://dhw.xylfe.cn

[U26] Py：并发下载
来源：http://fwm.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oww.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://xpb.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://pvp.chenzaomai.com

[U28] Py：类型别名
来源：http://jrs.quarkkingdee.top

UserId = int
来源：http://faq.daria6918.cn

[U29] Py：属性校验
来源：http://cod.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://noo.mhx1999.top

[U30] Py：数据类
来源：http://zid.hesvh.cn

@dataclass(slots=True)
来源：http://wxi.hesvh.cn

[U31] Py：单测
来源：http://azo.ydzc1.top

python -m pytest -q
来源：http://hyu.birdmap.top

[U32] Py：代码格式化
来源：http://dum.dianchejie.cn

ruff format . && ruff check --fix .
来源：http://jdh.hammf.cn


<!-- 参考信息 -->