代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vee.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://gfv.haohaochexian.top

time ./run.sh
来源：http://dtn.zycfv.cn

================================================================================
来源：http://qhm.gotoacloud.top

S. C / C++ 专题
来源：http://viv.xuetiantiany.cn

================================================================================
来源：http://gog.sysykeji.top

[S01] C：Hello World
来源：http://efa.jianghu66.top

#include <stdio.h>
来源：http://fnq.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fad.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://cuh.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://ezo.daria6918.cn

[S03] C：读入整数
来源：http://zka.bbcook.cn

int x; scanf("%d", &x);
来源：http://ytl.52xcode.cn

[S04] C：字符串复制
来源：http://rzr.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://ycl.hesvh.cn

[S05] C：字符串长度
来源：http://tml.yueranfly.top

strlen(s)
来源：http://vzy.xuanzx.com

[S06] C：字符串比较
来源：http://opj.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://gzk.chenzaomai.com

[S07] C：数组遍历求和
来源：http://hrs.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ynv.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://drq.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wno.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://kft.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://frx.sjlbkw.cn

[S10] C：指针与解引用
来源：http://dau.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://cki.hnqzz.top

[S11] C：逐行读文件
来源：http://nqu.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://zay.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mwu.fehbvm.com

fclose(f);
来源：http://drf.0kj1m.cn

[S12] C：写文件
来源：http://koh.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cxw.hammf.cn

[S13] C：宏定义
来源：http://ndy.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ohv.xinyue.icu

[S14] C：枚举
来源：http://mxa.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://elb.tian-w.cn

[S15] C：类型转换
来源：http://rgq.yj20258.top

(double) a / b
来源：http://qiq.yangfankeji.com

[S16] C：位操作置位
来源：http://wyd.vehdjk.com

x |= (1 << 3);
来源：http://miu.uphjek.com

[S17] C：安全拼接字符串
来源：http://pgq.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qpj.zdbjq.cn

[S18] C：命令行参数
来源：http://cvy.tianlin.xyz

int main(int argc, char **argv)
来源：http://wys.andypj.xyz

[S19] C：快速排序
来源：http://uis.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://eai.shanyushiyangtech.top

[S20] C：二分查找
来源：http://iyu.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pqx.jyoumei.cn

[S21] C：字符类别判断
来源：http://khc.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uqj.hysaishi.cn

[S22] C：字符串转数字
来源：http://xsp.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iut.andypj.xyz

[S23] C：随机数
来源：http://ppk.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hxi.jqgfzy.top

[S24] C：获取本地时间
来源：http://wje.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bou.ivvv.top

[S25] C：内存拷贝
来源：http://mmq.sweek.top

memcpy(dst, src, n);
来源：http://xqn.pycfn.com

[S26] C：内存清零
来源：http://ctl.wangdashe.top

memset(a, 0, sizeof a);
来源：http://ezb.yangfankeji.com

[S27] C：定义常量
来源：http://lgm.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://dzn.wangdashe.top

[S28] C：静态变量
来源：http://org.fehbvm.com

static int counter = 0;
来源：http://mft.chenzaomai.com

[S29] C：变参函数
来源：http://vwv.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fyi.cdnleiting.top

[S30] C：头文件保护
来源：http://ggr.quarkkingdee.top

#ifndef X_H
来源：http://gkd.yj20258.top

#define X_H
来源：http://ggn.hysaishi.cn

#endif
来源：http://aoe.nanxinkj.top

[S31] C++：Hello World
来源：http://cdf.sxryk.cn

#include <iostream>
来源：http://gzf.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://jfj.guowangkeji.top

[S32] C++：字符串
来源：http://eim.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://xef.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://iod.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gbw.cqqwz.cn

[S34] C++：遍历 vector
来源：http://aqq.hnxiangtu.top

for (auto &x : v) { std::cout << x; }
来源：http://teh.haohaochexian.top

[S35] C++：map
来源：http://yrp.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cgr.chenzaomai.com

[S36] C++：unordered_map
来源：http://ssj.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xpx.hnqzz.top

[S37] C++：set
来源：http://owz.fengsongda.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://llt.0kj1m.cn

[S38] C++：排序
来源：http://oqd.yj202588.top

std::sort(v.begin(), v.end());
来源：http://lhy.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://nqb.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xcg.cdnleiting.top

[S40] C++：查找元素
来源：http://zld.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qcg.ivvv.top

[S41] C++：类与构造函数
来源：http://kaj.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pge.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://alv.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://zel.pengpengdd.cyou

[S43] C++：智能指针
来源：http://ogc.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://ndc.sweek.top

[S44] C++：引用传参
来源：http://iyr.hfpthk.cn

void inc(int &x) { ++x; }
来源：http://ypm.xziqi.cn

[S45] C++：lambda
来源：http://kzg.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://vdd.tarul.cn

[S46] C++：函数模板
来源：http://ujt.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://esz.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://eyf.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nqz.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://hkd.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fim.epnwcf.com

while (std::getline(in, line)) { }
来源：http://wve.hfpthk.cn

[S49] C++：写文件
来源：http://nri.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vxz.guannengcc.top

[S50] C++：格式化数字
来源：http://yel.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://csw.zdqjudy.top

[S51] C++：显式类型转换
来源：http://eid.jianghu66.top

static_cast<double>(a) / b
来源：http://slf.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://nuu.tian-w.cn

int size() const noexcept { return n_; }
来源：http://uey.yueranfly.top

[S53] C++：移动语义
来源：http://wpf.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://hpk.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://tiu.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://teg.zycfv.cn

[S55] C++：结构化绑定
来源：http://utr.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nls.nanxinkj.top

[S56] C++：optional
来源：http://lop.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://trb.quarkkingdee.top

[S57] C++：编译期常量
来源：http://gcm.hnqzz.top

constexpr int N = 10;
来源：http://bgj.hnqzz.top

[S58] C++：命名空间
来源：http://lgw.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://fvs.ppjwa.cn

[S59] C++：静态断言
来源：http://iov.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yao.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://ipn.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://akt.ctjpmb.com

================================================================================
来源：http://cqr.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xkr.bjfxy.top

================================================================================
来源：http://kcf.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://luy.sufxvd.cn

println("Hello")
来源：http://tvi.chenzaomai.com

[T02] Kotlin：变量
来源：http://ffl.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yqm.yj202588.top

[T03] Kotlin：字符串模板
来源：http://har.xuanzx.com

"值: $b"
来源：http://fwg.wangdashe.top

[T04] Kotlin：空安全
来源：http://bsi.xziqi.cn

val n: String? = null;  n?.length
来源：http://gfh.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://xhi.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tuq.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://wok.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zsa.yj20258.top

[T07] Kotlin：集合过滤
来源：http://iez.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xum.nwbrower.top

[T08] Kotlin：数据类
来源：http://rif.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://fep.meibo888.top

[T09] Kotlin：扩展函数
来源：http://bjl.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://jpn.316326.xyz

[T10] Kotlin：默认参数
来源：http://nhk.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mdy.zhixingplan.top

[T11] Kotlin：协程
来源：http://kwv.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zgm.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://qez.xziqi.cn

val (a, b) = Pair(1, 2)
来源：http://fng.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://bwx.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://uxr.cheryme.top

[T14] Kotlin：循环
来源：http://adl.52xcode.cn

for (i in 1..10) println(i)
来源：http://men.316326.xyz

[T15] Kotlin：接口
来源：http://hce.guannengcc.top

interface Shape { fun area(): Double }
来源：http://alx.tian-w.cn

[T16] Swift：Hello World
来源：http://ffm.yfazqb.com

print("Hello")
来源：http://dyz.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://ptg.haohaochexian.top

var a = 1;  let b = 2
来源：http://yka.shuidangran.top

[T18] Swift：字符串插值
来源：http://cfl.zhongyouzk.top

"值: \(b)"
来源：http://tfc.cqqwz.cn

[T19] Swift：可选绑定
来源：http://bbh.iojbl.cn

if let n = opt { print(n) }
来源：http://vid.daria6918.cn

[T20] Swift：数组操作
来源：http://gvz.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://qby.zdbjq.cn

[T21] Swift：遍历
来源：http://oyd.quarkkingdee.top

for x in a { print(x) }
来源：http://wsv.zhengqikj.top

[T22] Swift：字典
来源：http://gdy.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://brp.fktsv.cn

[T23] Swift：函数
来源：http://nee.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ajr.aizwys.cn

[T24] Swift：闭包
来源：http://tzd.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://rhq.52xcode.cn

[T25] Swift：结构体
来源：http://lxi.havefunace.top

struct P { var x: Int }
来源：http://uze.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://xrk.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://bss.sjlbkw.cn

[T27] Swift：错误处理
来源：http://gmz.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://tyf.ywan-chungtsiang.top

[T28] Swift：枚举
来源：http://pjn.yanxiufei.cn

enum Color { case red, green }
来源：http://vyz.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://xob.chenjidiqi.icu

guard let x = opt else { return }
来源：http://czx.yongpay.top

[T30] Swift：协议
来源：http://tas.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://cpy.sweek.top

[T31] Lua：Hello World
来源：http://pox.andypj.xyz

print("Hello")
来源：http://zzz.aibaodan.cn

[T32] Lua：局部变量
来源：http://dxo.sxryk.cn

local a = 1
来源：http://hig.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://ykd.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ldh.zycfv.cn

[T34] Lua：遍历表
来源：http://vve.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://esd.hywenlv.cn

[T35] Lua：字典表
来源：http://wzj.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://odz.guowangkeji.top

[T36] Lua：函数
来源：http://ihi.quarkkingdee.top

function add(a, b) return a + b end
来源：http://wnu.sweek.top

[T37] Lua：字符串拼接
来源：http://dax.kuanghao11.cn

"a" .. "b"
来源：http://ini.xinyue.icu

[T38] Lua：条件
来源：http://qgg.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://ejr.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://kyi.hcnkem.com

string.find(s, "%d+")
来源：http://sec.ppjwa.cn

[T40] Lua：元表
来源：http://pdg.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://ley.guowangkeji.top

[T41] Perl：Hello World
来源：http://cix.yuxming.cn

print "Hello\n";
来源：http://pwp.aibaodan.cn

[T42] Perl：变量类型
来源：http://qkr.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dpc.sxryk.cn

[T43] Perl：字符串插值
来源：http://imy.havefunace.top

"值: $a"
来源：http://stk.zhixingplan.top

[T44] Perl：条件
来源：http://jes.meibo888.top

if ($a > 0) { print "正"; }
来源：http://zac.jianghu66.top

[T45] Perl：数组遍历
来源：http://pjh.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://wqs.cheryme.top

[T46] Perl：哈希操作
来源：http://bwt.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jhw.sysykeji.top

[T47] Perl：正则捕获
来源：http://trf.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hph.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://cqv.iojbl.cn

$s =~ s/old/new/g;
来源：http://rcb.meibo888.top

[T49] Perl：函数
来源：http://xos.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xat.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://kfu.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bwx.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://yvs.sufxvd.cn

[T51] Scala：Hello World
来源：http://rky.52xcode.cn

println("Hello")
来源：http://zke.gogol.net.cn

[T52] Scala：变量
来源：http://nwr.sxryk.cn

val a = 1;  var b = 2
来源：http://iuu.guannengcc.top

[T53] Scala：字符串插值
来源：http://yzc.hfpthk.cn

s"值: $b"
来源：http://buy.hfpthk.cn

[T54] Scala：集合映射
来源：http://gtf.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://nao.daria6918.cn

[T55] Scala：集合过滤
来源：http://uid.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://anj.chenzaomai.com

[T56] Scala：样例类
来源：http://ziu.wangdashe.top

case class User(name: String, age: Int)
来源：http://rsm.svipenyu.cn

[T57] Scala：模式匹配
来源：http://ofw.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://obn.0kj1m.cn

[T58] Scala：函数定义
来源：http://owf.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://qlq.guannengcc.top

[T59] Scala：循环
来源：http://jcl.jinqigfzy.top

for (i <- 1 to 10) println(i)
来源：http://zni.aibaodan.cn

[T60] Scala：折叠
来源：http://pzm.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jjn.sweek.top

================================================================================
来源：http://lrg.zhoulong.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sce.iojbl.cn

================================================================================
来源：http://wqs.gaohongyu789.top

[U01] Py：创建虚拟环境
来源：http://yey.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://fra.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://ntd.hysaishi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zgk.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://out.snrcjt.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ltn.fzhhl.top

[U04] Py：变量调试打印
来源：http://ymh.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ceu.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://onw.ybcxt.top

list(dict.fromkeys(arr))
来源：http://ecx.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://cxa.wangdashe.top

{**a, **b}
来源：http://qmi.zycfv.cn

[U07] Py：反转字典键值
来源：http://ita.0kj1m.cn

{v: k for k, v in d.items()}
来源：http://cjn.yueranfly.top

[U08] Py：展平二维列表
来源：http://nqu.dianchejie.cn

[y for x in nested for y in x]
来源：http://tur.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://hzt.zdbjq.cn

max(d, key=d.get)
来源：http://pkv.ybcxt.top

[U10] Py：按值排序字典
来源：http://yfo.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://guc.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://lvu.tanke756.top

(x * 2 for x in arr)
来源：http://hsx.hcnkem.com

[U12] Py：取出现最多的 3 个元素
来源：http://lbz.aizwys.cn

Counter(arr).most_common(3)
来源：http://wxy.yongpay.top

[U13] Py：固定长度队列
来源：http://iyi.epnwcf.com

deque(maxlen=10)
来源：http://bqq.zycfv.cn

[U14] Py：分组收集到列表
来源：http://tub.gogol.net.cn

defaultdict(list)
来源：http://bba.yj20258.top

[U15] Py：高精度计时
来源：http://mfo.9152youxi.cn

t = time.perf_counter()
来源：http://ezz.tanke756.top

[U16] Py：命令行参数解析
来源：http://cfn.ivvv.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gwq.shzxlz.cn

[U17] Py：初始化日志
来源：http://elw.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://nnr.nanxinkj.top

[U18] Py：预编译正则
来源：http://pzp.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://iid.gzhubu.top

[U19] Py：正则替换带回调
来源：http://hgi.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qxu.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://gru.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://ptf.yfazqb.com


<!-- 参考信息 -->