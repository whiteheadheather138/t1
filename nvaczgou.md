代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://faq.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://oal.sysykeji.top

time ./run.sh
来源：http://nfh.hnxiangtu.top

================================================================================
来源：http://skd.zhixingplan.top

S. C / C++ 专题
来源：http://pyj.ybcxt.top

================================================================================
来源：http://vze.kuanghao11.cn

[S01] C：Hello World
来源：http://usw.ybcxt.top

#include <stdio.h>
来源：http://kpg.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://eyu.birdmap.top

[S02] C：变量与格式化输出
来源：http://pjy.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://yqe.xuetiantiany.cn

[S03] C：读入整数
来源：http://fcg.fktsv.cn

int x; scanf("%d", &x);
来源：http://epl.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://nlp.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://uir.yj20258.top

[S05] C：字符串长度
来源：http://hec.ywan-chungtsiang.top

strlen(s)
来源：http://gcb.smart0.xyz

[S06] C：字符串比较
来源：http://bel.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://fwt.hesvh.cn

[S07] C：数组遍历求和
来源：http://cmh.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tzf.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://cfx.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pgk.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://vgi.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://onf.yuanzhike.top

[S10] C：指针与解引用
来源：http://upj.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://fpk.fehbvm.com

[S11] C：逐行读文件
来源：http://vlv.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://hwm.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://veo.yanxiufei.cn

fclose(f);
来源：http://wye.shzxlz.cn

[S12] C：写文件
来源：http://fqv.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mci.hnxiangtu.top

[S13] C：宏定义
来源：http://szo.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zzf.ehwqpu.com

[S14] C：枚举
来源：http://taa.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://csf.haohaochexian.top

[S15] C：类型转换
来源：http://ojp.shuidangran.top

(double) a / b
来源：http://yoz.snrcjt.cn

[S16] C：位操作置位
来源：http://uik.svipenyu.cn

x |= (1 << 3);
来源：http://rtb.tanke756.top

[S17] C：安全拼接字符串
来源：http://byp.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://njs.feifeiyinyue.top

[S18] C：命令行参数
来源：http://mud.gaohongyu789.top

int main(int argc, char **argv)
来源：http://vgz.cashguo.top

[S19] C：快速排序
来源：http://yyi.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jwr.tianlin.xyz

[S20] C：二分查找
来源：http://dlt.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jas.fehbvm.com

[S21] C：字符类别判断
来源：http://bgi.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pzp.zhengqikj.top

[S22] C：字符串转数字
来源：http://rrh.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://fuw.cucudq.cn

[S23] C：随机数
来源：http://qvz.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qrx.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://lpd.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kym.hesvh.cn

[S25] C：内存拷贝
来源：http://ybe.aizwys.cn

memcpy(dst, src, n);
来源：http://wtb.gogol.net.cn

[S26] C：内存清零
来源：http://btz.smart0.xyz

memset(a, 0, sizeof a);
来源：http://xoj.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://ggw.cashguo.top

const double PI = 3.14159;
来源：http://bpx.ctjpmb.com

[S28] C：静态变量
来源：http://sgw.bjfxy.top

static int counter = 0;
来源：http://pwd.dashuyun.cn

[S29] C：变参函数
来源：http://sbe.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rnc.cheryme.top

[S30] C：头文件保护
来源：http://roi.smart0.xyz

#ifndef X_H
来源：http://foq.svipenyu.cn

#define X_H
来源：http://egr.sysykeji.top

#endif
来源：http://pfn.hcnkem.com

[S31] C++：Hello World
来源：http://eav.cheryme.top

#include <iostream>
来源：http://fbb.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://xnv.fanxiaobao.xyz

[S32] C++：字符串
来源：http://zij.yonumen.top

std::string s = "hi";  s += "!";
来源：http://meo.shuidangran.top

[S33] C++：vector 增删
来源：http://prt.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qvb.xinyue.icu

[S34] C++：遍历 vector
来源：http://srm.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://dhx.yj20258.top

[S35] C++：map
来源：http://bqw.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hsp.ctjpmb.com

[S36] C++：unordered_map
来源：http://zdb.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bei.zdbjq.cn

[S37] C++：set
来源：http://udj.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fsx.jinghuilouyu.cn

[S38] C++：排序
来源：http://kln.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://coq.316326.xyz

[S39] C++：自定义比较器排序
来源：http://gee.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aao.jqgufenzy.top

[S40] C++：查找元素
来源：http://xau.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ctg.uphjek.com

[S41] C++：类与构造函数
来源：http://xou.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ria.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://oqy.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://zji.yvedp.cn

[S43] C++：智能指针
来源：http://svx.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://era.nwbrower.top

[S44] C++：引用传参
来源：http://jjc.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://shh.smart0.xyz

[S45] C++：lambda
来源：http://uxe.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://bbc.cdnleiting.top

[S46] C++：函数模板
来源：http://aqw.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kwx.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://xqz.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oti.hcnkem.com

[S48] C++：逐行读文件
来源：http://uey.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qpo.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://ssb.dashuyun.cn

[S49] C++：写文件
来源：http://xyd.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fps.nanxuanxn.top

[S50] C++：格式化数字
来源：http://zci.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sct.aibaodan.cn

[S51] C++：显式类型转换
来源：http://xlv.0kj1m.cn

static_cast<double>(a) / b
来源：http://knu.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://fbr.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://pbv.guowangkeji.top

[S53] C++：移动语义
来源：http://aas.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://cgd.ctjpmb.com

[S54] C++：异常处理
来源：http://dmd.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zyf.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://rqx.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nwq.0kj1m.cn

[S56] C++：optional
来源：http://oge.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nfw.52xcode.cn

[S57] C++：编译期常量
来源：http://njk.xylfe.cn

constexpr int N = 10;
来源：http://cel.yuanzhike.top

[S58] C++：命名空间
来源：http://ujz.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://nyt.ydzc1.top

[S59] C++：静态断言
来源：http://qsx.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zed.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://olm.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://awe.shangyingyoupin.top

================================================================================
来源：http://ztb.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dxp.epnwcf.com

================================================================================
来源：http://kqc.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://dkw.gotoacloud.top

println("Hello")
来源：http://ynb.hywenlv.cn

[T02] Kotlin：变量
来源：http://vhc.wangshuangyany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jor.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://knk.zhixingplan.top

"值: $b"
来源：http://glr.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://ghp.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://kam.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://azf.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://egh.tian-w.cn

[T06] Kotlin：集合映射
来源：http://vuh.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://iwv.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://buq.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ldu.jianghu66.top

[T08] Kotlin：数据类
来源：http://spi.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://tbf.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://thb.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://ucq.daria6918.cn

[T10] Kotlin：默认参数
来源：http://onw.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cnb.daria6918.cn

[T11] Kotlin：协程
来源：http://mvq.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ryp.sxryk.cn

[T12] Kotlin：解构声明
来源：http://cpx.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://giv.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://ttz.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://nqz.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://rwa.nanxinkj.top

for (i in 1..10) println(i)
来源：http://lry.cheryme.top

[T15] Kotlin：接口
来源：http://qea.tanke756.top

interface Shape { fun area(): Double }
来源：http://ycd.uphjek.com

[T16] Swift：Hello World
来源：http://krn.epnwcf.com

print("Hello")
来源：http://zam.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://amj.gzhubu.top

var a = 1;  let b = 2
来源：http://lqw.cheryme.top

[T18] Swift：字符串插值
来源：http://mpb.uphjek.com

"值: \(b)"
来源：http://lid.316326.xyz

[T19] Swift：可选绑定
来源：http://man.andypj.xyz

if let n = opt { print(n) }
来源：http://njd.chenzaomai.com

[T20] Swift：数组操作
来源：http://ora.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vhl.hcnkem.com

[T21] Swift：遍历
来源：http://uzh.fzhhl.top

for x in a { print(x) }
来源：http://prh.9152youxi.cn

[T22] Swift：字典
来源：http://wvw.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://syo.aibaodan.cn

[T23] Swift：函数
来源：http://nfq.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hin.redwolf501.top

[T24] Swift：闭包
来源：http://tsl.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ofy.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://wzo.ehwqpu.com

struct P { var x: Int }
来源：http://gxe.vehdjk.com

[T26] Swift：类与重写
来源：http://ild.jqgfzy.top

class A: Base { override func f() {} }
来源：http://icl.andypj.xyz

[T27] Swift：错误处理
来源：http://eec.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://vyc.sweek.top

[T28] Swift：枚举
来源：http://esf.jyoumei.cn

enum Color { case red, green }
来源：http://puf.cqqwz.cn

[T29] Swift：guard 提前返回
来源：http://rsy.svipenyu.cn

guard let x = opt else { return }
来源：http://tvn.wangshuangyany.cn

[T30] Swift：协议
来源：http://eoq.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://phg.hfpthk.cn

[T31] Lua：Hello World
来源：http://cdl.yanxiufei.cn

print("Hello")
来源：http://otb.zhongyouzk.top

[T32] Lua：局部变量
来源：http://hxr.vehdjk.com

local a = 1
来源：http://tap.hysaishi.cn

[T33] Lua：表（数组）
来源：http://bzn.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://amb.cheryme.top

[T34] Lua：遍历表
来源：http://bqz.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eoj.yonumen.top

[T35] Lua：字典表
来源：http://igm.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://twh.jinqigfzy.top

[T36] Lua：函数
来源：http://lal.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://hrv.xuanzx.com

[T37] Lua：字符串拼接
来源：http://upe.feifeiyinyue.top

"a" .. "b"
来源：http://uja.uphjek.com

[T38] Lua：条件
来源：http://ema.vehdjk.com

if x > 0 then print("正") end
来源：http://enr.hywenlv.cn

[T39] Lua：模式匹配
来源：http://fsp.hfpthk.cn

string.find(s, "%d+")
来源：http://jtn.sweek.top

[T40] Lua：元表
来源：http://smf.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://ddx.nanxuanxn.top

[T41] Perl：Hello World
来源：http://lwk.dianchejie.cn

print "Hello\n";
来源：http://wsu.ybcxt.top

[T42] Perl：变量类型
来源：http://xtl.birdmap.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zil.ehwqpu.com

[T43] Perl：字符串插值
来源：http://bxl.52xcode.cn

"值: $a"
来源：http://kxw.52xcode.cn

[T44] Perl：条件
来源：http://yrm.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://aup.zycfv.cn

[T45] Perl：数组遍历
来源：http://kvh.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://jyp.gaohongyu789.top

[T46] Perl：哈希操作
来源：http://hot.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wjq.redwolf501.top

[T47] Perl：正则捕获
来源：http://azy.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rqm.havefunace.top

[T48] Perl：正则替换
来源：http://qas.redwolf501.top

$s =~ s/old/new/g;
来源：http://sfm.zdqjudy.top

[T49] Perl：函数
来源：http://iai.nanxinkj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xgb.smart0.xyz

[T50] Perl：逐行读文件
来源：http://oaa.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wvt.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://rgk.cdnleiting.top

[T51] Scala：Hello World
来源：http://zoe.wangshuangyany.cn

println("Hello")
来源：http://vmw.ydjk.org.cn

[T52] Scala：变量
来源：http://rfg.sjlbkw.cn

val a = 1;  var b = 2
来源：http://ftb.fehbvm.com

[T53] Scala：字符串插值
来源：http://idc.sufxvd.cn

s"值: $b"
来源：http://mbd.dashuyun.cn

[T54] Scala：集合映射
来源：http://eud.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://lrf.ydzc1.top

[T55] Scala：集合过滤
来源：http://xgz.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://edr.chenzaomai.com

[T56] Scala：样例类
来源：http://lte.aibaodan.cn

case class User(name: String, age: Int)
来源：http://qaf.zhixingplan.top

[T57] Scala：模式匹配
来源：http://gue.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://bqb.yvedp.cn

[T58] Scala：函数定义
来源：http://iuw.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://gej.meibo888.top

[T59] Scala：循环
来源：http://dny.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://mmu.tarul.cn

[T60] Scala：折叠
来源：http://vyh.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cbu.shzxlz.cn

================================================================================
来源：http://xll.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dpi.yj20258.top

================================================================================
来源：http://pjp.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://tvv.tanke756.top

python -m venv .venv && source .venv/bin/activate
来源：http://wsd.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://ezu.hammf.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qny.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://uhl.zdbjq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zam.hesvh.cn

[U04] Py：变量调试打印
来源：http://far.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jqv.yfazqb.com

[U05] Py：列表去重且保序
来源：http://sol.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://mhm.zycfv.cn

[U06] Py：合并两个字典
来源：http://zgy.sufxvd.cn

{**a, **b}
来源：http://wpj.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://ltw.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://tbe.yueranfly.top

[U08] Py：展平二维列表
来源：http://vsl.xinyue.icu

[y for x in nested for y in x]
来源：http://fxr.cashguo.top

[U09] Py：字典取最大值的键
来源：http://vbj.zycfv.cn

max(d, key=d.get)
来源：http://oju.cqqwz.cn

[U10] Py：按值排序字典
来源：http://ttn.mhx1999.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bjl.redwolf501.top

[U11] Py：生成器表达式
来源：http://rnl.jlsjyb.cn

(x * 2 for x in arr)
来源：http://ymc.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://fxw.xylfe.cn

Counter(arr).most_common(3)
来源：http://lat.shuidangran.top

[U13] Py：固定长度队列
来源：http://bbb.sxryk.cn

deque(maxlen=10)
来源：http://mra.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://run.shzxlz.cn

defaultdict(list)
来源：http://bkx.jyoumei.cn

[U15] Py：高精度计时
来源：http://uvl.bjfxy.top

t = time.perf_counter()
来源：http://ybl.bbcook.cn

[U16] Py：命令行参数解析
来源：http://zwr.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mnd.jianghu66.top

[U17] Py：初始化日志
来源：http://yjo.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://rqe.havefunace.top

[U18] Py：预编译正则
来源：http://raw.hfpthk.cn

pat = re.compile(r"\d+")
来源：http://rnq.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://nmo.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ylp.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://dzy.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://rzs.zhixingplan.top


<!-- 参考信息 -->