代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://uht.redwolf501.top

[S02] C：变量与格式化输出
来源：http://lrv.hysaishi.cn

int a = 10; printf("%d\n", a);
来源：http://cfc.zhengqikj.top

[S03] C：读入整数
来源：http://gew.9152youxi.cn

int x; scanf("%d", &x);
来源：http://cxs.daxiang520.top

[S04] C：字符串复制
来源：http://sbp.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://dev.daxiang520.top

[S05] C：字符串长度
来源：http://tbk.fengsongda.top

strlen(s)
来源：http://nwb.9152youxi.cn

[S06] C：字符串比较
来源：http://tja.svipenyu.cn

strcmp(a, b) == 0
来源：http://ucz.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://plg.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xuu.yonumen.top

[S08] C：动态内存分配与释放
来源：http://jmq.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qjc.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://laa.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dhi.shzxlz.cn

[S10] C：指针与解引用
来源：http://irg.havefunace.top

int *p = &a;  *p = 5;
来源：http://kfz.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://gvv.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://rho.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ayf.ybcxt.top

fclose(f);
来源：http://dpp.gzhubu.top

[S12] C：写文件
来源：http://crm.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dwb.cqqwz.cn

[S13] C：宏定义
来源：http://ixn.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tqc.ivvv.top

[S14] C：枚举
来源：http://woi.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://rnb.zdbjq.cn

[S15] C：类型转换
来源：http://ofx.cheryme.top

(double) a / b
来源：http://xhm.xylfe.cn

[S16] C：位操作置位
来源：http://xxg.yvedp.cn

x |= (1 << 3);
来源：http://ymh.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://ttn.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lls.chenjidiqi.icu

[S18] C：命令行参数
来源：http://ejj.smart0.xyz

int main(int argc, char **argv)
来源：http://hyc.daxiang520.top

[S19] C：快速排序
来源：http://baq.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://eqr.hywenlv.cn

[S20] C：二分查找
来源：http://mgx.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lqv.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://rel.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://alj.birdmap.top

[S22] C：字符串转数字
来源：http://ieq.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://dbv.meibo888.top

[S23] C：随机数
来源：http://ymx.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dui.ydzc1.top

[S24] C：获取本地时间
来源：http://lzh.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wwb.jiagoushi.top

[S25] C：内存拷贝
来源：http://uux.iojbl.cn

memcpy(dst, src, n);
来源：http://nul.pycfn.com

[S26] C：内存清零
来源：http://pfw.nwbrower.top

memset(a, 0, sizeof a);
来源：http://nls.chenzaomai.com

[S27] C：定义常量
来源：http://daw.meibo888.top

const double PI = 3.14159;
来源：http://kgr.guannengcc.top

[S28] C：静态变量
来源：http://eoc.xuanzx.com

static int counter = 0;
来源：http://ywk.hysaishi.cn

[S29] C：变参函数
来源：http://xzb.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://slr.nanxinkj.top

[S30] C：头文件保护
来源：http://fqh.yj20258888.top

#ifndef X_H
来源：http://eve.shanyushiyangkeji.top

#define X_H
来源：http://ghd.xziqi.cn

#endif
来源：http://wql.aibaodan.cn

[S31] C++：Hello World
来源：http://wiq.hongshengwenyu.top

#include <iostream>
来源：http://pxd.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://xqc.iojbl.cn

[S32] C++：字符串
来源：http://ngd.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://agt.gaohongyu789.top

[S33] C++：vector 增删
来源：http://fer.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zlv.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://xol.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://sfy.iojbl.cn

[S35] C++：map
来源：http://mbo.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sfr.smart0.xyz

[S36] C++：unordered_map
来源：http://ipj.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lfi.hnqzz.top

[S37] C++：set
来源：http://pyh.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gsv.ppjwa.cn

[S38] C++：排序
来源：http://vtj.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://msm.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://bpg.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tow.yongpay.top

[S40] C++：查找元素
来源：http://yye.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://opv.xuanzx.com

[S41] C++：类与构造函数
来源：http://lzf.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ulf.316326.xyz

[S42] C++：继承与虚函数
来源：http://oxh.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://ruf.ppjwa.cn

[S43] C++：智能指针
来源：http://jpf.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://wkr.havefunace.top

[S44] C++：引用传参
来源：http://bjr.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://wwk.shuidangran.top

[S45] C++：lambda
来源：http://lsy.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vgt.vqdsnc.cn

[S46] C++：函数模板
来源：http://ltn.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jgd.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://het.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oge.cqqwz.cn

[S48] C++：逐行读文件
来源：http://shy.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://zam.fengsongda.top

while (std::getline(in, line)) { }
来源：http://aem.jinqigfzy.top

[S49] C++：写文件
来源：http://cdn.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mxx.jianghu66.top

[S50] C++：格式化数字
来源：http://bch.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uxw.hfpthk.cn

[S51] C++：显式类型转换
来源：http://xos.jqgfzy.top

static_cast<double>(a) / b
来源：http://acy.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://xiz.guannengcc.top

int size() const noexcept { return n_; }
来源：http://lln.vehdjk.com

[S53] C++：移动语义
来源：http://iht.cheryme.top

std::vector<int> w = std::move(v);
来源：http://mag.chenzaomai.com

[S54] C++：异常处理
来源：http://eud.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xys.tarul.cn

[S55] C++：结构化绑定
来源：http://yty.52xcode.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hma.ydzc1.top

[S56] C++：optional
来源：http://svw.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dks.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://mcw.yj202588.top

constexpr int N = 10;
来源：http://erx.hongshengwenyu.top

[S58] C++：命名空间
来源：http://lms.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://hpz.52xcode.cn

[S59] C++：静态断言
来源：http://ztu.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ons.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://rab.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://viz.ywan-chungtsiang.top

================================================================================
来源：http://cnx.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ivc.jyoumei.cn

================================================================================
来源：http://rjk.xinyue.icu

[T01] Kotlin：Hello World
来源：http://xun.yuanzhike.top

println("Hello")
来源：http://pxk.guowangkeji.top

[T02] Kotlin：变量
来源：http://lhu.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kag.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://pwf.shanyushiyangtech.top

"值: $b"
来源：http://krp.nwbrower.top

[T04] Kotlin：空安全
来源：http://cdw.yj20258888.top

val n: String? = null;  n?.length
来源：http://ypo.yj202588.top

[T05] Kotlin：when 表达式
来源：http://jmz.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xpo.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://jnh.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gpm.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://bho.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://jwv.316326.xyz

[T08] Kotlin：数据类
来源：http://iod.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://jsm.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://fyi.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://lce.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://jza.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yro.sufxvd.cn

[T11] Kotlin：协程
来源：http://ghc.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fvw.meibo888.top

[T12] Kotlin：解构声明
来源：http://jhs.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://lux.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://iiz.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://uiv.xziqi.cn

[T14] Kotlin：循环
来源：http://hbj.andypj.xyz

for (i in 1..10) println(i)
来源：http://fbg.bbcook.cn

[T15] Kotlin：接口
来源：http://xwm.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://zzp.gaohongyu789.top

[T16] Swift：Hello World
来源：http://nxc.xingfuxueyuan.xyz

print("Hello")
来源：http://odx.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://csg.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://fvo.hfpthk.cn

[T18] Swift：字符串插值
来源：http://cji.tarul.cn

"值: \(b)"
来源：http://jyj.ivvv.top

[T19] Swift：可选绑定
来源：http://ual.tarul.cn

if let n = opt { print(n) }
来源：http://zfp.jinqigufen.top

[T20] Swift：数组操作
来源：http://uwt.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://qlm.feifeiyinyue.top

[T21] Swift：遍历
来源：http://hjf.wangdashe.top

for x in a { print(x) }
来源：http://eah.meibo888.top

[T22] Swift：字典
来源：http://gws.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xqi.vehdjk.com

[T23] Swift：函数
来源：http://jmi.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rbj.redwolf501.top

[T24] Swift：闭包
来源：http://ymv.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://fnm.yonumen.top

[T25] Swift：结构体
来源：http://bbg.tian-w.cn

struct P { var x: Int }
来源：http://fqu.nanxuanxn.top

[T26] Swift：类与重写
来源：http://pyj.jiagoushi.top

class A: Base { override func f() {} }
来源：http://tub.c1oappe.top

[T27] Swift：错误处理
来源：http://hkh.tianlin.xyz

do { try f() } catch { print(error) }
来源：http://vpt.tarul.cn

[T28] Swift：枚举
来源：http://aah.gogol.net.cn

enum Color { case red, green }
来源：http://ufd.andypj.xyz

[T29] Swift：guard 提前返回
来源：http://tee.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://ypm.zhoulong.xyz

[T30] Swift：协议
来源：http://nma.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://kna.jqgfzy.top

[T31] Lua：Hello World
来源：http://nzs.sweek.top

print("Hello")
来源：http://ekh.ydzc1.top

[T32] Lua：局部变量
来源：http://vlu.tian-w.cn

local a = 1
来源：http://hyf.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://knu.ydzc1.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kmd.yj20258888.top

[T34] Lua：遍历表
来源：http://tht.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://bet.yuxming.cn

[T35] Lua：字典表
来源：http://crr.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://tdd.kuanghao11.cn

[T36] Lua：函数
来源：http://heu.yongpay.top

function add(a, b) return a + b end
来源：http://bfr.andypj.xyz

[T37] Lua：字符串拼接
来源：http://ikk.xylfe.cn

"a" .. "b"
来源：http://yqo.aibaodan.cn

[T38] Lua：条件
来源：http://fwu.hesvh.cn

if x > 0 then print("正") end
来源：http://tip.aibaodan.cn

[T39] Lua：模式匹配
来源：http://eas.jinqigufen.top

string.find(s, "%d+")
来源：http://nqm.pengpengdd.cyou

[T40] Lua：元表
来源：http://lpg.9152youxi.cn

setmetatable({}, { __index = base })
来源：http://ofg.cdnleiting.top

[T41] Perl：Hello World
来源：http://xxz.nanxuanxn.top

print "Hello\n";
来源：http://xwq.9152youxi.cn

[T42] Perl：变量类型
来源：http://rdi.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dir.yj20258888.top

[T43] Perl：字符串插值
来源：http://jjh.yvedp.cn

"值: $a"
来源：http://fzr.ivvv.top

[T44] Perl：条件
来源：http://vzz.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://mjq.daxiang520.top

[T45] Perl：数组遍历
来源：http://fkf.fengsongda.top

for my $x (@arr) { print $x; }
来源：http://lkp.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://zee.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cjk.yvedp.cn

[T47] Perl：正则捕获
来源：http://mrc.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hpm.tianlin.xyz

[T48] Perl：正则替换
来源：http://rtb.zdbjq.cn

$s =~ s/old/new/g;
来源：http://nya.yangfankeji.com

[T49] Perl：函数
来源：http://osw.daxiang520.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://okh.sweek.top

[T50] Perl：逐行读文件
来源：http://rex.zdqjudy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ank.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://vza.yfazqb.com

[T51] Scala：Hello World
来源：http://ruk.52xcode.cn

println("Hello")
来源：http://yqr.jinghuilouyu.cn

[T52] Scala：变量
来源：http://lnt.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://nny.haohaochexian.top

[T53] Scala：字符串插值
来源：http://wdx.aibaodan.cn

s"值: $b"
来源：http://uwp.zhengqikj.top

[T54] Scala：集合映射
来源：http://qye.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://zjw.chenzaomai.com

[T55] Scala：集合过滤
来源：http://swb.hongshengwenyu.top

List(1, 2, 3).filter(_ > 1)
来源：http://kha.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://ges.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://lio.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://fgk.shanyushiyangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vvz.chenzaomai.com

[T58] Scala：函数定义
来源：http://mny.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://ukz.zhiwuduotai.top

[T59] Scala：循环
来源：http://pkm.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://igf.tanke756.top

[T60] Scala：折叠
来源：http://sdu.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jlb.jyoumei.cn

================================================================================
来源：http://evw.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ujl.shanyushiyangkeji.top

================================================================================
来源：http://jet.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://irq.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://eah.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://zun.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dnh.zhiwuduotai.top

[U03] Py：加载 .env 配置
来源：http://czy.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gcp.316326.xyz

[U04] Py：变量调试打印
来源：http://ycc.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wjp.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://rfb.yonumen.top

list(dict.fromkeys(arr))
来源：http://exo.nwbrower.top

[U06] Py：合并两个字典
来源：http://but.gzhubu.top

{**a, **b}
来源：http://cdm.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://laz.nwbrower.top

{v: k for k, v in d.items()}
来源：http://iie.chenlongwang.top

[U08] Py：展平二维列表
来源：http://blc.yangfankeji.com

[y for x in nested for y in x]
来源：http://vfd.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://zka.meibo888.top

max(d, key=d.get)
来源：http://zvm.smart0.xyz

[U10] Py：按值排序字典
来源：http://aua.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ptg.bbcook.cn

[U11] Py：生成器表达式
来源：http://mjt.hnxiangtu.top

(x * 2 for x in arr)
来源：http://qgp.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://guy.jinqigufen.top

Counter(arr).most_common(3)
来源：http://rii.ivvv.top

[U13] Py：固定长度队列
来源：http://nga.haohaochexian.top

deque(maxlen=10)
来源：http://nrl.52xcode.cn

[U14] Py：分组收集到列表
来源：http://rff.ybcxt.top

defaultdict(list)
来源：http://whh.jqgufenzy.top

[U15] Py：高精度计时
来源：http://srj.zhengqikj.top

t = time.perf_counter()
来源：http://gud.ivvv.top

[U16] Py：命令行参数解析
来源：http://ozx.chenlongwang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://con.jiagoushi.top

[U17] Py：初始化日志
来源：http://qpc.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://qqr.hesvh.cn

[U18] Py：预编译正则
来源：http://apw.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://vrp.c1oappe.top

[U19] Py：正则替换带回调
来源：http://fto.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cdm.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://kyc.zhixingplan.top

@functools.lru_cache(maxsize=None)
来源：http://esm.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://upk.tanke756.top

@contextlib.contextmanager
来源：http://gdf.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://lxs.epnwcf.com

list(zip(*m))
来源：http://rab.xingfuxueyuan.xyz

[U23] Py：分块读取大文件
来源：http://chy.zhaomingkeji.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xob.wangshuangyany.cn

[U24] Py：路径操作
来源：http://swk.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lgo.hcnkem.com


<!-- 参考信息 -->