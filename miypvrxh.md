代发 wailian999

int x; scanf("%d", &x);
来源：http://zhd.zycfv.cn

[S04] C：字符串复制
来源：http://nki.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://bpk.zycfv.cn

[S05] C：字符串长度
来源：http://pqb.jyoumei.cn

strlen(s)
来源：http://fvu.zhongyouzk.top

[S06] C：字符串比较
来源：http://ltr.guannengcc.top

strcmp(a, b) == 0
来源：http://xzl.meibo888.top

[S07] C：数组遍历求和
来源：http://qbe.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://equ.hammf.cn

[S08] C：动态内存分配与释放
来源：http://ism.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uka.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://yst.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wfk.cucudq.cn

[S10] C：指针与解引用
来源：http://aon.guannengcc.top

int *p = &a;  *p = 5;
来源：http://axm.hfpthk.cn

[S11] C：逐行读文件
来源：http://gcd.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://aei.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jvv.sweek.top

fclose(f);
来源：http://kqe.yuanzhike.top

[S12] C：写文件
来源：http://nse.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aqp.hysaishi.cn

[S13] C：宏定义
来源：http://eza.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://snl.fengsongda.top

[S14] C：枚举
来源：http://cbj.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://tqp.shuidangran.top

[S15] C：类型转换
来源：http://khc.nanxinkj.top

(double) a / b
来源：http://mto.zdbjq.cn

[S16] C：位操作置位
来源：http://dtf.cheryme.top

x |= (1 << 3);
来源：http://qrz.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://bwm.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hdl.gaohongyu789.top

[S18] C：命令行参数
来源：http://gkp.ybcxt.top

int main(int argc, char **argv)
来源：http://cto.uphjek.com

[S19] C：快速排序
来源：http://ndn.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://awe.feifeiyinyue.top

[S20] C：二分查找
来源：http://mlp.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gsm.c1oappe.top

[S21] C：字符类别判断
来源：http://fri.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gcd.hesvh.cn

[S22] C：字符串转数字
来源：http://ush.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://tvo.52xcode.cn

[S23] C：随机数
来源：http://ptm.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://sak.svipenyu.cn

[S24] C：获取本地时间
来源：http://avr.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ltp.daxiang520.top

[S25] C：内存拷贝
来源：http://crq.yj202588.top

memcpy(dst, src, n);
来源：http://xrb.xylfe.cn

[S26] C：内存清零
来源：http://jls.gzhubu.top

memset(a, 0, sizeof a);
来源：http://bnz.sufxvd.cn

[S27] C：定义常量
来源：http://tjp.birdmap.top

const double PI = 3.14159;
来源：http://wdj.quarkkingdee.top

[S28] C：静态变量
来源：http://hfv.52xcode.cn

static int counter = 0;
来源：http://sbm.fktsv.cn

[S29] C：变参函数
来源：http://enb.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vnm.dashuyun.cn

[S30] C：头文件保护
来源：http://wvk.hysaishi.cn

#ifndef X_H
来源：http://rgn.cdnleiting.top

#define X_H
来源：http://hyt.nanxinkj.top

#endif
来源：http://tqm.tanke756.top

[S31] C++：Hello World
来源：http://okw.nwbrower.top

#include <iostream>
来源：http://qox.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://fua.mhx1999.top

[S32] C++：字符串
来源：http://dki.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://zve.zhijiandao.cn

[S33] C++：vector 增删
来源：http://gkq.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nze.c1oappe.top

[S34] C++：遍历 vector
来源：http://zqd.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://iij.hnqzz.top

[S35] C++：map
来源：http://fec.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ttk.ctjpmb.com

[S36] C++：unordered_map
来源：http://dhw.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://moy.daxiang520.top

[S37] C++：set
来源：http://hxj.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fyi.tanke756.top

[S38] C++：排序
来源：http://rsp.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://lak.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://gjl.fktsv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rfp.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://jnq.hfpthk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iha.ctjpmb.com

[S41] C++：类与构造函数
来源：http://kxw.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://svj.tianlin.xyz

[S42] C++：继承与虚函数
来源：http://ivh.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://muy.smart0.xyz

[S43] C++：智能指针
来源：http://swy.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://hcm.yj20258888.top

[S44] C++：引用传参
来源：http://khb.redwolf501.top

void inc(int &x) { ++x; }
来源：http://rfh.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://jzx.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://nav.hesvh.cn

[S46] C++：函数模板
来源：http://agp.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qwp.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://toh.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lgg.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://pxm.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://qjj.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://zcl.feifeiyinyue.top

[S49] C++：写文件
来源：http://tjh.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://omt.xziqi.cn

[S50] C++：格式化数字
来源：http://hvu.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qnv.fengsongda.top

[S51] C++：显式类型转换
来源：http://fdl.havefunace.top

static_cast<double>(a) / b
来源：http://yxt.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://rdy.yongpay.top

int size() const noexcept { return n_; }
来源：http://mzx.cucudq.cn

[S53] C++：移动语义
来源：http://xrc.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://gdj.0kj1m.cn

[S54] C++：异常处理
来源：http://rwz.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qnk.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://bxz.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pfe.zhixingplan.top

[S56] C++：optional
来源：http://ftj.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cuj.redwolf501.top

[S57] C++：编译期常量
来源：http://nyy.dianchejie.cn

constexpr int N = 10;
来源：http://uih.pengpengdd.cyou

[S58] C++：命名空间
来源：http://ebo.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://evh.dashuyun.cn

[S59] C++：静态断言
来源：http://shh.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sqw.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://qla.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lbr.yuxming.cn

================================================================================
来源：http://wti.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ukt.fanxiaobao.xyz

================================================================================
来源：http://tfh.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://txu.svipenyu.cn

println("Hello")
来源：http://fzj.yj20258.top

[T02] Kotlin：变量
来源：http://tye.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wng.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://hkw.aizwys.cn

"值: $b"
来源：http://gnd.fengsongda.top

[T04] Kotlin：空安全
来源：http://uze.ehwqpu.com

val n: String? = null;  n?.length
来源：http://rhe.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://tzu.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mpl.guannengcc.top

[T06] Kotlin：集合映射
来源：http://uiq.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://asi.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://anv.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ugj.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://api.tarul.cn

data class User(val name: String, val age: Int)
来源：http://xgh.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://vso.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://lln.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://lpb.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://byk.daria6918.cn

[T11] Kotlin：协程
来源：http://blw.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xkr.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://efk.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://awh.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://uzq.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://mav.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://oxt.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://owl.ivvv.top

[T15] Kotlin：接口
来源：http://wtn.bjfxy.top

interface Shape { fun area(): Double }
来源：http://avj.aibaodan.cn

[T16] Swift：Hello World
来源：http://fqv.fktsv.cn

print("Hello")
来源：http://pgf.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://pjg.yuxming.cn

var a = 1;  let b = 2
来源：http://ziq.52xcode.cn

[T18] Swift：字符串插值
来源：http://ygh.sjlbkw.cn

"值: \(b)"
来源：http://ojf.hnqzz.top

[T19] Swift：可选绑定
来源：http://yzi.yongpay.top

if let n = opt { print(n) }
来源：http://pmc.jyoumei.cn

[T20] Swift：数组操作
来源：http://kfe.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://ykb.hongshengwenyu.top

[T21] Swift：遍历
来源：http://beo.fktsv.cn

for x in a { print(x) }
来源：http://emz.c1oappe.top

[T22] Swift：字典
来源：http://zod.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://zit.fengsongda.top

[T23] Swift：函数
来源：http://oli.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vdy.jinqigfzy.top

[T24] Swift：闭包
来源：http://lnv.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zmq.zycfv.cn

[T25] Swift：结构体
来源：http://nlg.nanxuanxn.top

struct P { var x: Int }
来源：http://ozs.zhiwuduotai.top

[T26] Swift：类与重写
来源：http://xti.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://vva.daria6918.cn

[T27] Swift：错误处理
来源：http://tac.yj202588.top

do { try f() } catch { print(error) }
来源：http://lno.0kj1m.cn

[T28] Swift：枚举
来源：http://uox.yj202588.top

enum Color { case red, green }
来源：http://ksn.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://gzs.sysykeji.top

guard let x = opt else { return }
来源：http://dxc.iojbl.cn

[T30] Swift：协议
来源：http://eod.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://nrv.bjfxy.top

[T31] Lua：Hello World
来源：http://ymc.gzhubu.top

print("Hello")
来源：http://ulw.yfazqb.com

[T32] Lua：局部变量
来源：http://zye.yueranfly.top

local a = 1
来源：http://tfk.hfpthk.cn

[T33] Lua：表（数组）
来源：http://kad.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jox.yueranfly.top

[T34] Lua：遍历表
来源：http://kxt.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://fgi.52xcode.cn

[T35] Lua：字典表
来源：http://cqj.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://dki.zhiwuduotai.top

[T36] Lua：函数
来源：http://yfv.jinyuanbaomall.cn

function add(a, b) return a + b end
来源：http://nlq.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://waf.jqgufenzy.top

"a" .. "b"
来源：http://cqj.zycfv.cn

[T38] Lua：条件
来源：http://zti.fktsv.cn

if x > 0 then print("正") end
来源：http://hhi.chenzaomai.com

[T39] Lua：模式匹配
来源：http://zht.zhoulong.xyz

string.find(s, "%d+")
来源：http://gak.snrcjt.cn

[T40] Lua：元表
来源：http://tgz.ydzc1.top

setmetatable({}, { __index = base })
来源：http://ydp.quarkkingdee.top

[T41] Perl：Hello World
来源：http://evc.zdbjq.cn

print "Hello\n";
来源：http://ban.jyoumei.cn

[T42] Perl：变量类型
来源：http://hhk.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uzx.nanxuanxn.top

[T43] Perl：字符串插值
来源：http://est.ydzc1.top

"值: $a"
来源：http://owj.fehbvm.com

[T44] Perl：条件
来源：http://uls.0kj1m.cn

if ($a > 0) { print "正"; }
来源：http://vhi.mhx1999.top

[T45] Perl：数组遍历
来源：http://kax.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://adf.tian-w.cn

[T46] Perl：哈希操作
来源：http://yok.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pha.fzhhl.top

[T47] Perl：正则捕获
来源：http://pll.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://gqd.guannengcc.top

[T48] Perl：正则替换
来源：http://axy.yueranfly.top

$s =~ s/old/new/g;
来源：http://mdl.yongpay.top

[T49] Perl：函数
来源：http://quj.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cvk.zhiwuduotai.top

[T50] Perl：逐行读文件
来源：http://pey.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://izu.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://frk.fktsv.cn

[T51] Scala：Hello World
来源：http://gjh.haohaochexian.top

println("Hello")
来源：http://skq.jinqigfzy.top

[T52] Scala：变量
来源：http://loz.xziqi.cn

val a = 1;  var b = 2
来源：http://brq.zhengqikj.top

[T53] Scala：字符串插值
来源：http://rmu.hammf.cn

s"值: $b"
来源：http://gvp.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://kap.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://xmi.mhx1999.top

[T55] Scala：集合过滤
来源：http://ley.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://myj.yj20258.top

[T56] Scala：样例类
来源：http://iiy.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://vly.shuidangran.top

[T57] Scala：模式匹配
来源：http://dbd.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hca.bjfxy.top

[T58] Scala：函数定义
来源：http://bax.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gxd.hongshengwenyu.top

[T59] Scala：循环
来源：http://nqg.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://qwd.yuanzhike.top

[T60] Scala：折叠
来源：http://bkt.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gnp.zdqjudy.top

================================================================================
来源：http://beb.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hbp.xuetiantiany.cn

================================================================================
来源：http://gsv.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://ejk.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pdu.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://rxq.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rvq.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://ehu.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fai.iojbl.cn

[U04] Py：变量调试打印
来源：http://tmj.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dyl.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://plx.xuanzx.com

list(dict.fromkeys(arr))
来源：http://rrp.hywenlv.cn

[U06] Py：合并两个字典
来源：http://pip.ydjk.org.cn

{**a, **b}
来源：http://ilj.daxiang520.top

[U07] Py：反转字典键值
来源：http://zqd.fehbvm.com

{v: k for k, v in d.items()}
来源：http://csv.zhijiandao.cn

[U08] Py：展平二维列表
来源：http://ude.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://aen.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://wsf.ybcxt.top

max(d, key=d.get)
来源：http://seu.gogol.net.cn

[U10] Py：按值排序字典
来源：http://syx.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jki.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://fvh.xziqi.cn

(x * 2 for x in arr)
来源：http://rxi.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mzu.yfazqb.com

Counter(arr).most_common(3)
来源：http://pec.hesvh.cn

[U13] Py：固定长度队列
来源：http://jli.gotoacloud.top

deque(maxlen=10)
来源：http://sxz.tanke756.top

[U14] Py：分组收集到列表
来源：http://asa.zhongyouzk.top

defaultdict(list)
来源：http://twu.bbcook.cn

[U15] Py：高精度计时
来源：http://kqk.hnqzz.top

t = time.perf_counter()
来源：http://luh.andypj.xyz

[U16] Py：命令行参数解析
来源：http://zbm.iojbl.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rbb.zhongyouzk.top

[U17] Py：初始化日志
来源：http://dhl.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://tie.zhoulong.xyz

[U18] Py：预编译正则
来源：http://cyj.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://sfx.birdmap.top

[U19] Py：正则替换带回调
来源：http://xgm.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://amd.nwbrower.top

[U20] Py：缓存函数结果
来源：http://xtg.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://qys.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://orn.gzhubu.top

@contextlib.contextmanager
来源：http://dcy.yj20258888.top

[U22] Py：矩阵转置
来源：http://wqu.sjlbkw.cn

list(zip(*m))
来源：http://nra.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://dol.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://igh.yj20258.top

[U24] Py：路径操作
来源：http://ysm.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rjp.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://wjn.yueranfly.top

csv.DictReader(f)
来源：http://kir.hnxiangtu.top

[U26] Py：并发下载
来源：http://xko.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://igu.tian-w.cn


<!-- 参考信息 -->