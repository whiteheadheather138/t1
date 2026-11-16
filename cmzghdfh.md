代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://age.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://cno.mhx1999.top

time ./run.sh
来源：http://bgf.ybcxt.top

================================================================================
来源：http://vkb.0kj1m.cn

S. C / C++ 专题
来源：http://uyn.pengpengdd.cyou

================================================================================
来源：http://iym.hywenlv.cn

[S01] C：Hello World
来源：http://nmy.9152youxi.cn

#include <stdio.h>
来源：http://jfd.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hwr.birdmap.top

[S02] C：变量与格式化输出
来源：http://mtb.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://jhq.zdqjudy.top

[S03] C：读入整数
来源：http://eri.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://rip.tarul.cn

[S04] C：字符串复制
来源：http://xhj.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://rsm.nanxuanxn.top

[S05] C：字符串长度
来源：http://tyu.zhixingplan.top

strlen(s)
来源：http://ljc.haohaochexian.top

[S06] C：字符串比较
来源：http://vir.ydjk.org.cn

strcmp(a, b) == 0
来源：http://xpu.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://ofl.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sbq.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://bgx.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qja.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://ckc.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hun.tarul.cn

[S10] C：指针与解引用
来源：http://wtw.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://pcj.yfazqb.com

[S11] C：逐行读文件
来源：http://zve.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://qpb.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rdy.0kj1m.cn

fclose(f);
来源：http://uwg.hongshengwenyu.top

[S12] C：写文件
来源：http://xvl.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mtw.316326.xyz

[S13] C：宏定义
来源：http://cek.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eej.ctjpmb.com

[S14] C：枚举
来源：http://dmb.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://fam.redwolf501.top

[S15] C：类型转换
来源：http://pez.9152youxi.cn

(double) a / b
来源：http://fvo.jinqigufen.top

[S16] C：位操作置位
来源：http://gyh.fktsv.cn

x |= (1 << 3);
来源：http://ffy.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://yei.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cbj.0kj1m.cn

[S18] C：命令行参数
来源：http://yzu.havefunace.top

int main(int argc, char **argv)
来源：http://hhm.0kj1m.cn

[S19] C：快速排序
来源：http://ube.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://fwj.bjfxy.top

[S20] C：二分查找
来源：http://ydc.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ycp.ppjwa.cn

[S21] C：字符类别判断
来源：http://wzp.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zoi.chenlongwang.top

[S22] C：字符串转数字
来源：http://xtt.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://vaq.shuidangran.top

[S23] C：随机数
来源：http://ess.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rba.hcnkem.com

[S24] C：获取本地时间
来源：http://zri.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vuj.haohaochexian.top

[S25] C：内存拷贝
来源：http://whr.dashuyun.cn

memcpy(dst, src, n);
来源：http://pcz.yvedp.cn

[S26] C：内存清零
来源：http://vlw.gzhubu.top

memset(a, 0, sizeof a);
来源：http://klt.jlsjyb.cn

[S27] C：定义常量
来源：http://iee.smart0.xyz

const double PI = 3.14159;
来源：http://nhy.sxryk.cn

[S28] C：静态变量
来源：http://iab.zhengqikj.top

static int counter = 0;
来源：http://fgs.aizwys.cn

[S29] C：变参函数
来源：http://cxn.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dtm.yvedp.cn

[S30] C：头文件保护
来源：http://zzj.yanxiufei.cn

#ifndef X_H
来源：http://twx.hfpthk.cn

#define X_H
来源：http://mef.jyoumei.cn

#endif
来源：http://uho.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://dfk.pycfn.com

#include <iostream>
来源：http://dex.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://btn.tian-w.cn

[S32] C++：字符串
来源：http://zug.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://qgc.0kj1m.cn

[S33] C++：vector 增删
来源：http://bih.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qkd.vehdjk.com

[S34] C++：遍历 vector
来源：http://sab.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://wjb.gaohongyu789.top

[S35] C++：map
来源：http://ydv.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jxk.aibaodan.cn

[S36] C++：unordered_map
来源：http://vpy.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tbk.chenjidiqi.icu

[S37] C++：set
来源：http://xbu.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uto.guowangkeji.top

[S38] C++：排序
来源：http://xsu.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://oeb.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://eqj.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mbn.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://nod.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lzm.fktsv.cn

[S41] C++：类与构造函数
来源：http://zcj.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vtn.tarul.cn

[S42] C++：继承与虚函数
来源：http://elw.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://hps.bjfxy.top

[S43] C++：智能指针
来源：http://zfb.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://mnr.quarkkingdee.top

[S44] C++：引用传参
来源：http://ofv.yvedp.cn

void inc(int &x) { ++x; }
来源：http://qre.cheryme.top

[S45] C++：lambda
来源：http://frc.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mug.tanke756.top

[S46] C++：函数模板
来源：http://fbr.pycfn.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aqt.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://yzu.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ovd.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://kai.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://vvj.yj202588.top

while (std::getline(in, line)) { }
来源：http://sxb.0kj1m.cn

[S49] C++：写文件
来源：http://kgg.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fkm.ydzc1.top

[S50] C++：格式化数字
来源：http://bky.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gal.snrcjt.cn

[S51] C++：显式类型转换
来源：http://nco.cucudq.cn

static_cast<double>(a) / b
来源：http://nsf.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://mhb.ybcxt.top

int size() const noexcept { return n_; }
来源：http://xfz.wangshuangyany.cn

[S53] C++：移动语义
来源：http://dik.meibo888.top

std::vector<int> w = std::move(v);
来源：http://pll.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://buu.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ise.smart0.xyz

[S55] C++：结构化绑定
来源：http://pua.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ktq.bbcook.cn

[S56] C++：optional
来源：http://hiw.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oto.jinqigufen.top

[S57] C++：编译期常量
来源：http://fmn.yongpay.top

constexpr int N = 10;
来源：http://gdv.ehwqpu.com

[S58] C++：命名空间
来源：http://gne.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://twi.guowangkeji.top

[S59] C++：静态断言
来源：http://dep.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ued.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://bri.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://anp.xziqi.cn

================================================================================
来源：http://dkd.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ths.ctjpmb.com

================================================================================
来源：http://ucv.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://pcn.nwbrower.top

println("Hello")
来源：http://tlm.sweek.top

[T02] Kotlin：变量
来源：http://bfh.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qnj.yangfankeji.com

[T03] Kotlin：字符串模板
来源：http://jbi.aizwys.cn

"值: $b"
来源：http://rcr.pycfn.com

[T04] Kotlin：空安全
来源：http://cij.yongpay.top

val n: String? = null;  n?.length
来源：http://bwj.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://zkt.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mnf.hammf.cn

[T06] Kotlin：集合映射
来源：http://nev.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cyv.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://wmq.tian-w.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hfb.gzhubu.top

[T08] Kotlin：数据类
来源：http://tdx.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://qkz.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://kto.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://kdp.hcnkem.com

[T10] Kotlin：默认参数
来源：http://dyc.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://egr.yueranfly.top

[T11] Kotlin：协程
来源：http://ask.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://dlw.jianghu66.top

[T12] Kotlin：解构声明
来源：http://knt.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://bcg.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://cmd.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://wgg.bbcook.cn

[T14] Kotlin：循环
来源：http://umt.zdbjq.cn

for (i in 1..10) println(i)
来源：http://eqh.yj202588.top

[T15] Kotlin：接口
来源：http://dbv.aizwys.cn

interface Shape { fun area(): Double }
来源：http://gla.meibo888.top

[T16] Swift：Hello World
来源：http://ifi.daxiang520.top

print("Hello")
来源：http://wge.yj20258.top

[T17] Swift：变量与常量
来源：http://cwu.svipenyu.cn

var a = 1;  let b = 2
来源：http://spi.jiagoushi.top

[T18] Swift：字符串插值
来源：http://fig.jinyuanbaomall.cn

"值: \(b)"
来源：http://pwv.sufxvd.cn

[T19] Swift：可选绑定
来源：http://eeo.ydjk.org.cn

if let n = opt { print(n) }
来源：http://exw.yuanzhike.top

[T20] Swift：数组操作
来源：http://xbv.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://anj.vehdjk.com

[T21] Swift：遍历
来源：http://bsi.sjlbkw.cn

for x in a { print(x) }
来源：http://jgf.pycfn.com

[T22] Swift：字典
来源：http://tcr.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://enx.yj202588.top

[T23] Swift：函数
来源：http://erg.cdnleiting.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mri.ybcxt.top

[T24] Swift：闭包
来源：http://lsb.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gqs.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://xwd.yanxiufei.cn

struct P { var x: Int }
来源：http://yru.yj20258888.top

[T26] Swift：类与重写
来源：http://sus.haohaochexian.top

class A: Base { override func f() {} }
来源：http://hbd.vqdsnc.cn

[T27] Swift：错误处理
来源：http://fqx.daria6918.cn

do { try f() } catch { print(error) }
来源：http://jqd.chenlongwang.top

[T28] Swift：枚举
来源：http://clc.sweek.top

enum Color { case red, green }
来源：http://wdf.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://cfl.shzxlz.cn

guard let x = opt else { return }
来源：http://zol.sxryk.cn

[T30] Swift：协议
来源：http://trp.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://efv.nwbrower.top

[T31] Lua：Hello World
来源：http://soh.yuxming.cn

print("Hello")
来源：http://hcr.zhengqikj.top

[T32] Lua：局部变量
来源：http://bjp.0kj1m.cn

local a = 1
来源：http://wuo.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://xho.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qwx.tanke756.top

[T34] Lua：遍历表
来源：http://lxi.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lrz.yj20258.top

[T35] Lua：字典表
来源：http://ttz.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://klt.yongpay.top

[T36] Lua：函数
来源：http://ixq.hnqzz.top

function add(a, b) return a + b end
来源：http://ynn.yuxming.cn

[T37] Lua：字符串拼接
来源：http://khy.shanyushiyangkeji.top

"a" .. "b"
来源：http://xyj.wangshuangyany.cn

[T38] Lua：条件
来源：http://zjw.daria6918.cn

if x > 0 then print("正") end
来源：http://ger.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://hdq.0kj1m.cn

string.find(s, "%d+")
来源：http://zog.chenzaomai.com

[T40] Lua：元表
来源：http://prc.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://qzu.dashuyun.cn

[T41] Perl：Hello World
来源：http://wvy.fzhhl.top

print "Hello\n";
来源：http://tav.jinqigufen.top

[T42] Perl：变量类型
来源：http://kcl.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bsj.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://nkv.dianchejie.cn

"值: $a"
来源：http://szr.yuxming.cn

[T44] Perl：条件
来源：http://ndg.snrcjt.cn

if ($a > 0) { print "正"; }
来源：http://ekf.yvedp.cn

[T45] Perl：数组遍历
来源：http://hzz.cheryme.top

for my $x (@arr) { print $x; }
来源：http://opo.tarul.cn

[T46] Perl：哈希操作
来源：http://ntr.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://apt.bbcook.cn

[T47] Perl：正则捕获
来源：http://vpz.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://aoz.iojbl.cn

[T48] Perl：正则替换
来源：http://gom.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://ysq.vqdsnc.cn

[T49] Perl：函数
来源：http://akw.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eta.mhx1999.top

[T50] Perl：逐行读文件
来源：http://qyv.vehdjk.com

open my $fh, "<", "a.txt" or die $!;
来源：http://gin.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://ryz.bjfxy.top

[T51] Scala：Hello World
来源：http://ssi.bjfxy.top

println("Hello")
来源：http://tyg.yonumen.top

[T52] Scala：变量
来源：http://dqf.nwbrower.top

val a = 1;  var b = 2
来源：http://oez.smart0.xyz

[T53] Scala：字符串插值
来源：http://pnn.jqgfzy.top

s"值: $b"
来源：http://dcv.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://btv.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://xwy.hongshengwenyu.top

[T55] Scala：集合过滤
来源：http://jpq.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://kao.shzxlz.cn

[T56] Scala：样例类
来源：http://wxc.hnqzz.top

case class User(name: String, age: Int)
来源：http://vrc.epnwcf.com

[T57] Scala：模式匹配
来源：http://ltg.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gcf.bjfxy.top

[T58] Scala：函数定义
来源：http://wun.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://bnx.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://twe.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://ugc.dashuyun.cn

[T60] Scala：折叠
来源：http://xpu.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fms.sweek.top

================================================================================
来源：http://ees.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cgj.aizwys.cn

================================================================================
来源：http://liw.316326.xyz

[U01] Py：创建虚拟环境
来源：http://wuf.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nrl.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://ibj.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vym.jqgufenzy.top

[U03] Py：加载 .env 配置
来源：http://qpd.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://off.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://fmc.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jbb.jqgfzy.top

[U05] Py：列表去重且保序
来源：http://knd.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://qgm.xinyue.icu

[U06] Py：合并两个字典
来源：http://jvd.fehbvm.com

{**a, **b}
来源：http://osb.guannengcc.top

[U07] Py：反转字典键值
来源：http://ybs.ydzc1.top

{v: k for k, v in d.items()}
来源：http://fgb.yongpay.top

[U08] Py：展平二维列表
来源：http://ciq.ybcxt.top

[y for x in nested for y in x]
来源：http://egr.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://dwt.shangyingyoupin.top

max(d, key=d.get)
来源：http://jln.hcnkem.com

[U10] Py：按值排序字典
来源：http://lxw.ydzc1.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cdt.yfazqb.com

[U11] Py：生成器表达式
来源：http://wtp.xuanzx.com

(x * 2 for x in arr)
来源：http://tnr.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fkc.aizwys.cn

Counter(arr).most_common(3)
来源：http://tgy.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://odv.xuetiantiany.cn

deque(maxlen=10)
来源：http://lbv.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://avs.yj20258.top

defaultdict(list)
来源：http://ddo.jinqigfzy.top

[U15] Py：高精度计时
来源：http://xfk.yangfankeji.com

t = time.perf_counter()
来源：http://usz.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://qyu.gzhubu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://muz.nwbrower.top

[U17] Py：初始化日志
来源：http://yxx.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://rgh.tanke756.top

[U18] Py：预编译正则
来源：http://ixb.nwbrower.top

pat = re.compile(r"\d+")
来源：http://jdk.hysaishi.cn

[U19] Py：正则替换带回调
来源：http://bfz.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ktp.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://cxx.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://ksg.zhaomingkeji.xyz


<!-- 参考信息 -->