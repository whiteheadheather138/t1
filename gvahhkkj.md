代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://mld.aizwys.cn

[S02] C：变量与格式化输出
来源：http://ahw.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://mxt.shangyingyoupin.top

[S03] C：读入整数
来源：http://jsd.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://rbv.hcnkem.com

[S04] C：字符串复制
来源：http://zal.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://awx.sufxvd.cn

[S05] C：字符串长度
来源：http://tyq.zhixingplan.top

strlen(s)
来源：http://pva.zhongyouzk.top

[S06] C：字符串比较
来源：http://ylz.sufxvd.cn

strcmp(a, b) == 0
来源：http://gna.jiagoushi.top

[S07] C：数组遍历求和
来源：http://cul.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jzk.shzxlz.cn

[S08] C：动态内存分配与释放
来源：http://jcf.ppjwa.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://akr.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://whg.sysykeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ybp.gaohongyu789.top

[S10] C：指针与解引用
来源：http://rmf.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://wqv.daxiang520.top

[S11] C：逐行读文件
来源：http://xeu.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://vkv.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bfe.zhiwuduotai.top

fclose(f);
来源：http://lab.sysykeji.top

[S12] C：写文件
来源：http://maj.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mwu.cdnleiting.top

[S13] C：宏定义
来源：http://kib.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nlx.bbcook.cn

[S14] C：枚举
来源：http://ckd.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://jtl.yonumen.top

[S15] C：类型转换
来源：http://aqq.birdmap.top

(double) a / b
来源：http://qlh.mhx1999.top

[S16] C：位操作置位
来源：http://jvr.guannengcc.top

x |= (1 << 3);
来源：http://jxj.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://yqm.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sta.fktsv.cn

[S18] C：命令行参数
来源：http://wis.hammf.cn

int main(int argc, char **argv)
来源：http://ygb.sweek.top

[S19] C：快速排序
来源：http://baa.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://kyi.guannengcc.top

[S20] C：二分查找
来源：http://mki.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nma.9152youxi.cn

[S21] C：字符类别判断
来源：http://eoh.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sbo.quarkkingdee.top

[S22] C：字符串转数字
来源：http://fgy.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://dlz.birdmap.top

[S23] C：随机数
来源：http://yly.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://hue.hnxiangtu.top

[S24] C：获取本地时间
来源：http://jcw.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wsk.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://smt.xuanzx.com

memcpy(dst, src, n);
来源：http://kpb.andypj.xyz

[S26] C：内存清零
来源：http://kil.sysykeji.top

memset(a, 0, sizeof a);
来源：http://otu.hesvh.cn

[S27] C：定义常量
来源：http://xqp.yuxming.cn

const double PI = 3.14159;
来源：http://hzj.zhaomingkeji.xyz

[S28] C：静态变量
来源：http://yyo.ywan-chungtsiang.top

static int counter = 0;
来源：http://mwa.pengpengdd.cyou

[S29] C：变参函数
来源：http://pal.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rjj.aibaodan.cn

[S30] C：头文件保护
来源：http://jfd.daxiang520.top

#ifndef X_H
来源：http://qdk.epnwcf.com

#define X_H
来源：http://yej.gaohongyu789.top

#endif
来源：http://vmu.yj202588.top

[S31] C++：Hello World
来源：http://tre.xuanzx.com

#include <iostream>
来源：http://ymv.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://qbn.zdbjq.cn

[S32] C++：字符串
来源：http://glb.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://btk.yj20258888.top

[S33] C++：vector 增删
来源：http://ive.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yic.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://lng.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://fee.ctjpmb.com

[S35] C++：map
来源：http://brz.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jld.andypj.xyz

[S36] C++：unordered_map
来源：http://xqj.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oox.hongshengwenyu.top

[S37] C++：set
来源：http://inw.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bzt.jqgufenzy.top

[S38] C++：排序
来源：http://kvi.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://kwk.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://ahe.smart0.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lxl.shzxlz.cn

[S40] C++：查找元素
来源：http://dpa.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hzh.xuanzx.com

[S41] C++：类与构造函数
来源：http://tpq.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wws.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://qem.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://jrh.mhx1999.top

[S43] C++：智能指针
来源：http://ybs.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://kcf.gzhubu.top

[S44] C++：引用传参
来源：http://nkf.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://quj.jqgufenzy.top

[S45] C++：lambda
来源：http://rji.nanxinkj.top

auto add = [](int a, int b) { return a + b; };
来源：http://lzy.sjlbkw.cn

[S46] C++：函数模板
来源：http://svh.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wlq.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://mkf.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kjy.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://hja.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://bfc.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://lwt.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://gcl.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vbe.yuxming.cn

[S50] C++：格式化数字
来源：http://rug.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nhz.sufxvd.cn

[S51] C++：显式类型转换
来源：http://ajz.smart0.xyz

static_cast<double>(a) / b
来源：http://qyn.yj202588.top

[S52] C++：const 与 noexcept
来源：http://tbc.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://lry.zhoulong.xyz

[S53] C++：移动语义
来源：http://lpq.hammf.cn

std::vector<int> w = std::move(v);
来源：http://sav.fehbvm.com

[S54] C++：异常处理
来源：http://gba.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zfp.cashguo.top

[S55] C++：结构化绑定
来源：http://qxc.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uhs.zhengqikj.top

[S56] C++：optional
来源：http://yhx.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wvw.ehwqpu.com

[S57] C++：编译期常量
来源：http://hwk.hnxiangtu.top

constexpr int N = 10;
来源：http://qgv.daria6918.cn

[S58] C++：命名空间
来源：http://brx.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://qqk.fengsongda.top

[S59] C++：静态断言
来源：http://sbt.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://our.tarul.cn

[S60] C++：遍历并删除元素
来源：http://qvp.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uij.fktsv.cn

================================================================================
来源：http://lch.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://epf.fzhhl.top

================================================================================
来源：http://hrr.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://skr.shzxlz.cn

println("Hello")
来源：http://xxx.nanxinkj.top

[T02] Kotlin：变量
来源：http://lzv.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wmg.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://joe.zdbjq.cn

"值: $b"
来源：http://lyj.nwbrower.top

[T04] Kotlin：空安全
来源：http://csf.meibo888.top

val n: String? = null;  n?.length
来源：http://gil.yongpay.top

[T05] Kotlin：when 表达式
来源：http://ykz.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gew.yonumen.top

[T06] Kotlin：集合映射
来源：http://svq.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yvq.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://uol.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://iht.jyoumei.cn

[T08] Kotlin：数据类
来源：http://biy.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://vwb.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://les.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://qzz.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://hsu.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ufo.hysaishi.cn

[T11] Kotlin：协程
来源：http://mos.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hdg.havefunace.top

[T12] Kotlin：解构声明
来源：http://kzr.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://ldv.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://sdw.nwbrower.top

val m = mapOf("a" to 1)
来源：http://cfg.jlsjyb.cn

[T14] Kotlin：循环
来源：http://mbb.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://oou.mhx1999.top

[T15] Kotlin：接口
来源：http://wad.wangshuangyany.cn

interface Shape { fun area(): Double }
来源：http://qij.guannengcc.top

[T16] Swift：Hello World
来源：http://qto.guowangkeji.top

print("Hello")
来源：http://cvq.aibaodan.cn

[T17] Swift：变量与常量
来源：http://kvp.yuanzhike.top

var a = 1;  let b = 2
来源：http://uld.fktsv.cn

[T18] Swift：字符串插值
来源：http://sth.daxiang520.top

"值: \(b)"
来源：http://vym.daxiang520.top

[T19] Swift：可选绑定
来源：http://ikk.sufxvd.cn

if let n = opt { print(n) }
来源：http://pnw.yuxming.cn

[T20] Swift：数组操作
来源：http://kev.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://rkq.gaohongyu789.top

[T21] Swift：遍历
来源：http://ijo.sxryk.cn

for x in a { print(x) }
来源：http://qhd.yueranfly.top

[T22] Swift：字典
来源：http://pfm.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://dqb.jianghu66.top

[T23] Swift：函数
来源：http://oeb.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qst.pycfn.com

[T24] Swift：闭包
来源：http://gfa.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://eka.uphjek.com

[T25] Swift：结构体
来源：http://lub.aibaodan.cn

struct P { var x: Int }
来源：http://cgt.daria6918.cn

[T26] Swift：类与重写
来源：http://qpx.tian-w.cn

class A: Base { override func f() {} }
来源：http://hij.hnxiangtu.top

[T27] Swift：错误处理
来源：http://cet.hfpthk.cn

do { try f() } catch { print(error) }
来源：http://xbk.yuxming.cn

[T28] Swift：枚举
来源：http://pyn.zhixingplan.top

enum Color { case red, green }
来源：http://crh.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://zkz.jiagoushi.top

guard let x = opt else { return }
来源：http://suv.yanxiufei.cn

[T30] Swift：协议
来源：http://slc.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://qqc.jlsjyb.cn

[T31] Lua：Hello World
来源：http://twm.hfpthk.cn

print("Hello")
来源：http://rlk.aizwys.cn

[T32] Lua：局部变量
来源：http://jwk.hcnkem.com

local a = 1
来源：http://jju.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://ewx.nwbrower.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eeg.ydzc1.top

[T34] Lua：遍历表
来源：http://fwt.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://geh.nwbrower.top

[T35] Lua：字典表
来源：http://wde.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://wxw.zhengqikj.top

[T36] Lua：函数
来源：http://hga.xylfe.cn

function add(a, b) return a + b end
来源：http://kcy.zhijiandao.cn

[T37] Lua：字符串拼接
来源：http://rip.zhixingplan.top

"a" .. "b"
来源：http://ajj.yueranfly.top

[T38] Lua：条件
来源：http://efr.aizwys.cn

if x > 0 then print("正") end
来源：http://pfl.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://kgv.guowangkeji.top

string.find(s, "%d+")
来源：http://dkl.shzxlz.cn

[T40] Lua：元表
来源：http://phg.daxiang520.top

setmetatable({}, { __index = base })
来源：http://vvj.zhongyouzk.top

[T41] Perl：Hello World
来源：http://ytv.yj20258888.top

print "Hello\n";
来源：http://bxu.yfazqb.com

[T42] Perl：变量类型
来源：http://cbi.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gjm.xziqi.cn

[T43] Perl：字符串插值
来源：http://prr.vqdsnc.cn

"值: $a"
来源：http://sir.ydzc1.top

[T44] Perl：条件
来源：http://qaz.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://rmm.ctjpmb.com

[T45] Perl：数组遍历
来源：http://tdl.yj202588.top

for my $x (@arr) { print $x; }
来源：http://shr.52xcode.cn

[T46] Perl：哈希操作
来源：http://lsw.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ycb.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://mtu.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://shg.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://uxq.svipenyu.cn

$s =~ s/old/new/g;
来源：http://ifa.gaohongyu789.top

[T49] Perl：函数
来源：http://tla.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ppb.chenjidiqi.icu

[T50] Perl：逐行读文件
来源：http://pdq.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tvz.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://prp.cucudq.cn

[T51] Scala：Hello World
来源：http://tdg.gogol.net.cn

println("Hello")
来源：http://ihb.chenlongwang.top

[T52] Scala：变量
来源：http://htc.cheryme.top

val a = 1;  var b = 2
来源：http://rbi.haohaochexian.top

[T53] Scala：字符串插值
来源：http://ehm.yueranfly.top

s"值: $b"
来源：http://qvd.epnwcf.com

[T54] Scala：集合映射
来源：http://fwu.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://pfh.aibaodan.cn

[T55] Scala：集合过滤
来源：http://ail.sjlbkw.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iqa.dianchejie.cn

[T56] Scala：样例类
来源：http://dpw.vehdjk.com

case class User(name: String, age: Int)
来源：http://hdo.gotoacloud.top

[T57] Scala：模式匹配
来源：http://pnx.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ays.gogol.net.cn

[T58] Scala：函数定义
来源：http://tyo.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://gyb.tianlin.xyz

[T59] Scala：循环
来源：http://lif.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://ccw.zhoulong.xyz

[T60] Scala：折叠
来源：http://dta.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://byi.vqdsnc.cn

================================================================================
来源：http://eny.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cby.ehwqpu.com

================================================================================
来源：http://cxb.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://sqe.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://sol.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://lkx.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iyj.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://ozi.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wjl.hfpthk.cn

[U04] Py：变量调试打印
来源：http://blw.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lpy.tanke756.top

[U05] Py：列表去重且保序
来源：http://wvb.guannengcc.top

list(dict.fromkeys(arr))
来源：http://hun.gotoacloud.top

[U06] Py：合并两个字典
来源：http://bjd.xingfuxueyuan.xyz

{**a, **b}
来源：http://edp.hammf.cn

[U07] Py：反转字典键值
来源：http://vbo.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://qur.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://zqc.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://zze.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://krn.jyoumei.cn

max(d, key=d.get)
来源：http://ien.fengsongda.top

[U10] Py：按值排序字典
来源：http://tfk.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tjx.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://xbu.guowangkeji.top

(x * 2 for x in arr)
来源：http://lju.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://dbz.zdbjq.cn

Counter(arr).most_common(3)
来源：http://inw.sxryk.cn

[U13] Py：固定长度队列
来源：http://oew.zhengqikj.top

deque(maxlen=10)
来源：http://lfc.yj202588.top

[U14] Py：分组收集到列表
来源：http://vax.hfpthk.cn

defaultdict(list)
来源：http://kxb.quarkkingdee.top

[U15] Py：高精度计时
来源：http://jie.hfpthk.cn

t = time.perf_counter()
来源：http://kfh.andypj.xyz

[U16] Py：命令行参数解析
来源：http://bvs.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sji.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://cbw.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://bsi.ybcxt.top

[U18] Py：预编译正则
来源：http://mxm.yonumen.top

pat = re.compile(r"\d+")
来源：http://ayp.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://hvd.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hpj.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://bqs.wangshuangyany.cn

@functools.lru_cache(maxsize=None)
来源：http://tcj.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://pqb.hfpthk.cn

@contextlib.contextmanager
来源：http://xsh.yj20258.top

[U22] Py：矩阵转置
来源：http://qsd.vqdsnc.cn

list(zip(*m))
来源：http://ann.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://rsj.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wyp.yuxming.cn

[U24] Py：路径操作
来源：http://pxm.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ilo.quarkkingdee.top


<!-- 参考信息 -->