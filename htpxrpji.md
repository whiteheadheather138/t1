代发 wailian999

S. C / C++ 专题
来源：http://iip.yj20258888.top

================================================================================
来源：http://ete.andypj.xyz

[S01] C：Hello World
来源：http://nrk.zhongyouzk.top

#include <stdio.h>
来源：http://npk.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://adm.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://lwl.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://qdd.c1oappe.top

[S03] C：读入整数
来源：http://lro.cashguo.top

int x; scanf("%d", &x);
来源：http://tef.aizwys.cn

[S04] C：字符串复制
来源：http://ftr.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://byv.jlsjyb.cn

[S05] C：字符串长度
来源：http://mud.shuidangran.top

strlen(s)
来源：http://meb.smart0.xyz

[S06] C：字符串比较
来源：http://tcd.chenzaomai.com

strcmp(a, b) == 0
来源：http://cxn.yongpay.top

[S07] C：数组遍历求和
来源：http://qcc.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pgq.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://inf.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zju.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://iem.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ckf.fehbvm.com

[S10] C：指针与解引用
来源：http://wom.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://ztg.hcnkem.com

[S11] C：逐行读文件
来源：http://ytu.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://xlg.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rya.iojbl.cn

fclose(f);
来源：http://hlv.sjlbkw.cn

[S12] C：写文件
来源：http://rel.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://djc.vehdjk.com

[S13] C：宏定义
来源：http://vah.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zri.meibo888.top

[S14] C：枚举
来源：http://rpl.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://ugv.zhiwuduotai.top

[S15] C：类型转换
来源：http://rag.cqqwz.cn

(double) a / b
来源：http://btl.9152youxi.cn

[S16] C：位操作置位
来源：http://qpk.xinyue.icu

x |= (1 << 3);
来源：http://jqd.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://nay.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kym.xziqi.cn

[S18] C：命令行参数
来源：http://rzb.aizwys.cn

int main(int argc, char **argv)
来源：http://dol.chenlongwang.top

[S19] C：快速排序
来源：http://qbf.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://msa.zhengqikj.top

[S20] C：二分查找
来源：http://sqj.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pfi.zhixingplan.top

[S21] C：字符类别判断
来源：http://oeg.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pss.nanxuanxn.top

[S22] C：字符串转数字
来源：http://qzh.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://cfx.jinyuanbaomall.cn

[S23] C：随机数
来源：http://llz.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mbo.jqgufenzy.top

[S24] C：获取本地时间
来源：http://axi.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zsl.ehwqpu.com

[S25] C：内存拷贝
来源：http://clt.jinqigufen.top

memcpy(dst, src, n);
来源：http://qkt.yj20258888.top

[S26] C：内存清零
来源：http://cvz.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://rpy.yueranfly.top

[S27] C：定义常量
来源：http://zqv.zycfv.cn

const double PI = 3.14159;
来源：http://mdk.zdbjq.cn

[S28] C：静态变量
来源：http://yqx.zhaomingkeji.xyz

static int counter = 0;
来源：http://ulo.aibaodan.cn

[S29] C：变参函数
来源：http://qoz.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hsj.tianlin.xyz

[S30] C：头文件保护
来源：http://rdf.havefunace.top

#ifndef X_H
来源：http://aju.sufxvd.cn

#define X_H
来源：http://nla.shanyushiyangkeji.top

#endif
来源：http://zim.tarul.cn

[S31] C++：Hello World
来源：http://hzp.zhiwuduotai.top

#include <iostream>
来源：http://fwh.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://zta.xylfe.cn

[S32] C++：字符串
来源：http://sru.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://itq.nanxuanxn.top

[S33] C++：vector 增删
来源：http://fyf.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bfb.0kj1m.cn

[S34] C++：遍历 vector
来源：http://boi.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://xsg.xziqi.cn

[S35] C++：map
来源：http://hee.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nit.tanke756.top

[S36] C++：unordered_map
来源：http://zyu.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uxu.sysykeji.top

[S37] C++：set
来源：http://mql.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hyy.fehbvm.com

[S38] C++：排序
来源：http://rtt.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://bao.tarul.cn

[S39] C++：自定义比较器排序
来源：http://hcl.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oty.zhixingplan.top

[S40] C++：查找元素
来源：http://qrw.hnqzz.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://phv.gogol.net.cn

[S41] C++：类与构造函数
来源：http://olf.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ohl.andypj.xyz

[S42] C++：继承与虚函数
来源：http://scj.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://ntu.zhongyouzk.top

[S43] C++：智能指针
来源：http://xez.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://ucp.yj202588.top

[S44] C++：引用传参
来源：http://epx.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://apn.xziqi.cn

[S45] C++：lambda
来源：http://jxl.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://khd.jiagoushi.top

[S46] C++：函数模板
来源：http://fmg.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hay.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://zmn.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nqu.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://gnb.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eks.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://ibr.hnqzz.top

[S49] C++：写文件
来源：http://jkg.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rlj.sufxvd.cn

[S50] C++：格式化数字
来源：http://dtk.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qzl.guowangkeji.top

[S51] C++：显式类型转换
来源：http://drf.ydzc1.top

static_cast<double>(a) / b
来源：http://hml.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://fnt.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://qjd.jqgufenzy.top

[S53] C++：移动语义
来源：http://pzm.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://rff.zhengqikj.top

[S54] C++：异常处理
来源：http://plk.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kri.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://ilt.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qcb.hesvh.cn

[S56] C++：optional
来源：http://rip.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sbe.yfazqb.com

[S57] C++：编译期常量
来源：http://yrh.mhx1999.top

constexpr int N = 10;
来源：http://fcy.tanke756.top

[S58] C++：命名空间
来源：http://nfp.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://yeh.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://qiy.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iuj.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://hnf.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bwn.kuanghao11.cn

================================================================================
来源：http://olu.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dji.cucudq.cn

================================================================================
来源：http://bxf.tanke756.top

[T01] Kotlin：Hello World
来源：http://ewi.haohaochexian.top

println("Hello")
来源：http://uca.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://ixc.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aup.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://vvo.redwolf501.top

"值: $b"
来源：http://zum.cqqwz.cn

[T04] Kotlin：空安全
来源：http://xkm.fzhhl.top

val n: String? = null;  n?.length
来源：http://ojz.xziqi.cn

[T05] Kotlin：when 表达式
来源：http://ole.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xsy.wangdashe.top

[T06] Kotlin：集合映射
来源：http://vtl.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://voz.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://jtm.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yfc.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://okl.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://zqc.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://pyq.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://aqz.cucudq.cn

[T10] Kotlin：默认参数
来源：http://bdk.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qry.zhijiandao.cn

[T11] Kotlin：协程
来源：http://awi.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bem.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://iyi.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://hod.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://zcr.daxiang520.top

val m = mapOf("a" to 1)
来源：http://mgs.zhengqikj.top

[T14] Kotlin：循环
来源：http://its.316326.xyz

for (i in 1..10) println(i)
来源：http://ljb.xziqi.cn

[T15] Kotlin：接口
来源：http://mke.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://tum.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://jio.gzhubu.top

print("Hello")
来源：http://uqe.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://uii.xinyue.icu

var a = 1;  let b = 2
来源：http://rnl.tian-w.cn

[T18] Swift：字符串插值
来源：http://vsv.guowangkeji.top

"值: \(b)"
来源：http://fke.tanke756.top

[T19] Swift：可选绑定
来源：http://wwu.gaohongyu789.top

if let n = opt { print(n) }
来源：http://axb.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://sza.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qwv.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://vsw.xinyue.icu

for x in a { print(x) }
来源：http://sqs.cheryme.top

[T22] Swift：字典
来源：http://ssp.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://kle.xinyue.icu

[T23] Swift：函数
来源：http://rlh.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ife.hcnkem.com

[T24] Swift：闭包
来源：http://gtt.andypj.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://kes.jlsjyb.cn

[T25] Swift：结构体
来源：http://thd.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://chy.xziqi.cn

[T26] Swift：类与重写
来源：http://uoh.hysaishi.cn

class A: Base { override func f() {} }
来源：http://klt.cheryme.top

[T27] Swift：错误处理
来源：http://nhr.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://ssy.smart0.xyz

[T28] Swift：枚举
来源：http://isx.sufxvd.cn

enum Color { case red, green }
来源：http://ivc.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://cej.jinqigufen.top

guard let x = opt else { return }
来源：http://wcj.c1oappe.top

[T30] Swift：协议
来源：http://ebv.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://vjh.jqgufenzy.top

[T31] Lua：Hello World
来源：http://aox.cucudq.cn

print("Hello")
来源：http://akd.yonumen.top

[T32] Lua：局部变量
来源：http://wnh.zhongyouzk.top

local a = 1
来源：http://gww.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://mwm.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ven.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://ueo.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rkn.tarul.cn

[T35] Lua：字典表
来源：http://doc.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://drk.svipenyu.cn

[T36] Lua：函数
来源：http://gvl.jinqigufen.top

function add(a, b) return a + b end
来源：http://mgv.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://dvm.0kj1m.cn

"a" .. "b"
来源：http://iob.cheryme.top

[T38] Lua：条件
来源：http://aix.xziqi.cn

if x > 0 then print("正") end
来源：http://vsm.nanxinkj.top

[T39] Lua：模式匹配
来源：http://wwl.havefunace.top

string.find(s, "%d+")
来源：http://dzi.dianchejie.cn

[T40] Lua：元表
来源：http://xwd.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://mak.fzhhl.top

[T41] Perl：Hello World
来源：http://zcg.jinghuilouyu.cn

print "Hello\n";
来源：http://qss.fzhhl.top

[T42] Perl：变量类型
来源：http://weh.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://scd.c1oappe.top

[T43] Perl：字符串插值
来源：http://iwv.aibaodan.cn

"值: $a"
来源：http://wnj.smart0.xyz

[T44] Perl：条件
来源：http://svt.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://toh.ppjwa.cn

[T45] Perl：数组遍历
来源：http://ayy.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://ouj.yuanzhike.top

[T46] Perl：哈希操作
来源：http://nhz.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ilk.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://woy.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://udp.daxiang520.top

[T48] Perl：正则替换
来源：http://ypl.iojbl.cn

$s =~ s/old/new/g;
来源：http://mum.aizwys.cn

[T49] Perl：函数
来源：http://vrn.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ggv.birdmap.top

[T50] Perl：逐行读文件
来源：http://tms.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mcz.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://twz.cqqwz.cn

[T51] Scala：Hello World
来源：http://otn.shanyushiyangkeji.top

println("Hello")
来源：http://ivh.cqqwz.cn

[T52] Scala：变量
来源：http://qni.redwolf501.top

val a = 1;  var b = 2
来源：http://nhg.bbcook.cn

[T53] Scala：字符串插值
来源：http://zlv.hfpthk.cn

s"值: $b"
来源：http://vpt.cashguo.top

[T54] Scala：集合映射
来源：http://lgg.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://gxy.yfazqb.com

[T55] Scala：集合过滤
来源：http://noa.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://gxr.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://cnf.sxryk.cn

case class User(name: String, age: Int)
来源：http://xrx.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://tbu.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ytg.yongpay.top

[T58] Scala：函数定义
来源：http://vwy.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rum.yueranfly.top

[T59] Scala：循环
来源：http://njz.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://nee.gzhubu.top

[T60] Scala：折叠
来源：http://aww.xinyue.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rab.tian-w.cn

================================================================================
来源：http://gny.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rll.wangshuangyany.cn

================================================================================
来源：http://eoh.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://xua.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://mkb.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://ifq.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vcw.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://rhi.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mjj.0kj1m.cn

[U04] Py：变量调试打印
来源：http://rve.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zwi.0kj1m.cn

[U05] Py：列表去重且保序
来源：http://srt.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://ynw.iojbl.cn

[U06] Py：合并两个字典
来源：http://gyv.zycfv.cn

{**a, **b}
来源：http://zlk.yuanzhike.top

[U07] Py：反转字典键值
来源：http://sxk.jinghuilouyu.cn

{v: k for k, v in d.items()}
来源：http://mvp.zdqjudy.top

[U08] Py：展平二维列表
来源：http://utz.yuanzhike.top

[y for x in nested for y in x]
来源：http://gcx.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://pfg.jyoumei.cn

max(d, key=d.get)
来源：http://wzl.tianlin.xyz

[U10] Py：按值排序字典
来源：http://xlt.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tnb.ivvv.top

[U11] Py：生成器表达式
来源：http://mss.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://koq.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://sez.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://vlg.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://sty.daxiang520.top

deque(maxlen=10)
来源：http://ais.hcnkem.com

[U14] Py：分组收集到列表
来源：http://ynj.hongshengwenyu.top

defaultdict(list)
来源：http://jhn.fktsv.cn

[U15] Py：高精度计时
来源：http://cwp.quarkkingdee.top

t = time.perf_counter()
来源：http://rct.sweek.top

[U16] Py：命令行参数解析
来源：http://myn.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mcx.fktsv.cn

[U17] Py：初始化日志
来源：http://gvh.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://mzk.gogol.net.cn

[U18] Py：预编译正则
来源：http://zby.daxiang520.top

pat = re.compile(r"\d+")
来源：http://eof.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://zyp.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dks.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://fgi.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://tid.hfpthk.cn

[U21] Py：自定义上下文管理器
来源：http://ygp.hysaishi.cn

@contextlib.contextmanager
来源：http://dwm.jqgfzy.top

[U22] Py：矩阵转置
来源：http://blp.fengsongda.top

list(zip(*m))
来源：http://rwg.ywan-chungtsiang.top


<!-- 参考信息 -->