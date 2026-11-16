代发 wailian999

S. C / C++ 专题
来源：http://zfe.gogol.net.cn

================================================================================
来源：http://jsc.aizwys.cn

[S01] C：Hello World
来源：http://dzk.zhaomingkeji.xyz

#include <stdio.h>
来源：http://vhv.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://msj.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://txb.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://ruh.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://fwp.nanxinkj.top

int x; scanf("%d", &x);
来源：http://sye.yvedp.cn

[S04] C：字符串复制
来源：http://ezf.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://ptk.sysykeji.top

[S05] C：字符串长度
来源：http://pqj.cqqwz.cn

strlen(s)
来源：http://hxf.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://tfk.yvedp.cn

strcmp(a, b) == 0
来源：http://fnk.cheryme.top

[S07] C：数组遍历求和
来源：http://uta.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zvx.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://pme.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wfp.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://sla.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lxw.xylfe.cn

[S10] C：指针与解引用
来源：http://rgw.fehbvm.com

int *p = &a;  *p = 5;
来源：http://mid.yanxiufei.cn

[S11] C：逐行读文件
来源：http://mse.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://dyj.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gxf.yonumen.top

fclose(f);
来源：http://qnm.iojbl.cn

[S12] C：写文件
来源：http://rrp.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://miu.zhoulong.xyz

[S13] C：宏定义
来源：http://tzm.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jab.tian-w.cn

[S14] C：枚举
来源：http://yvs.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://zke.ctjpmb.com

[S15] C：类型转换
来源：http://bex.zdbjq.cn

(double) a / b
来源：http://qqu.sweek.top

[S16] C：位操作置位
来源：http://ufu.hesvh.cn

x |= (1 << 3);
来源：http://lcm.yvedp.cn

[S17] C：安全拼接字符串
来源：http://ljd.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://viq.meibo888.top

[S18] C：命令行参数
来源：http://tic.guannengcc.top

int main(int argc, char **argv)
来源：http://drx.jinqigfzy.top

[S19] C：快速排序
来源：http://sis.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://feq.yj202588.top

[S20] C：二分查找
来源：http://cqu.havefunace.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zfv.daria6918.cn

[S21] C：字符类别判断
来源：http://sti.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://roq.yfazqb.com

[S22] C：字符串转数字
来源：http://qkh.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://dod.ybcxt.top

[S23] C：随机数
来源：http://zht.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mpg.hnxiangtu.top

[S24] C：获取本地时间
来源：http://qgg.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wke.yj20258.top

[S25] C：内存拷贝
来源：http://tpa.chenlongwang.top

memcpy(dst, src, n);
来源：http://wns.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://avq.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://ovf.chenlongwang.top

[S27] C：定义常量
来源：http://naq.jlsjyb.cn

const double PI = 3.14159;
来源：http://srb.ehwqpu.com

[S28] C：静态变量
来源：http://asq.mhx1999.top

static int counter = 0;
来源：http://gkg.jlsjyb.cn

[S29] C：变参函数
来源：http://ufj.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ngn.jianghu66.top

[S30] C：头文件保护
来源：http://shb.jqgufenzy.top

#ifndef X_H
来源：http://zsy.haohaochexian.top

#define X_H
来源：http://vur.pycfn.com

#endif
来源：http://xtk.feifeiyinyue.top

[S31] C++：Hello World
来源：http://guw.hesvh.cn

#include <iostream>
来源：http://tra.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://nha.nwbrower.top

[S32] C++：字符串
来源：http://egm.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://tpi.gzhubu.top

[S33] C++：vector 增删
来源：http://fwa.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://inx.yj202588.top

[S34] C++：遍历 vector
来源：http://feh.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://axm.xuetiantiany.cn

[S35] C++：map
来源：http://coe.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vbn.sufxvd.cn

[S36] C++：unordered_map
来源：http://ief.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fkt.yvedp.cn

[S37] C++：set
来源：http://wnz.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cyi.52xcode.cn

[S38] C++：排序
来源：http://fal.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://wpe.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://htu.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oes.daxiang520.top

[S40] C++：查找元素
来源：http://zob.hfpthk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://veo.epnwcf.com

[S41] C++：类与构造函数
来源：http://msf.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vch.xinyue.icu

[S42] C++：继承与虚函数
来源：http://qxu.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://hge.yuxming.cn

[S43] C++：智能指针
来源：http://pju.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://fjq.meibo888.top

[S44] C++：引用传参
来源：http://anq.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://waz.bbcook.cn

[S45] C++：lambda
来源：http://qgs.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wrw.ydjk.org.cn

[S46] C++：函数模板
来源：http://iwj.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pae.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://vzb.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nsf.hywenlv.cn

[S48] C++：逐行读文件
来源：http://mlb.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://qha.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://ets.xuetiantiany.cn

[S49] C++：写文件
来源：http://oyj.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yfd.zhengqikj.top

[S50] C++：格式化数字
来源：http://peg.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fqv.zycfv.cn

[S51] C++：显式类型转换
来源：http://rvq.jlsjyb.cn

static_cast<double>(a) / b
来源：http://hvy.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://shk.cucudq.cn

int size() const noexcept { return n_; }
来源：http://vhf.cheryme.top

[S53] C++：移动语义
来源：http://nlv.birdmap.top

std::vector<int> w = std::move(v);
来源：http://ehg.chenzaomai.com

[S54] C++：异常处理
来源：http://iny.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vlk.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://nij.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cve.cdnleiting.top

[S56] C++：optional
来源：http://kbu.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kne.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://kdo.svipenyu.cn

constexpr int N = 10;
来源：http://zkb.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://lbi.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://uyo.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://uel.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qfg.tarul.cn

[S60] C++：遍历并删除元素
来源：http://tjt.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mzn.hcnkem.com

================================================================================
来源：http://nky.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sqw.aibaodan.cn

================================================================================
来源：http://poo.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://aqw.ehwqpu.com

println("Hello")
来源：http://dkj.zycfv.cn

[T02] Kotlin：变量
来源：http://wqr.zhongyouzk.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ywr.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://ass.cdnleiting.top

"值: $b"
来源：http://bpa.c1oappe.top

[T04] Kotlin：空安全
来源：http://utv.tanke756.top

val n: String? = null;  n?.length
来源：http://xtg.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://mgp.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://upw.yj202588.top

[T06] Kotlin：集合映射
来源：http://cdz.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ywr.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://pxi.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xra.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://cmx.ivvv.top

data class User(val name: String, val age: Int)
来源：http://hao.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://yre.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://lwc.hammf.cn

[T10] Kotlin：默认参数
来源：http://xaw.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mqo.zhongyouzk.top

[T11] Kotlin：协程
来源：http://vxr.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zqx.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://xbd.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://rwc.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://pim.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://ehi.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://bzh.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://swc.jyoumei.cn

[T15] Kotlin：接口
来源：http://lfi.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://swb.daxiang520.top

[T16] Swift：Hello World
来源：http://xax.ppjwa.cn

print("Hello")
来源：http://taf.svipenyu.cn

[T17] Swift：变量与常量
来源：http://pmi.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://prc.nanxinkj.top

[T18] Swift：字符串插值
来源：http://gex.yvedp.cn

"值: \(b)"
来源：http://gst.gzhubu.top

[T19] Swift：可选绑定
来源：http://azn.ppjwa.cn

if let n = opt { print(n) }
来源：http://krr.cqqwz.cn

[T20] Swift：数组操作
来源：http://tds.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zzt.ctjpmb.com

[T21] Swift：遍历
来源：http://ayr.gotoacloud.top

for x in a { print(x) }
来源：http://pyw.wangdashe.top

[T22] Swift：字典
来源：http://bai.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://npm.zhiwuduotai.top

[T23] Swift：函数
来源：http://thl.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bng.52xcode.cn

[T24] Swift：闭包
来源：http://pao.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ugk.zhoulong.xyz

[T25] Swift：结构体
来源：http://kbp.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://mek.gaohongyu789.top

[T26] Swift：类与重写
来源：http://jos.sxryk.cn

class A: Base { override func f() {} }
来源：http://lro.epnwcf.com

[T27] Swift：错误处理
来源：http://hhy.xziqi.cn

do { try f() } catch { print(error) }
来源：http://wtc.hywenlv.cn

[T28] Swift：枚举
来源：http://diy.c1oappe.top

enum Color { case red, green }
来源：http://ioz.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://pvr.sysykeji.top

guard let x = opt else { return }
来源：http://ubq.cashguo.top

[T30] Swift：协议
来源：http://wth.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://phj.9152youxi.cn

[T31] Lua：Hello World
来源：http://jjj.sysykeji.top

print("Hello")
来源：http://msz.yj20258888.top

[T32] Lua：局部变量
来源：http://nft.yongpay.top

local a = 1
来源：http://qal.uphjek.com

[T33] Lua：表（数组）
来源：http://kws.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pxo.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://wrg.yvedp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nfz.gotoacloud.top

[T35] Lua：字典表
来源：http://dpv.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://yqp.feifeiyinyue.top

[T36] Lua：函数
来源：http://jxb.yangfankeji.com

function add(a, b) return a + b end
来源：http://qbd.sysykeji.top

[T37] Lua：字符串拼接
来源：http://zeg.gzhubu.top

"a" .. "b"
来源：http://crj.ctjpmb.com

[T38] Lua：条件
来源：http://akw.fengsongda.top

if x > 0 then print("正") end
来源：http://zue.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://lkj.vqdsnc.cn

string.find(s, "%d+")
来源：http://tfg.bbcook.cn

[T40] Lua：元表
来源：http://jga.sweek.top

setmetatable({}, { __index = base })
来源：http://srs.zdqjudy.top

[T41] Perl：Hello World
来源：http://ibd.guannengcc.top

print "Hello\n";
来源：http://jab.xziqi.cn

[T42] Perl：变量类型
来源：http://cwa.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hhy.vehdjk.com

[T43] Perl：字符串插值
来源：http://cms.feifeiyinyue.top

"值: $a"
来源：http://lpt.cashguo.top

[T44] Perl：条件
来源：http://mfo.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://icv.gotoacloud.top

[T45] Perl：数组遍历
来源：http://dgg.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://fsz.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://hpk.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pvg.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://ccz.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ptb.wangdashe.top

[T48] Perl：正则替换
来源：http://cex.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://jds.yueranfly.top

[T49] Perl：函数
来源：http://ppm.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jeb.hammf.cn

[T50] Perl：逐行读文件
来源：http://hre.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lxt.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://teq.nanxuanxn.top

[T51] Scala：Hello World
来源：http://fng.shuidangran.top

println("Hello")
来源：http://euf.bbcook.cn

[T52] Scala：变量
来源：http://vwr.smart0.xyz

val a = 1;  var b = 2
来源：http://eem.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://krn.wangdashe.top

s"值: $b"
来源：http://mds.xuetiantiany.cn

[T54] Scala：集合映射
来源：http://uec.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://ldr.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://dfa.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xjr.hammf.cn

[T56] Scala：样例类
来源：http://duj.316326.xyz

case class User(name: String, age: Int)
来源：http://qdx.aibaodan.cn

[T57] Scala：模式匹配
来源：http://mzo.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dru.hammf.cn

[T58] Scala：函数定义
来源：http://qtg.wangdashe.top

def add(a: Int, b: Int): Int = a + b
来源：http://rta.sweek.top

[T59] Scala：循环
来源：http://lpj.haohaochexian.top

for (i <- 1 to 10) println(i)
来源：http://prf.zhongyouzk.top

[T60] Scala：折叠
来源：http://ren.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kwd.guannengcc.top

================================================================================
来源：http://bqx.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pfx.shuidangran.top

================================================================================
来源：http://ksk.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://hvn.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tod.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://lqj.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mat.sjlbkw.cn

[U03] Py：加载 .env 配置
来源：http://jvu.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ize.xinyue.icu

[U04] Py：变量调试打印
来源：http://qjk.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://flr.gaohongyu789.top

[U05] Py：列表去重且保序
来源：http://qfa.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://sdn.haohaochexian.top

[U06] Py：合并两个字典
来源：http://ser.yangfankeji.com

{**a, **b}
来源：http://uqp.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://ulg.yvedp.cn

{v: k for k, v in d.items()}
来源：http://jno.iojbl.cn

[U08] Py：展平二维列表
来源：http://biw.ctjpmb.com

[y for x in nested for y in x]
来源：http://jku.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://kjo.shangyingyoupin.top

max(d, key=d.get)
来源：http://fjq.bbcook.cn

[U10] Py：按值排序字典
来源：http://olr.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qgx.havefunace.top

[U11] Py：生成器表达式
来源：http://ncr.fzhhl.top

(x * 2 for x in arr)
来源：http://tqy.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://mli.wangdashe.top

Counter(arr).most_common(3)
来源：http://sqs.jianghu66.top

[U13] Py：固定长度队列
来源：http://bbp.zhiwuduotai.top

deque(maxlen=10)
来源：http://duf.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://nuv.cashguo.top

defaultdict(list)
来源：http://ldo.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://vgd.zycfv.cn

t = time.perf_counter()
来源：http://dmf.zycfv.cn

[U16] Py：命令行参数解析
来源：http://lky.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bju.ivvv.top

[U17] Py：初始化日志
来源：http://vco.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://sfr.bbcook.cn

[U18] Py：预编译正则
来源：http://gok.hesvh.cn

pat = re.compile(r"\d+")
来源：http://odo.gotoacloud.top

[U19] Py：正则替换带回调
来源：http://gur.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://voj.chenzaomai.com

[U20] Py：缓存函数结果
来源：http://rrs.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://dqp.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://lgm.daria6918.cn

@contextlib.contextmanager
来源：http://ivx.gogol.net.cn

[U22] Py：矩阵转置
来源：http://syd.wangshuangyany.cn

list(zip(*m))
来源：http://zwp.yangfankeji.com


<!-- 参考信息 -->