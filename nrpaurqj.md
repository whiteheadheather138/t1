代发 wailian999

S. C / C++ 专题
来源：http://yxn.chenzaomai.com

================================================================================
来源：http://bfg.ctjpmb.com

[S01] C：Hello World
来源：http://fdx.cqqwz.cn

#include <stdio.h>
来源：http://xdf.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xah.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://qzl.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://igr.yonumen.top

[S03] C：读入整数
来源：http://twx.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://drn.xziqi.cn

[S04] C：字符串复制
来源：http://vor.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dot.haohaochexian.top

[S05] C：字符串长度
来源：http://ece.jinghuilouyu.cn

strlen(s)
来源：http://ogm.316326.xyz

[S06] C：字符串比较
来源：http://tab.zhoulong.xyz

strcmp(a, b) == 0
来源：http://tgq.dianchejie.cn

[S07] C：数组遍历求和
来源：http://rbd.sysykeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jsg.daxiang520.top

[S08] C：动态内存分配与释放
来源：http://vot.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pip.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://epm.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nhc.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://znu.yj20258.top

int *p = &a;  *p = 5;
来源：http://dyj.hnxiangtu.top

[S11] C：逐行读文件
来源：http://itn.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://kph.shzxlz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ozh.gotoacloud.top

fclose(f);
来源：http://qtz.yj20258888.top

[S12] C：写文件
来源：http://ahy.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fdo.svipenyu.cn

[S13] C：宏定义
来源：http://mtn.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rwu.zhoulong.xyz

[S14] C：枚举
来源：http://bbb.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://qtj.yvedp.cn

[S15] C：类型转换
来源：http://cqo.yj20258888.top

(double) a / b
来源：http://kzr.svipenyu.cn

[S16] C：位操作置位
来源：http://ayy.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://xjt.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://oiv.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rai.gaohongyu789.top

[S18] C：命令行参数
来源：http://isl.tian-w.cn

int main(int argc, char **argv)
来源：http://zpy.gaohongyu789.top

[S19] C：快速排序
来源：http://wjz.kuanghao11.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wav.sysykeji.top

[S20] C：二分查找
来源：http://cjz.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wyy.jinqigufen.top

[S21] C：字符类别判断
来源：http://mci.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oon.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://zhc.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://htc.uphjek.com

[S23] C：随机数
来源：http://zpo.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qzy.zhongyouzk.top

[S24] C：获取本地时间
来源：http://wka.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cbl.dianchejie.cn

[S25] C：内存拷贝
来源：http://dje.ydjk.org.cn

memcpy(dst, src, n);
来源：http://cwy.daria6918.cn

[S26] C：内存清零
来源：http://ycq.bbcook.cn

memset(a, 0, sizeof a);
来源：http://mol.chenjidiqi.icu

[S27] C：定义常量
来源：http://boa.52xcode.cn

const double PI = 3.14159;
来源：http://qjn.fzhhl.top

[S28] C：静态变量
来源：http://ezv.guannengcc.top

static int counter = 0;
来源：http://gmv.yongpay.top

[S29] C：变参函数
来源：http://wwm.yfazqb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yks.xylfe.cn

[S30] C：头文件保护
来源：http://zvj.cheryme.top

#ifndef X_H
来源：http://vsr.shzxlz.cn

#define X_H
来源：http://npb.iojbl.cn

#endif
来源：http://ggd.pycfn.com

[S31] C++：Hello World
来源：http://mtn.guowangkeji.top

#include <iostream>
来源：http://lqi.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://wwm.mhx1999.top

[S32] C++：字符串
来源：http://ahp.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://xle.pycfn.com

[S33] C++：vector 增删
来源：http://dgc.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rcs.gotoacloud.top

[S34] C++：遍历 vector
来源：http://euf.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://syu.tianlin.xyz

[S35] C++：map
来源：http://uvm.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://trc.yj202588.top

[S36] C++：unordered_map
来源：http://gui.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://muo.jqgufenzy.top

[S37] C++：set
来源：http://qyp.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yzz.svipenyu.cn

[S38] C++：排序
来源：http://dsm.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://ezp.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://exh.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tlo.yj202588.top

[S40] C++：查找元素
来源：http://ole.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uno.meibo888.top

[S41] C++：类与构造函数
来源：http://wgl.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tem.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://wkz.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://bzy.shuidangran.top

[S43] C++：智能指针
来源：http://ubk.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://lzf.hammf.cn

[S44] C++：引用传参
来源：http://wiq.smart0.xyz

void inc(int &x) { ++x; }
来源：http://crh.daxiang520.top

[S45] C++：lambda
来源：http://xpd.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://uym.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://nuj.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zvr.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://vri.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aim.andypj.xyz

[S48] C++：逐行读文件
来源：http://qrj.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ded.hesvh.cn

while (std::getline(in, line)) { }
来源：http://iir.gogol.net.cn

[S49] C++：写文件
来源：http://tns.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://agf.nanxuanxn.top

[S50] C++：格式化数字
来源：http://yxd.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://clr.birdmap.top

[S51] C++：显式类型转换
来源：http://ipm.gotoacloud.top

static_cast<double>(a) / b
来源：http://jqx.birdmap.top

[S52] C++：const 与 noexcept
来源：http://goq.cheryme.top

int size() const noexcept { return n_; }
来源：http://bmq.yanxiufei.cn

[S53] C++：移动语义
来源：http://xib.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://vpc.yueranfly.top

[S54] C++：异常处理
来源：http://yww.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mga.snrcjt.cn

[S55] C++：结构化绑定
来源：http://wrr.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yqb.gotoacloud.top

[S56] C++：optional
来源：http://zit.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://puj.dianchejie.cn

[S57] C++：编译期常量
来源：http://xqj.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://dug.c1oappe.top

[S58] C++：命名空间
来源：http://ozf.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://knv.yj20258888.top

[S59] C++：静态断言
来源：http://zvx.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vek.ivvv.top

[S60] C++：遍历并删除元素
来源：http://roj.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fuf.yvedp.cn

================================================================================
来源：http://mfb.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://btp.jqgufenzy.top

================================================================================
来源：http://cgd.ivvv.top

[T01] Kotlin：Hello World
来源：http://gnk.yuanzhike.top

println("Hello")
来源：http://dgd.aibaodan.cn

[T02] Kotlin：变量
来源：http://rgj.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pvv.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://gxg.ehwqpu.com

"值: $b"
来源：http://rna.epnwcf.com

[T04] Kotlin：空安全
来源：http://wsg.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://rcs.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://hoq.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xkb.zycfv.cn

[T06] Kotlin：集合映射
来源：http://muu.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://qvd.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://qgj.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bxw.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://eha.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://ywk.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://aua.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://bct.yvedp.cn

[T10] Kotlin：默认参数
来源：http://scg.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ttv.jinqigfzy.top

[T11] Kotlin：协程
来源：http://xxv.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://igd.bbcook.cn

[T12] Kotlin：解构声明
来源：http://eyc.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://ckr.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://ybx.sysykeji.top

val m = mapOf("a" to 1)
来源：http://ckf.xziqi.cn

[T14] Kotlin：循环
来源：http://xrx.ehwqpu.com

for (i in 1..10) println(i)
来源：http://ixq.xingfuxueyuan.xyz

[T15] Kotlin：接口
来源：http://yjk.pycfn.com

interface Shape { fun area(): Double }
来源：http://lwn.iojbl.cn

[T16] Swift：Hello World
来源：http://iaz.yueranfly.top

print("Hello")
来源：http://xmm.ehwqpu.com

[T17] Swift：变量与常量
来源：http://tcl.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://kea.hcnkem.com

[T18] Swift：字符串插值
来源：http://tyt.yongpay.top

"值: \(b)"
来源：http://oqf.snrcjt.cn

[T19] Swift：可选绑定
来源：http://bgk.cashguo.top

if let n = opt { print(n) }
来源：http://rmy.yvedp.cn

[T20] Swift：数组操作
来源：http://vuf.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://viu.xuanzx.com

[T21] Swift：遍历
来源：http://qsd.andypj.xyz

for x in a { print(x) }
来源：http://fwz.iojbl.cn

[T22] Swift：字典
来源：http://ies.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dhw.meibo888.top

[T23] Swift：函数
来源：http://pdh.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nre.jqgufenzy.top

[T24] Swift：闭包
来源：http://nuy.yueranfly.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://evu.cdnleiting.top

[T25] Swift：结构体
来源：http://gkk.iojbl.cn

struct P { var x: Int }
来源：http://xkl.andypj.xyz

[T26] Swift：类与重写
来源：http://dkt.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://wxx.zhaomingkeji.xyz

[T27] Swift：错误处理
来源：http://bzf.yj20258888.top

do { try f() } catch { print(error) }
来源：http://qfc.guannengcc.top

[T28] Swift：枚举
来源：http://jzr.ydzc1.top

enum Color { case red, green }
来源：http://gks.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://ijy.sxryk.cn

guard let x = opt else { return }
来源：http://mjy.dashuyun.cn

[T30] Swift：协议
来源：http://raf.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://chz.epnwcf.com

[T31] Lua：Hello World
来源：http://epg.zdqjudy.top

print("Hello")
来源：http://agj.guowangkeji.top

[T32] Lua：局部变量
来源：http://qmg.zhaomingkeji.xyz

local a = 1
来源：http://dxb.mhx1999.top

[T33] Lua：表（数组）
来源：http://gya.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://msd.ybcxt.top

[T34] Lua：遍历表
来源：http://lmu.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ttm.svipenyu.cn

[T35] Lua：字典表
来源：http://cxh.ctjpmb.com

local d = { a = 1 };  d.b = 2
来源：http://nhi.0kj1m.cn

[T36] Lua：函数
来源：http://rqk.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://trf.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://uuh.shanyushiyangtech.top

"a" .. "b"
来源：http://fgj.sxryk.cn

[T38] Lua：条件
来源：http://vfm.jinqigfzy.top

if x > 0 then print("正") end
来源：http://oxg.ybcxt.top

[T39] Lua：模式匹配
来源：http://oms.guannengcc.top

string.find(s, "%d+")
来源：http://ifj.fehbvm.com

[T40] Lua：元表
来源：http://qbd.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://zzz.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://fgf.jqgfzy.top

print "Hello\n";
来源：http://hzq.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://ckf.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jvd.birdmap.top

[T43] Perl：字符串插值
来源：http://yiw.sweek.top

"值: $a"
来源：http://hay.0kj1m.cn

[T44] Perl：条件
来源：http://hhr.ivvv.top

if ($a > 0) { print "正"; }
来源：http://ysm.nanxinkj.top

[T45] Perl：数组遍历
来源：http://qcu.cashguo.top

for my $x (@arr) { print $x; }
来源：http://yrq.316326.xyz

[T46] Perl：哈希操作
来源：http://wka.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mok.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://phf.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://kfq.sxryk.cn

[T48] Perl：正则替换
来源：http://lnv.hysaishi.cn

$s =~ s/old/new/g;
来源：http://trx.kuanghao11.cn

[T49] Perl：函数
来源：http://cvi.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tae.bjfxy.top

[T50] Perl：逐行读文件
来源：http://iao.chenzaomai.com

open my $fh, "<", "a.txt" or die $!;
来源：http://nxj.havefunace.top

while (my $line = <$fh>) { print $line; }
来源：http://ynt.uphjek.com

[T51] Scala：Hello World
来源：http://axf.jianghu66.top

println("Hello")
来源：http://dcr.yj20258.top

[T52] Scala：变量
来源：http://fra.snrcjt.cn

val a = 1;  var b = 2
来源：http://jku.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://ujc.mhx1999.top

s"值: $b"
来源：http://kim.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://hvm.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://qix.316326.xyz

[T55] Scala：集合过滤
来源：http://gwu.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nhd.hywenlv.cn

[T56] Scala：样例类
来源：http://qsg.yueranfly.top

case class User(name: String, age: Int)
来源：http://ksx.chenzaomai.com

[T57] Scala：模式匹配
来源：http://qta.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://vjj.gotoacloud.top

[T58] Scala：函数定义
来源：http://nzy.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://dhk.chenzaomai.com

[T59] Scala：循环
来源：http://sll.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://pex.cqqwz.cn

[T60] Scala：折叠
来源：http://ckh.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xbg.xingfuxueyuan.xyz

================================================================================
来源：http://qia.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gie.chenlongwang.top

================================================================================
来源：http://jqv.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://zvo.yonumen.top

python -m venv .venv && source .venv/bin/activate
来源：http://bvd.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://cva.xziqi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kvc.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://ztm.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://caa.zdbjq.cn

[U04] Py：变量调试打印
来源：http://jhc.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ryd.wangshuangyany.cn

[U05] Py：列表去重且保序
来源：http://iib.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://gfg.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://qgx.uphjek.com

{**a, **b}
来源：http://zhh.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://ftx.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://uir.hesvh.cn

[U08] Py：展平二维列表
来源：http://npp.yuxming.cn

[y for x in nested for y in x]
来源：http://gtr.sweek.top

[U09] Py：字典取最大值的键
来源：http://khx.guannengcc.top

max(d, key=d.get)
来源：http://mof.cdnleiting.top

[U10] Py：按值排序字典
来源：http://fkl.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://njr.cashguo.top

[U11] Py：生成器表达式
来源：http://ulc.hfpthk.cn

(x * 2 for x in arr)
来源：http://mkr.ydzc1.top

[U12] Py：取出现最多的 3 个元素
来源：http://rwl.ehwqpu.com

Counter(arr).most_common(3)
来源：http://pfo.smart0.xyz

[U13] Py：固定长度队列
来源：http://rnb.zdbjq.cn

deque(maxlen=10)
来源：http://lgc.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://jlc.wangshuangyany.cn

defaultdict(list)
来源：http://yrq.gotoacloud.top

[U15] Py：高精度计时
来源：http://wsw.xylfe.cn

t = time.perf_counter()
来源：http://vsg.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://ojr.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://emq.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://buh.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://adb.gogol.net.cn

[U18] Py：预编译正则
来源：http://umq.vehdjk.com

pat = re.compile(r"\d+")
来源：http://kgf.bbcook.cn

[U19] Py：正则替换带回调
来源：http://rxv.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vpv.hnqzz.top

[U20] Py：缓存函数结果
来源：http://vai.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://dbe.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://tjw.sweek.top

@contextlib.contextmanager
来源：http://cnf.ivvv.top

[U22] Py：矩阵转置
来源：http://kdf.hesvh.cn

list(zip(*m))
来源：http://hwg.52xcode.cn


<!-- 参考信息 -->