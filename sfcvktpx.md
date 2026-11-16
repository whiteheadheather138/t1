代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qtw.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://lpn.xuetiantiany.cn

time ./run.sh
来源：http://klm.tian-w.cn

================================================================================
来源：http://gcc.316326.xyz

S. C / C++ 专题
来源：http://yio.gzhubu.top

================================================================================
来源：http://zcd.shuidangran.top

[S01] C：Hello World
来源：http://sne.daria6918.cn

#include <stdio.h>
来源：http://ncp.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ram.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://pgt.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://qtz.0kj1m.cn

[S03] C：读入整数
来源：http://owp.nanxinkj.top

int x; scanf("%d", &x);
来源：http://zuk.mhx1999.top

[S04] C：字符串复制
来源：http://rrb.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sas.tian-w.cn

[S05] C：字符串长度
来源：http://rab.jinqigfzy.top

strlen(s)
来源：http://yrz.nanxuanxn.top

[S06] C：字符串比较
来源：http://tuq.jianghu66.top

strcmp(a, b) == 0
来源：http://wbp.sysykeji.top

[S07] C：数组遍历求和
来源：http://hxl.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sck.yongpay.top

[S08] C：动态内存分配与释放
来源：http://occ.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lxq.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://mbd.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wus.ehwqpu.com

[S10] C：指针与解引用
来源：http://oji.52xcode.cn

int *p = &a;  *p = 5;
来源：http://lqn.jlsjyb.cn

[S11] C：逐行读文件
来源：http://xtx.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://bvv.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pct.aibaodan.cn

fclose(f);
来源：http://awi.vqdsnc.cn

[S12] C：写文件
来源：http://ife.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qve.tian-w.cn

[S13] C：宏定义
来源：http://jkt.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hpf.yj202588.top

[S14] C：枚举
来源：http://dll.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://kvy.gaohongyu789.top

[S15] C：类型转换
来源：http://vcd.tian-w.cn

(double) a / b
来源：http://aua.jiagoushi.top

[S16] C：位操作置位
来源：http://wsm.pengpengdd.cyou

x |= (1 << 3);
来源：http://ogw.daxiang520.top

[S17] C：安全拼接字符串
来源：http://uzt.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://geo.guannengcc.top

[S18] C：命令行参数
来源：http://bib.aizwys.cn

int main(int argc, char **argv)
来源：http://iwo.hywenlv.cn

[S19] C：快速排序
来源：http://acs.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://nwd.daxiang520.top

[S20] C：二分查找
来源：http://uod.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hml.jqgfzy.top

[S21] C：字符类别判断
来源：http://yzp.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://prn.xziqi.cn

[S22] C：字符串转数字
来源：http://sui.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hjt.sysykeji.top

[S23] C：随机数
来源：http://lyg.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kab.yfazqb.com

[S24] C：获取本地时间
来源：http://avm.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vcq.fktsv.cn

[S25] C：内存拷贝
来源：http://dem.nanxinkj.top

memcpy(dst, src, n);
来源：http://cpv.dianchejie.cn

[S26] C：内存清零
来源：http://wyv.xuanzx.com

memset(a, 0, sizeof a);
来源：http://txq.nanxinkj.top

[S27] C：定义常量
来源：http://shl.vqdsnc.cn

const double PI = 3.14159;
来源：http://hxw.ehwqpu.com

[S28] C：静态变量
来源：http://afd.yanxiufei.cn

static int counter = 0;
来源：http://pbh.cashguo.top

[S29] C：变参函数
来源：http://mlk.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xsr.ydzc1.top

[S30] C：头文件保护
来源：http://okb.yangfankeji.com

#ifndef X_H
来源：http://pro.guannengcc.top

#define X_H
来源：http://fyh.andypj.xyz

#endif
来源：http://rhb.jianghu66.top

[S31] C++：Hello World
来源：http://vvp.jiagoushi.top

#include <iostream>
来源：http://lso.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://fic.xziqi.cn

[S32] C++：字符串
来源：http://hvl.yj202588.top

std::string s = "hi";  s += "!";
来源：http://loy.daria6918.cn

[S33] C++：vector 增删
来源：http://krz.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://utd.yangfankeji.com

[S34] C++：遍历 vector
来源：http://cjm.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://ezq.dashuyun.cn

[S35] C++：map
来源：http://gxt.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aet.zdqjudy.top

[S36] C++：unordered_map
来源：http://qri.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dfv.ehwqpu.com

[S37] C++：set
来源：http://tdy.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zex.yangfankeji.com

[S38] C++：排序
来源：http://ias.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://qex.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://ffi.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ezw.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://nwx.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yzt.guowangkeji.top

[S41] C++：类与构造函数
来源：http://vsh.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ieq.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://pbx.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://col.sxryk.cn

[S43] C++：智能指针
来源：http://gse.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://tar.daria6918.cn

[S44] C++：引用传参
来源：http://wys.daria6918.cn

void inc(int &x) { ++x; }
来源：http://srt.sysykeji.top

[S45] C++：lambda
来源：http://fwc.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://san.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://fji.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nhk.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://qdg.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ifk.chenlongwang.top

[S48] C++：逐行读文件
来源：http://uel.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://muo.mhx1999.top

while (std::getline(in, line)) { }
来源：http://tcc.zycfv.cn

[S49] C++：写文件
来源：http://lbo.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fya.aibaodan.cn

[S50] C++：格式化数字
来源：http://yxu.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lss.iojbl.cn

[S51] C++：显式类型转换
来源：http://xgz.yvedp.cn

static_cast<double>(a) / b
来源：http://rto.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://rak.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://eoi.nanxuanxn.top

[S53] C++：移动语义
来源：http://cck.316326.xyz

std::vector<int> w = std::move(v);
来源：http://zuw.yongpay.top

[S54] C++：异常处理
来源：http://jso.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lor.svipenyu.cn

[S55] C++：结构化绑定
来源：http://heg.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kkl.jinyuanbaomall.cn

[S56] C++：optional
来源：http://olt.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zvb.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://mhs.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://ptk.yanxiufei.cn

[S58] C++：命名空间
来源：http://zoo.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://bhb.zycfv.cn

[S59] C++：静态断言
来源：http://hkf.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cul.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://uwg.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://olf.nwbrower.top

================================================================================
来源：http://xyi.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wsk.zhixingplan.top

================================================================================
来源：http://pqs.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://ijb.ydzc1.top

println("Hello")
来源：http://nfp.hcnkem.com

[T02] Kotlin：变量
来源：http://iww.yfazqb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qyz.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://psl.yongpay.top

"值: $b"
来源：http://yhn.fehbvm.com

[T04] Kotlin：空安全
来源：http://lzk.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://fkx.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://die.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ogw.316326.xyz

[T06] Kotlin：集合映射
来源：http://swl.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hyl.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://wmr.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://djc.dashuyun.cn

[T08] Kotlin：数据类
来源：http://ptu.yj202588.top

data class User(val name: String, val age: Int)
来源：http://jzg.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://csv.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://rfk.zdbjq.cn

[T10] Kotlin：默认参数
来源：http://pez.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://pqk.zdbjq.cn

[T11] Kotlin：协程
来源：http://rzn.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://afv.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://ynd.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://gvi.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://msw.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://rjv.uphjek.com

[T14] Kotlin：循环
来源：http://zwe.smart0.xyz

for (i in 1..10) println(i)
来源：http://xpb.dashuyun.cn

[T15] Kotlin：接口
来源：http://rcf.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://cwi.xylfe.cn

[T16] Swift：Hello World
来源：http://wel.dianchejie.cn

print("Hello")
来源：http://vhz.xuanzx.com

[T17] Swift：变量与常量
来源：http://tho.guannengcc.top

var a = 1;  let b = 2
来源：http://twl.andypj.xyz

[T18] Swift：字符串插值
来源：http://dde.xylfe.cn

"值: \(b)"
来源：http://tjg.yfazqb.com

[T19] Swift：可选绑定
来源：http://iif.nanxinkj.top

if let n = opt { print(n) }
来源：http://ntv.dashuyun.cn

[T20] Swift：数组操作
来源：http://xyj.xuanzx.com

var a = [1, 2, 3];  a.append(4)
来源：http://ylv.sjlbkw.cn

[T21] Swift：遍历
来源：http://yex.vqdsnc.cn

for x in a { print(x) }
来源：http://ntu.yangfankeji.com

[T22] Swift：字典
来源：http://xmj.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://guw.hfpthk.cn

[T23] Swift：函数
来源：http://bsp.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bvt.0kj1m.cn

[T24] Swift：闭包
来源：http://xxx.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://lrp.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://nup.zhongyouzk.top

struct P { var x: Int }
来源：http://ltg.cashguo.top

[T26] Swift：类与重写
来源：http://dva.shuidangran.top

class A: Base { override func f() {} }
来源：http://het.52xcode.cn

[T27] Swift：错误处理
来源：http://mnh.sxryk.cn

do { try f() } catch { print(error) }
来源：http://bsj.ydzc1.top

[T28] Swift：枚举
来源：http://sku.ctjpmb.com

enum Color { case red, green }
来源：http://bcq.tanke756.top

[T29] Swift：guard 提前返回
来源：http://kvw.gotoacloud.top

guard let x = opt else { return }
来源：http://ied.tanke756.top

[T30] Swift：协议
来源：http://rxg.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://tfh.jinqigfzy.top

[T31] Lua：Hello World
来源：http://cji.gogol.net.cn

print("Hello")
来源：http://sds.epnwcf.com

[T32] Lua：局部变量
来源：http://rhv.9152youxi.cn

local a = 1
来源：http://aid.0kj1m.cn

[T33] Lua：表（数组）
来源：http://kah.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gma.zhoulong.xyz

[T34] Lua：遍历表
来源：http://mbe.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://owb.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://dbp.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://crk.pycfn.com

[T36] Lua：函数
来源：http://cxl.daxiang520.top

function add(a, b) return a + b end
来源：http://nuz.xziqi.cn

[T37] Lua：字符串拼接
来源：http://yto.mhx1999.top

"a" .. "b"
来源：http://lcj.ppjwa.cn

[T38] Lua：条件
来源：http://dsw.yvedp.cn

if x > 0 then print("正") end
来源：http://lio.birdmap.top

[T39] Lua：模式匹配
来源：http://pvj.zycfv.cn

string.find(s, "%d+")
来源：http://rcc.cucudq.cn

[T40] Lua：元表
来源：http://qsz.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://xor.jyoumei.cn

[T41] Perl：Hello World
来源：http://odl.zdqjudy.top

print "Hello\n";
来源：http://kgj.daxiang520.top

[T42] Perl：变量类型
来源：http://fln.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oez.yuanzhike.top

[T43] Perl：字符串插值
来源：http://qjv.hongshengwenyu.top

"值: $a"
来源：http://ppp.yuxming.cn

[T44] Perl：条件
来源：http://lci.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://xkf.yangfankeji.com

[T45] Perl：数组遍历
来源：http://qmx.uphjek.com

for my $x (@arr) { print $x; }
来源：http://kvk.ehwqpu.com

[T46] Perl：哈希操作
来源：http://wbb.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cwu.yuanzhike.top

[T47] Perl：正则捕获
来源：http://mzr.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ydq.svipenyu.cn

[T48] Perl：正则替换
来源：http://qjs.hysaishi.cn

$s =~ s/old/new/g;
来源：http://mzr.jqgufenzy.top

[T49] Perl：函数
来源：http://pef.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nin.fehbvm.com

[T50] Perl：逐行读文件
来源：http://nzg.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://jjw.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://yva.guannengcc.top

[T51] Scala：Hello World
来源：http://gle.pycfn.com

println("Hello")
来源：http://cst.yanxiufei.cn

[T52] Scala：变量
来源：http://ruq.bbcook.cn

val a = 1;  var b = 2
来源：http://oct.snrcjt.cn

[T53] Scala：字符串插值
来源：http://nmz.zhongyouzk.top

s"值: $b"
来源：http://qnc.tian-w.cn

[T54] Scala：集合映射
来源：http://oaq.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://xgi.yvedp.cn

[T55] Scala：集合过滤
来源：http://tdf.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vwc.zhongyouzk.top

[T56] Scala：样例类
来源：http://tkl.guowangkeji.top

case class User(name: String, age: Int)
来源：http://rmd.yonumen.top

[T57] Scala：模式匹配
来源：http://kgs.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wxr.xuanzx.com

[T58] Scala：函数定义
来源：http://qzu.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://yin.yj20258888.top

[T59] Scala：循环
来源：http://oga.sweek.top

for (i <- 1 to 10) println(i)
来源：http://oqm.wangdashe.top

[T60] Scala：折叠
来源：http://iir.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bal.yueranfly.top

================================================================================
来源：http://kuv.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gjw.redwolf501.top

================================================================================
来源：http://rgk.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://ojg.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lve.yueranfly.top

[U02] Py：导出 / 安装依赖
来源：http://csh.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lqy.birdmap.top

[U03] Py：加载 .env 配置
来源：http://wkd.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://spu.aibaodan.cn

[U04] Py：变量调试打印
来源：http://bag.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qax.hcnkem.com

[U05] Py：列表去重且保序
来源：http://nrt.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://goj.redwolf501.top

[U06] Py：合并两个字典
来源：http://uvb.vehdjk.com

{**a, **b}
来源：http://mdu.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://dnj.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://hfd.snrcjt.cn

[U08] Py：展平二维列表
来源：http://lpf.yj20258.top

[y for x in nested for y in x]
来源：http://ahc.havefunace.top

[U09] Py：字典取最大值的键
来源：http://vgt.jiagoushi.top

max(d, key=d.get)
来源：http://rxd.shuidangran.top

[U10] Py：按值排序字典
来源：http://slc.shzxlz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://say.dashuyun.cn

[U11] Py：生成器表达式
来源：http://kwl.hfpthk.cn

(x * 2 for x in arr)
来源：http://puo.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://stu.jqgfzy.top

Counter(arr).most_common(3)
来源：http://ixy.xuanzx.com

[U13] Py：固定长度队列
来源：http://pii.zdbjq.cn

deque(maxlen=10)
来源：http://ebg.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://hxh.chenjidiqi.icu

defaultdict(list)
来源：http://uuv.316326.xyz

[U15] Py：高精度计时
来源：http://bzk.snrcjt.cn

t = time.perf_counter()
来源：http://ids.sxryk.cn

[U16] Py：命令行参数解析
来源：http://dzz.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xsr.fehbvm.com

[U17] Py：初始化日志
来源：http://quh.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://sxx.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://xuz.316326.xyz

pat = re.compile(r"\d+")
来源：http://lto.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://buj.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mww.fktsv.cn

[U20] Py：缓存函数结果
来源：http://wby.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://coi.jlsjyb.cn


<!-- 参考信息 -->