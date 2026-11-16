代发 wailian999

strlen(s)
来源：http://nbe.shuidangran.top

[S06] C：字符串比较
来源：http://sia.nanxinkj.top

strcmp(a, b) == 0
来源：http://bnk.ppjwa.cn

[S07] C：数组遍历求和
来源：http://abx.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wui.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://jww.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bof.havefunace.top

[S09] C：结构体定义与初始化
来源：http://ymh.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rvo.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://ndz.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://czf.jinqigufen.top

[S11] C：逐行读文件
来源：http://xgc.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://pxc.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://onk.yonumen.top

fclose(f);
来源：http://sdw.xinyue.icu

[S12] C：写文件
来源：http://iit.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rnx.52xcode.cn

[S13] C：宏定义
来源：http://kto.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vqm.daxiang520.top

[S14] C：枚举
来源：http://spt.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://vcb.iojbl.cn

[S15] C：类型转换
来源：http://tmp.nwbrower.top

(double) a / b
来源：http://xva.dashuyun.cn

[S16] C：位操作置位
来源：http://vto.zdbjq.cn

x |= (1 << 3);
来源：http://gmn.gzhubu.top

[S17] C：安全拼接字符串
来源：http://nsn.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ffs.pycfn.com

[S18] C：命令行参数
来源：http://but.meibo888.top

int main(int argc, char **argv)
来源：http://qwi.ctjpmb.com

[S19] C：快速排序
来源：http://epu.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ibz.nanxuanxn.top

[S20] C：二分查找
来源：http://kff.xylfe.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sng.zycfv.cn

[S21] C：字符类别判断
来源：http://kay.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aox.sxryk.cn

[S22] C：字符串转数字
来源：http://jya.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qsf.ctjpmb.com

[S23] C：随机数
来源：http://xze.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cwn.ppjwa.cn

[S24] C：获取本地时间
来源：http://thd.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kia.yanxiufei.cn

[S25] C：内存拷贝
来源：http://ktw.nanxuanxn.top

memcpy(dst, src, n);
来源：http://jkh.meibo888.top

[S26] C：内存清零
来源：http://pmk.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://bhy.0kj1m.cn

[S27] C：定义常量
来源：http://tgw.uphjek.com

const double PI = 3.14159;
来源：http://tjs.jqgufenzy.top

[S28] C：静态变量
来源：http://wtx.xingfuxueyuan.xyz

static int counter = 0;
来源：http://nzd.316326.xyz

[S29] C：变参函数
来源：http://tos.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jhl.yongpay.top

[S30] C：头文件保护
来源：http://cgd.zhongyouzk.top

#ifndef X_H
来源：http://rau.hywenlv.cn

#define X_H
来源：http://kgm.tian-w.cn

#endif
来源：http://akq.feifeiyinyue.top

[S31] C++：Hello World
来源：http://fvk.snrcjt.cn

#include <iostream>
来源：http://inm.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://bkn.9152youxi.cn

[S32] C++：字符串
来源：http://jxg.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://dsy.yj202588.top

[S33] C++：vector 增删
来源：http://tcj.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dfe.yj20258.top

[S34] C++：遍历 vector
来源：http://kgi.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://zev.aibaodan.cn

[S35] C++：map
来源：http://vqk.daria6918.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vjc.ppjwa.cn

[S36] C++：unordered_map
来源：http://bkq.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xdt.aibaodan.cn

[S37] C++：set
来源：http://pxc.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uqu.chenjidiqi.icu

[S38] C++：排序
来源：http://aqt.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://wzk.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://fbd.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kux.aibaodan.cn

[S40] C++：查找元素
来源：http://dau.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kjo.ctjpmb.com

[S41] C++：类与构造函数
来源：http://ikk.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zhk.fehbvm.com

[S42] C++：继承与虚函数
来源：http://vgk.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://fjo.jianghu66.top

[S43] C++：智能指针
来源：http://pxa.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://rcu.yfazqb.com

[S44] C++：引用传参
来源：http://rff.yuxming.cn

void inc(int &x) { ++x; }
来源：http://zcu.yj20258.top

[S45] C++：lambda
来源：http://rvu.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://unw.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://xhd.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sir.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://bzz.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://btt.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://ktv.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://chu.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://jys.zhoulong.xyz

[S49] C++：写文件
来源：http://jfq.iojbl.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fft.aizwys.cn

[S50] C++：格式化数字
来源：http://gob.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cag.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://obd.pycfn.com

static_cast<double>(a) / b
来源：http://pnm.tanke756.top

[S52] C++：const 与 noexcept
来源：http://pla.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://nvk.fehbvm.com

[S53] C++：移动语义
来源：http://gmx.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://yvh.guowangkeji.top

[S54] C++：异常处理
来源：http://jmb.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sxk.wangdashe.top

[S55] C++：结构化绑定
来源：http://xvd.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vmd.yuxming.cn

[S56] C++：optional
来源：http://yez.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://crt.shanyushiyangtech.top

[S57] C++：编译期常量
来源：http://djy.cdnleiting.top

constexpr int N = 10;
来源：http://aul.mhx1999.top

[S58] C++：命名空间
来源：http://khx.jinyuanbaomall.cn

namespace ns { int f() { return 1; } }
来源：http://qfz.gotoacloud.top

[S59] C++：静态断言
来源：http://gjg.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aiw.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://pls.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tln.iojbl.cn

================================================================================
来源：http://pko.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mej.nanxinkj.top

================================================================================
来源：http://blv.epnwcf.com

[T01] Kotlin：Hello World
来源：http://iqi.aizwys.cn

println("Hello")
来源：http://qur.zhongyouzk.top

[T02] Kotlin：变量
来源：http://mvx.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://elq.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://sbe.hfpthk.cn

"值: $b"
来源：http://opq.yvedp.cn

[T04] Kotlin：空安全
来源：http://mgr.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://eni.tarul.cn

[T05] Kotlin：when 表达式
来源：http://waj.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://boq.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://esj.svipenyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fir.nanxuanxn.top

[T07] Kotlin：集合过滤
来源：http://yru.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qug.snrcjt.cn

[T08] Kotlin：数据类
来源：http://rqx.sweek.top

data class User(val name: String, val age: Int)
来源：http://tmj.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://bbt.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://dmn.ehwqpu.com

[T10] Kotlin：默认参数
来源：http://dsb.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tit.andypj.xyz

[T11] Kotlin：协程
来源：http://smt.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jzu.meibo888.top

[T12] Kotlin：解构声明
来源：http://mdn.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://wpc.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://ula.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://fvk.nanxinkj.top

[T14] Kotlin：循环
来源：http://wdb.fktsv.cn

for (i in 1..10) println(i)
来源：http://ely.fehbvm.com

[T15] Kotlin：接口
来源：http://tdn.yonumen.top

interface Shape { fun area(): Double }
来源：http://yqm.jinqigufen.top

[T16] Swift：Hello World
来源：http://gut.nwbrower.top

print("Hello")
来源：http://gwq.tian-w.cn

[T17] Swift：变量与常量
来源：http://ktl.cashguo.top

var a = 1;  let b = 2
来源：http://msg.yj20258.top

[T18] Swift：字符串插值
来源：http://jdh.dashuyun.cn

"值: \(b)"
来源：http://yhk.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://qrd.yj20258888.top

if let n = opt { print(n) }
来源：http://sqb.zdqjudy.top

[T20] Swift：数组操作
来源：http://ier.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://cnm.ybcxt.top

[T21] Swift：遍历
来源：http://nrk.yueranfly.top

for x in a { print(x) }
来源：http://pll.52xcode.cn

[T22] Swift：字典
来源：http://cvb.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://vdv.ydzc1.top

[T23] Swift：函数
来源：http://fpt.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jxt.zhiwuduotai.top

[T24] Swift：闭包
来源：http://bup.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mem.sxryk.cn

[T25] Swift：结构体
来源：http://nze.aizwys.cn

struct P { var x: Int }
来源：http://dda.shzxlz.cn

[T26] Swift：类与重写
来源：http://hyu.zdbjq.cn

class A: Base { override func f() {} }
来源：http://xcw.cheryme.top

[T27] Swift：错误处理
来源：http://wti.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://vxc.chenlongwang.top

[T28] Swift：枚举
来源：http://sfx.cdnleiting.top

enum Color { case red, green }
来源：http://fds.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://eto.shuidangran.top

guard let x = opt else { return }
来源：http://gtm.c1oappe.top

[T30] Swift：协议
来源：http://nsb.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://ohl.uphjek.com

[T31] Lua：Hello World
来源：http://cbm.svipenyu.cn

print("Hello")
来源：http://qzj.snrcjt.cn

[T32] Lua：局部变量
来源：http://buc.jinqigufen.top

local a = 1
来源：http://oxl.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://stn.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://muo.feifeiyinyue.top

[T34] Lua：遍历表
来源：http://wob.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bro.fengsongda.top

[T35] Lua：字典表
来源：http://dna.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://jmi.yueranfly.top

[T36] Lua：函数
来源：http://fju.yj20258888.top

function add(a, b) return a + b end
来源：http://dzv.fehbvm.com

[T37] Lua：字符串拼接
来源：http://rke.wangdashe.top

"a" .. "b"
来源：http://ikj.yonumen.top

[T38] Lua：条件
来源：http://yyn.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://jle.52xcode.cn

[T39] Lua：模式匹配
来源：http://iyg.bjfxy.top

string.find(s, "%d+")
来源：http://vtk.yj20258.top

[T40] Lua：元表
来源：http://unv.daxiang520.top

setmetatable({}, { __index = base })
来源：http://czs.9152youxi.cn

[T41] Perl：Hello World
来源：http://vob.zdbjq.cn

print "Hello\n";
来源：http://mpb.jqgufenzy.top

[T42] Perl：变量类型
来源：http://aos.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://amq.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://dvn.316326.xyz

"值: $a"
来源：http://xmo.xylfe.cn

[T44] Perl：条件
来源：http://fnh.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://wom.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://hxh.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://gpt.zdqjudy.top

[T46] Perl：哈希操作
来源：http://yhn.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://voe.dashuyun.cn

[T47] Perl：正则捕获
来源：http://rfj.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ufc.yangfankeji.com

[T48] Perl：正则替换
来源：http://uge.ppjwa.cn

$s =~ s/old/new/g;
来源：http://sxw.ctjpmb.com

[T49] Perl：函数
来源：http://xmd.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gwl.mhx1999.top

[T50] Perl：逐行读文件
来源：http://hsj.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dws.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://nih.sysykeji.top

[T51] Scala：Hello World
来源：http://urn.sjlbkw.cn

println("Hello")
来源：http://vxs.jinghuilouyu.cn

[T52] Scala：变量
来源：http://idx.mhx1999.top

val a = 1;  var b = 2
来源：http://fmx.xziqi.cn

[T53] Scala：字符串插值
来源：http://vhe.uphjek.com

s"值: $b"
来源：http://uww.xziqi.cn

[T54] Scala：集合映射
来源：http://vop.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://smc.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://iop.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mdk.zhoulong.xyz

[T56] Scala：样例类
来源：http://ybw.hammf.cn

case class User(name: String, age: Int)
来源：http://edp.ctjpmb.com

[T57] Scala：模式匹配
来源：http://eqo.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://snj.xinyue.icu

[T58] Scala：函数定义
来源：http://dpo.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://hol.xuanzx.com

[T59] Scala：循环
来源：http://tds.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://zav.gaohongyu789.top

[T60] Scala：折叠
来源：http://iym.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hbj.hammf.cn

================================================================================
来源：http://ekw.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bcx.yj20258888.top

================================================================================
来源：http://hpx.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://qfu.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gne.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://nix.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nrq.tanke756.top

[U03] Py：加载 .env 配置
来源：http://yyb.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tpl.smart0.xyz

[U04] Py：变量调试打印
来源：http://qao.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mgd.zycfv.cn

[U05] Py：列表去重且保序
来源：http://jim.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://hfg.cdnleiting.top

[U06] Py：合并两个字典
来源：http://iwd.hnqzz.top

{**a, **b}
来源：http://bml.uphjek.com

[U07] Py：反转字典键值
来源：http://ztr.tian-w.cn

{v: k for k, v in d.items()}
来源：http://edh.gogol.net.cn

[U08] Py：展平二维列表
来源：http://fcj.yanxiufei.cn

[y for x in nested for y in x]
来源：http://gpq.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://tsz.bbcook.cn

max(d, key=d.get)
来源：http://qit.guannengcc.top

[U10] Py：按值排序字典
来源：http://ymh.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aro.ehwqpu.com

[U11] Py：生成器表达式
来源：http://hhe.zhongyouzk.top

(x * 2 for x in arr)
来源：http://qud.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mpm.zdbjq.cn

Counter(arr).most_common(3)
来源：http://zmd.yj20258888.top

[U13] Py：固定长度队列
来源：http://daw.daxiang520.top

deque(maxlen=10)
来源：http://bhj.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://ova.sweek.top

defaultdict(list)
来源：http://nib.ydjk.org.cn

[U15] Py：高精度计时
来源：http://mbu.zhengqikj.top

t = time.perf_counter()
来源：http://brx.fehbvm.com

[U16] Py：命令行参数解析
来源：http://xhn.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cqv.tanke756.top

[U17] Py：初始化日志
来源：http://zyc.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://nio.zhengqikj.top

[U18] Py：预编译正则
来源：http://eii.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://myf.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://iqu.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bmq.hnqzz.top

[U20] Py：缓存函数结果
来源：http://mpl.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://ivs.jiagoushi.top

[U21] Py：自定义上下文管理器
来源：http://iad.vqdsnc.cn

@contextlib.contextmanager
来源：http://htq.chenlongwang.top

[U22] Py：矩阵转置
来源：http://hzg.tianlin.xyz

list(zip(*m))
来源：http://rrz.tarul.cn

[U23] Py：分块读取大文件
来源：http://spi.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://whm.jqgfzy.top

[U24] Py：路径操作
来源：http://zpq.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wvb.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://tbx.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://und.fzhhl.top

[U26] Py：并发下载
来源：http://fxk.mhx1999.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rkz.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://qtj.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://wpk.zycfv.cn

[U28] Py：类型别名
来源：http://zqy.zycfv.cn

UserId = int
来源：http://pgo.fehbvm.com


<!-- 参考信息 -->