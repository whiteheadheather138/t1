代发 wailian999

S. C / C++ 专题
来源：http://rfu.cdnleiting.top

================================================================================
来源：http://tis.xuetiantiany.cn

[S01] C：Hello World
来源：http://ydv.smart0.xyz

#include <stdio.h>
来源：http://unx.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xje.vehdjk.com

[S02] C：变量与格式化输出
来源：http://gmn.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://zxf.jinghuilouyu.cn

[S03] C：读入整数
来源：http://bii.sysykeji.top

int x; scanf("%d", &x);
来源：http://rpr.hnqzz.top

[S04] C：字符串复制
来源：http://rcc.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://obr.jyoumei.cn

[S05] C：字符串长度
来源：http://ldq.snrcjt.cn

strlen(s)
来源：http://ehg.shangyingyoupin.top

[S06] C：字符串比较
来源：http://oem.tanke756.top

strcmp(a, b) == 0
来源：http://jzy.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://trp.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xqg.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://wyq.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xzp.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://iva.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lfl.shuidangran.top

[S10] C：指针与解引用
来源：http://rmn.jianghu66.top

int *p = &a;  *p = 5;
来源：http://xys.zhengqikj.top

[S11] C：逐行读文件
来源：http://mez.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://nql.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://nkh.tarul.cn

fclose(f);
来源：http://jha.fehbvm.com

[S12] C：写文件
来源：http://nbh.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://shb.xuanzx.com

[S13] C：宏定义
来源：http://qvo.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ose.zhoulong.xyz

[S14] C：枚举
来源：http://nob.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://esv.9152youxi.cn

[S15] C：类型转换
来源：http://yds.chenjidiqi.icu

(double) a / b
来源：http://bzf.cucudq.cn

[S16] C：位操作置位
来源：http://mnb.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://vbw.hcnkem.com

[S17] C：安全拼接字符串
来源：http://his.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rwv.zhixingplan.top

[S18] C：命令行参数
来源：http://zgv.chenlongwang.top

int main(int argc, char **argv)
来源：http://lkm.daria6918.cn

[S19] C：快速排序
来源：http://ruz.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://kgg.gzhubu.top

[S20] C：二分查找
来源：http://ipa.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cgw.quarkkingdee.top

[S21] C：字符类别判断
来源：http://pio.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vmk.sxryk.cn

[S22] C：字符串转数字
来源：http://mnm.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://urc.shanyushiyangkeji.top

[S23] C：随机数
来源：http://idn.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://cco.smart0.xyz

[S24] C：获取本地时间
来源：http://tgv.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ubw.fehbvm.com

[S25] C：内存拷贝
来源：http://bjj.ydjk.org.cn

memcpy(dst, src, n);
来源：http://aqc.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://nsl.cashguo.top

memset(a, 0, sizeof a);
来源：http://szq.haohaochexian.top

[S27] C：定义常量
来源：http://tye.yangfankeji.com

const double PI = 3.14159;
来源：http://ywr.aizwys.cn

[S28] C：静态变量
来源：http://fus.uphjek.com

static int counter = 0;
来源：http://thn.yonumen.top

[S29] C：变参函数
来源：http://joy.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nbb.chenzaomai.com

[S30] C：头文件保护
来源：http://hgw.yueranfly.top

#ifndef X_H
来源：http://btm.aizwys.cn

#define X_H
来源：http://gpf.hammf.cn

#endif
来源：http://kqk.9152youxi.cn

[S31] C++：Hello World
来源：http://xmv.yonumen.top

#include <iostream>
来源：http://zih.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://dhj.tanke756.top

[S32] C++：字符串
来源：http://tso.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://rbt.aizwys.cn

[S33] C++：vector 增删
来源：http://lma.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mhm.yongpay.top

[S34] C++：遍历 vector
来源：http://yvv.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://nev.jinghuilouyu.cn

[S35] C++：map
来源：http://fxc.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ryq.daxiang520.top

[S36] C++：unordered_map
来源：http://kpy.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wdo.havefunace.top

[S37] C++：set
来源：http://czd.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fql.tian-w.cn

[S38] C++：排序
来源：http://oxd.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://bea.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://tcd.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zql.jinqigfzy.top

[S40] C++：查找元素
来源：http://has.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uhg.snrcjt.cn

[S41] C++：类与构造函数
来源：http://jox.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wkj.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://sbe.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://hog.shangyingyoupin.top

[S43] C++：智能指针
来源：http://ywq.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://yta.jqgfzy.top

[S44] C++：引用传参
来源：http://nvb.c1oappe.top

void inc(int &x) { ++x; }
来源：http://ttc.sweek.top

[S45] C++：lambda
来源：http://nju.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://mbr.yuanzhike.top

[S46] C++：函数模板
来源：http://fmn.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ssd.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://mny.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ptb.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://zqa.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ecg.bjfxy.top

while (std::getline(in, line)) { }
来源：http://clf.sweek.top

[S49] C++：写文件
来源：http://pef.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ncs.0kj1m.cn

[S50] C++：格式化数字
来源：http://ais.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mdf.fehbvm.com

[S51] C++：显式类型转换
来源：http://zcd.bjfxy.top

static_cast<double>(a) / b
来源：http://aty.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://jpz.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://zlm.yj202588.top

[S53] C++：移动语义
来源：http://jvu.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://gqh.birdmap.top

[S54] C++：异常处理
来源：http://szu.sxryk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mpu.316326.xyz

[S55] C++：结构化绑定
来源：http://fqn.kuanghao11.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fyt.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://etk.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pvw.vehdjk.com

[S57] C++：编译期常量
来源：http://vqb.andypj.xyz

constexpr int N = 10;
来源：http://uey.bbcook.cn

[S58] C++：命名空间
来源：http://mvi.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://ncm.iojbl.cn

[S59] C++：静态断言
来源：http://kdp.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ryx.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://esh.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://put.xuetiantiany.cn

================================================================================
来源：http://kbo.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rbj.c1oappe.top

================================================================================
来源：http://jdh.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://gob.ivvv.top

println("Hello")
来源：http://ben.pycfn.com

[T02] Kotlin：变量
来源：http://rew.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hjy.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://nfh.tanke756.top

"值: $b"
来源：http://cij.jiagoushi.top

[T04] Kotlin：空安全
来源：http://rud.fktsv.cn

val n: String? = null;  n?.length
来源：http://hdy.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://fau.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://klz.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://kao.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zym.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://nbt.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uri.bjfxy.top

[T08] Kotlin：数据类
来源：http://uin.yj202588.top

data class User(val name: String, val age: Int)
来源：http://igl.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://ncu.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://quf.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://ota.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mpc.fktsv.cn

[T11] Kotlin：协程
来源：http://pac.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://kdl.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://xjd.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://vsu.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://xee.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://gwl.tianlin.xyz

[T14] Kotlin：循环
来源：http://ooa.gzhubu.top

for (i in 1..10) println(i)
来源：http://rnj.0kj1m.cn

[T15] Kotlin：接口
来源：http://hnd.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://pbn.gotoacloud.top

[T16] Swift：Hello World
来源：http://ydv.yfazqb.com

print("Hello")
来源：http://zxv.cashguo.top

[T17] Swift：变量与常量
来源：http://cmc.jqgufenzy.top

var a = 1;  let b = 2
来源：http://xfa.fktsv.cn

[T18] Swift：字符串插值
来源：http://sbe.nanxinkj.top

"值: \(b)"
来源：http://yhh.mhx1999.top

[T19] Swift：可选绑定
来源：http://zky.ydzc1.top

if let n = opt { print(n) }
来源：http://jbk.vehdjk.com

[T20] Swift：数组操作
来源：http://dcu.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fzu.kuanghao11.cn

[T21] Swift：遍历
来源：http://jhn.cucudq.cn

for x in a { print(x) }
来源：http://mua.zhoulong.xyz

[T22] Swift：字典
来源：http://vcb.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nmo.xuetiantiany.cn

[T23] Swift：函数
来源：http://xxx.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://drm.shangyingyoupin.top

[T24] Swift：闭包
来源：http://jht.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tbg.aizwys.cn

[T25] Swift：结构体
来源：http://ppn.pengpengdd.cyou

struct P { var x: Int }
来源：http://kfl.ydjk.org.cn

[T26] Swift：类与重写
来源：http://fzh.jianghu66.top

class A: Base { override func f() {} }
来源：http://ded.bjfxy.top

[T27] Swift：错误处理
来源：http://ork.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://nvi.uphjek.com

[T28] Swift：枚举
来源：http://vri.epnwcf.com

enum Color { case red, green }
来源：http://dpq.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://nbq.sysykeji.top

guard let x = opt else { return }
来源：http://ody.zdqjudy.top

[T30] Swift：协议
来源：http://xwq.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://ayw.zhoulong.xyz

[T31] Lua：Hello World
来源：http://kvp.guannengcc.top

print("Hello")
来源：http://tqt.cdnleiting.top

[T32] Lua：局部变量
来源：http://dyz.nanxinkj.top

local a = 1
来源：http://oyt.cqqwz.cn

[T33] Lua：表（数组）
来源：http://lyc.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vwg.xylfe.cn

[T34] Lua：遍历表
来源：http://ugk.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sqh.andypj.xyz

[T35] Lua：字典表
来源：http://hco.aibaodan.cn

local d = { a = 1 };  d.b = 2
来源：http://mjc.pengpengdd.cyou

[T36] Lua：函数
来源：http://ijq.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://tbx.52xcode.cn

[T37] Lua：字符串拼接
来源：http://xpl.hysaishi.cn

"a" .. "b"
来源：http://bnm.chenzaomai.com

[T38] Lua：条件
来源：http://gxw.ybcxt.top

if x > 0 then print("正") end
来源：http://mji.fehbvm.com

[T39] Lua：模式匹配
来源：http://vqw.smart0.xyz

string.find(s, "%d+")
来源：http://vyo.ywan-chungtsiang.top

[T40] Lua：元表
来源：http://paz.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://svk.316326.xyz

[T41] Perl：Hello World
来源：http://zmz.iojbl.cn

print "Hello\n";
来源：http://cec.dashuyun.cn

[T42] Perl：变量类型
来源：http://skb.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zou.yangfankeji.com

[T43] Perl：字符串插值
来源：http://okd.shzxlz.cn

"值: $a"
来源：http://tki.shanyushiyangtech.top

[T44] Perl：条件
来源：http://kgg.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://mkx.gogol.net.cn

[T45] Perl：数组遍历
来源：http://ikd.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://wjz.cucudq.cn

[T46] Perl：哈希操作
来源：http://igt.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nyy.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://vmh.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wtz.birdmap.top

[T48] Perl：正则替换
来源：http://lug.daxiang520.top

$s =~ s/old/new/g;
来源：http://vjq.zhixingplan.top

[T49] Perl：函数
来源：http://yks.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://psw.fehbvm.com

[T50] Perl：逐行读文件
来源：http://ohr.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dgn.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://tij.cucudq.cn

[T51] Scala：Hello World
来源：http://rql.jiagoushi.top

println("Hello")
来源：http://unv.jinghuilouyu.cn

[T52] Scala：变量
来源：http://wya.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://aeu.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://qtf.yonumen.top

s"值: $b"
来源：http://nnp.chenlongwang.top

[T54] Scala：集合映射
来源：http://dpr.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://crv.jqgfzy.top

[T55] Scala：集合过滤
来源：http://nfr.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fws.jqgfzy.top

[T56] Scala：样例类
来源：http://uus.gotoacloud.top

case class User(name: String, age: Int)
来源：http://ypf.fktsv.cn

[T57] Scala：模式匹配
来源：http://fdl.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://qjo.chenlongwang.top

[T58] Scala：函数定义
来源：http://rfn.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://yzq.52xcode.cn

[T59] Scala：循环
来源：http://axa.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://hku.ydzc1.top

[T60] Scala：折叠
来源：http://syk.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rvt.xuanzx.com

================================================================================
来源：http://fhu.zhoulong.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vbj.yangfankeji.com

================================================================================
来源：http://ccw.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://bzv.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://mvi.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://tdx.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cwl.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://afe.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nrc.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://cij.tarul.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://haw.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://riu.ydzc1.top

list(dict.fromkeys(arr))
来源：http://jox.shanyushiyangtech.top

[U06] Py：合并两个字典
来源：http://fpa.sufxvd.cn

{**a, **b}
来源：http://izg.zdqjudy.top

[U07] Py：反转字典键值
来源：http://rai.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://cnd.tianlin.xyz

[U08] Py：展平二维列表
来源：http://gum.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://rvu.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://gyr.ppjwa.cn

max(d, key=d.get)
来源：http://fif.yuanzhike.top

[U10] Py：按值排序字典
来源：http://aja.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fzf.hesvh.cn

[U11] Py：生成器表达式
来源：http://gkn.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://udg.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://eba.fengsongda.top

Counter(arr).most_common(3)
来源：http://mil.ivvv.top

[U13] Py：固定长度队列
来源：http://vcs.kuanghao11.cn

deque(maxlen=10)
来源：http://vvo.hcnkem.com

[U14] Py：分组收集到列表
来源：http://czl.zdbjq.cn

defaultdict(list)
来源：http://roq.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://xjj.shanyushiyangtech.top

t = time.perf_counter()
来源：http://rte.yongpay.top

[U16] Py：命令行参数解析
来源：http://slm.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uaj.daxiang520.top

[U17] Py：初始化日志
来源：http://zan.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://usr.tarul.cn

[U18] Py：预编译正则
来源：http://rqu.xinyue.icu

pat = re.compile(r"\d+")
来源：http://kwk.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://xyt.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xnw.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://crq.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://mbv.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://nhz.xinyue.icu

@contextlib.contextmanager
来源：http://rtr.hfpthk.cn

[U22] Py：矩阵转置
来源：http://zdz.cashguo.top

list(zip(*m))
来源：http://nlc.0kj1m.cn


<!-- 参考信息 -->