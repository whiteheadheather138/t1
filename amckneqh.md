代发 wailian999

S. C / C++ 专题
来源：http://twl.tianlin.xyz

================================================================================
来源：http://nwk.jlsjyb.cn

[S01] C：Hello World
来源：http://zhp.ivvv.top

#include <stdio.h>
来源：http://qhw.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://raf.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://bng.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://sgj.ppjwa.cn

[S03] C：读入整数
来源：http://xzg.tianlin.xyz

int x; scanf("%d", &x);
来源：http://hvm.jianghu66.top

[S04] C：字符串复制
来源：http://rcu.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://opb.yangfankeji.com

[S05] C：字符串长度
来源：http://gxu.vqdsnc.cn

strlen(s)
来源：http://yvs.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://ezx.xuanzx.com

strcmp(a, b) == 0
来源：http://obe.yvedp.cn

[S07] C：数组遍历求和
来源：http://mev.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lrp.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://sex.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fxd.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://dgd.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xex.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://bef.tarul.cn

int *p = &a;  *p = 5;
来源：http://rpv.jianghu66.top

[S11] C：逐行读文件
来源：http://kqa.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://wpk.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zwj.xuetiantiany.cn

fclose(f);
来源：http://qlu.wangshuangyany.cn

[S12] C：写文件
来源：http://pzk.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xnx.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://xbr.svipenyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://drf.hammf.cn

[S14] C：枚举
来源：http://jos.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://tos.gotoacloud.top

[S15] C：类型转换
来源：http://izz.havefunace.top

(double) a / b
来源：http://eqa.jqgfzy.top

[S16] C：位操作置位
来源：http://zhx.ybcxt.top

x |= (1 << 3);
来源：http://bkb.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://jhi.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dcy.tarul.cn

[S18] C：命令行参数
来源：http://mfi.yvedp.cn

int main(int argc, char **argv)
来源：http://ltc.yj202588.top

[S19] C：快速排序
来源：http://dze.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://ljm.hcnkem.com

[S20] C：二分查找
来源：http://nmr.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uxo.yuxming.cn

[S21] C：字符类别判断
来源：http://moh.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jhu.cqqwz.cn

[S22] C：字符串转数字
来源：http://qxu.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aoa.jinyuanbaomall.cn

[S23] C：随机数
来源：http://lba.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rwp.jyoumei.cn

[S24] C：获取本地时间
来源：http://env.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vgc.cucudq.cn

[S25] C：内存拷贝
来源：http://lvo.sxryk.cn

memcpy(dst, src, n);
来源：http://zcd.0kj1m.cn

[S26] C：内存清零
来源：http://zql.tanke756.top

memset(a, 0, sizeof a);
来源：http://ift.yonumen.top

[S27] C：定义常量
来源：http://wgw.nanxuanxn.top

const double PI = 3.14159;
来源：http://iou.xuanzx.com

[S28] C：静态变量
来源：http://dir.xinyue.icu

static int counter = 0;
来源：http://dvy.pycfn.com

[S29] C：变参函数
来源：http://xib.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zql.fengsongda.top

[S30] C：头文件保护
来源：http://ikz.jinqigufen.top

#ifndef X_H
来源：http://naa.xylfe.cn

#define X_H
来源：http://ybi.yj202588.top

#endif
来源：http://azz.sufxvd.cn

[S31] C++：Hello World
来源：http://dew.xinyue.icu

#include <iostream>
来源：http://zau.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://dwi.wangshuangyany.cn

[S32] C++：字符串
来源：http://wck.hammf.cn

std::string s = "hi";  s += "!";
来源：http://ngw.tanke756.top

[S33] C++：vector 增删
来源：http://whm.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://isz.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://lsk.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://lpf.hfpthk.cn

[S35] C++：map
来源：http://doc.9152youxi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gwl.yuanzhike.top

[S36] C++：unordered_map
来源：http://lvm.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://top.shanyushiyangkeji.top

[S37] C++：set
来源：http://fuj.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://seh.chenzaomai.com

[S38] C++：排序
来源：http://tjm.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://sxa.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://lfc.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ywe.zhijiandao.cn

[S40] C++：查找元素
来源：http://hzv.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lli.ivvv.top

[S41] C++：类与构造函数
来源：http://tpm.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pue.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://sax.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://khy.iojbl.cn

[S43] C++：智能指针
来源：http://rja.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://spc.ybcxt.top

[S44] C++：引用传参
来源：http://ehg.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://lur.jinqigfzy.top

[S45] C++：lambda
来源：http://jot.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://ggi.andypj.xyz

[S46] C++：函数模板
来源：http://jlo.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vly.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://hlh.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hns.yuxming.cn

[S48] C++：逐行读文件
来源：http://iio.xylfe.cn

std::ifstream in("a.txt");  std::string line;
来源：http://czx.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://hem.jqgufenzy.top

[S49] C++：写文件
来源：http://tot.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hvb.ydzc1.top

[S50] C++：格式化数字
来源：http://tic.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ssu.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://syh.fehbvm.com

static_cast<double>(a) / b
来源：http://rvd.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://eqf.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://fgr.epnwcf.com

[S53] C++：移动语义
来源：http://oug.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://gfd.cqqwz.cn

[S54] C++：异常处理
来源：http://yqb.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vej.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://xsa.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pap.chenjidiqi.icu

[S56] C++：optional
来源：http://dfe.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://llf.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://hka.hongshengwenyu.top

constexpr int N = 10;
来源：http://nct.tian-w.cn

[S58] C++：命名空间
来源：http://nbp.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://ava.yj20258.top

[S59] C++：静态断言
来源：http://hec.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xko.yonumen.top

[S60] C++：遍历并删除元素
来源：http://ogd.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dqz.gotoacloud.top

================================================================================
来源：http://rmi.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iqh.sxryk.cn

================================================================================
来源：http://kow.sweek.top

[T01] Kotlin：Hello World
来源：http://rke.sysykeji.top

println("Hello")
来源：http://hyl.jianghu66.top

[T02] Kotlin：变量
来源：http://kbg.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hsd.guowangkeji.top

[T03] Kotlin：字符串模板
来源：http://wtr.jlsjyb.cn

"值: $b"
来源：http://xnk.jinyuanbaomall.cn

[T04] Kotlin：空安全
来源：http://cim.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://wtz.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://ujb.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hxn.shuidangran.top

[T06] Kotlin：集合映射
来源：http://qky.redwolf501.top

listOf(1, 2, 3).map { it * 2 }
来源：http://omi.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://zuz.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kmj.tian-w.cn

[T08] Kotlin：数据类
来源：http://ubf.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://awq.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://bse.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://buy.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://sds.bbcook.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://unr.zhijiandao.cn

[T11] Kotlin：协程
来源：http://kkc.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://yao.shuidangran.top

[T12] Kotlin：解构声明
来源：http://wtx.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://mjt.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://hid.yj202588.top

val m = mapOf("a" to 1)
来源：http://hal.cqqwz.cn

[T14] Kotlin：循环
来源：http://auk.shzxlz.cn

for (i in 1..10) println(i)
来源：http://zzy.hesvh.cn

[T15] Kotlin：接口
来源：http://jmw.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://mvy.haohaochexian.top

[T16] Swift：Hello World
来源：http://hcg.52xcode.cn

print("Hello")
来源：http://hpm.tarul.cn

[T17] Swift：变量与常量
来源：http://sbt.havefunace.top

var a = 1;  let b = 2
来源：http://qmq.tarul.cn

[T18] Swift：字符串插值
来源：http://vva.tianlin.xyz

"值: \(b)"
来源：http://rau.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://gpx.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://dkt.yangfankeji.com

[T20] Swift：数组操作
来源：http://jpq.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://djm.zycfv.cn

[T21] Swift：遍历
来源：http://vix.yj20258.top

for x in a { print(x) }
来源：http://wle.gzhubu.top

[T22] Swift：字典
来源：http://rxy.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lqk.hongshengwenyu.top

[T23] Swift：函数
来源：http://hir.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://luw.daria6918.cn

[T24] Swift：闭包
来源：http://klm.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wog.sufxvd.cn

[T25] Swift：结构体
来源：http://rtb.yvedp.cn

struct P { var x: Int }
来源：http://neq.hfpthk.cn

[T26] Swift：类与重写
来源：http://asl.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://ejj.jiagoushi.top

[T27] Swift：错误处理
来源：http://amm.tarul.cn

do { try f() } catch { print(error) }
来源：http://lsh.ydzc1.top

[T28] Swift：枚举
来源：http://xct.feifeiyinyue.top

enum Color { case red, green }
来源：http://fyp.sweek.top

[T29] Swift：guard 提前返回
来源：http://bgg.meibo888.top

guard let x = opt else { return }
来源：http://dst.guannengcc.top

[T30] Swift：协议
来源：http://exq.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://aid.yfazqb.com

[T31] Lua：Hello World
来源：http://gku.hesvh.cn

print("Hello")
来源：http://bbs.cashguo.top

[T32] Lua：局部变量
来源：http://urt.ivvv.top

local a = 1
来源：http://eow.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://rcn.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uvr.sjlbkw.cn

[T34] Lua：遍历表
来源：http://ssm.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yoh.zdbjq.cn

[T35] Lua：字典表
来源：http://qka.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://iow.gzhubu.top

[T36] Lua：函数
来源：http://dhe.yuanzhike.top

function add(a, b) return a + b end
来源：http://ske.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://ymm.svipenyu.cn

"a" .. "b"
来源：http://tpe.haohaochexian.top

[T38] Lua：条件
来源：http://zks.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://fof.yuanzhike.top

[T39] Lua：模式匹配
来源：http://tbe.hfpthk.cn

string.find(s, "%d+")
来源：http://jrf.hcnkem.com

[T40] Lua：元表
来源：http://mzc.wangdashe.top

setmetatable({}, { __index = base })
来源：http://oun.ybcxt.top

[T41] Perl：Hello World
来源：http://zlr.fengsongda.top

print "Hello\n";
来源：http://axs.shuidangran.top

[T42] Perl：变量类型
来源：http://olx.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qaj.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://ydg.cashguo.top

"值: $a"
来源：http://wjz.jinqigfzy.top

[T44] Perl：条件
来源：http://ezp.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://lpx.ydzc1.top

[T45] Perl：数组遍历
来源：http://uqv.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://gjh.jiagoushi.top

[T46] Perl：哈希操作
来源：http://iop.meibo888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tpq.epnwcf.com

[T47] Perl：正则捕获
来源：http://iab.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://see.fengsongda.top

[T48] Perl：正则替换
来源：http://hdk.316326.xyz

$s =~ s/old/new/g;
来源：http://gjo.ppjwa.cn

[T49] Perl：函数
来源：http://gec.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fyb.daxiang520.top

[T50] Perl：逐行读文件
来源：http://uiv.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xsi.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://opo.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://yfz.xylfe.cn

println("Hello")
来源：http://wcf.ehwqpu.com

[T52] Scala：变量
来源：http://fwy.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://avv.yj20258.top

[T53] Scala：字符串插值
来源：http://zvv.vehdjk.com

s"值: $b"
来源：http://smc.xylfe.cn

[T54] Scala：集合映射
来源：http://yne.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://srb.birdmap.top

[T55] Scala：集合过滤
来源：http://eqo.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://nce.sysykeji.top

[T56] Scala：样例类
来源：http://xem.havefunace.top

case class User(name: String, age: Int)
来源：http://zdb.haohaochexian.top

[T57] Scala：模式匹配
来源：http://yrq.redwolf501.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zku.shzxlz.cn

[T58] Scala：函数定义
来源：http://nmb.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://myn.epnwcf.com

[T59] Scala：循环
来源：http://hcd.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://xnw.zhiwuduotai.top

[T60] Scala：折叠
来源：http://pll.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mnv.meibo888.top

================================================================================
来源：http://xtz.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qie.sysykeji.top

================================================================================
来源：http://oyw.gaohongyu789.top

[U01] Py：创建虚拟环境
来源：http://wpo.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://tak.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://fom.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dtc.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://pzu.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://smt.xylfe.cn

[U04] Py：变量调试打印
来源：http://njs.ydzc1.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://imc.aizwys.cn

[U05] Py：列表去重且保序
来源：http://yif.jqgufenzy.top

list(dict.fromkeys(arr))
来源：http://wvf.cheryme.top

[U06] Py：合并两个字典
来源：http://tgw.dashuyun.cn

{**a, **b}
来源：http://dhw.vehdjk.com

[U07] Py：反转字典键值
来源：http://hzt.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://zbr.shuidangran.top

[U08] Py：展平二维列表
来源：http://znp.aizwys.cn

[y for x in nested for y in x]
来源：http://mof.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://nib.jqgufenzy.top

max(d, key=d.get)
来源：http://bab.xuanzx.com

[U10] Py：按值排序字典
来源：http://dvw.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ogk.havefunace.top

[U11] Py：生成器表达式
来源：http://xdr.xuanzx.com

(x * 2 for x in arr)
来源：http://iyl.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ddt.uphjek.com

Counter(arr).most_common(3)
来源：http://frq.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://pwi.guowangkeji.top

deque(maxlen=10)
来源：http://pbs.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://jcw.hammf.cn

defaultdict(list)
来源：http://nqf.hywenlv.cn

[U15] Py：高精度计时
来源：http://jys.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://mvg.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://dwv.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nvh.shzxlz.cn

[U17] Py：初始化日志
来源：http://pfz.bbcook.cn

logging.basicConfig(level=logging.INFO)
来源：http://svo.havefunace.top

[U18] Py：预编译正则
来源：http://frh.iojbl.cn

pat = re.compile(r"\d+")
来源：http://lys.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://vzf.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ykk.havefunace.top

[U20] Py：缓存函数结果
来源：http://vmm.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://exe.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://vje.zhongyouzk.top

@contextlib.contextmanager
来源：http://pue.hammf.cn

[U22] Py：矩阵转置
来源：http://dhs.52xcode.cn

list(zip(*m))
来源：http://pkf.jqgfzy.top


<!-- 参考信息 -->