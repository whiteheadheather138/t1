代发 wailian999

S. C / C++ 专题
来源：http://sci.xziqi.cn

================================================================================
来源：http://jlf.xuetiantiany.cn

[S01] C：Hello World
来源：http://mfs.daria6918.cn

#include <stdio.h>
来源：http://foj.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://sqi.havefunace.top

[S02] C：变量与格式化输出
来源：http://bfs.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://gfr.ydzc1.top

[S03] C：读入整数
来源：http://ecd.cqqwz.cn

int x; scanf("%d", &x);
来源：http://vkb.sweek.top

[S04] C：字符串复制
来源：http://kcp.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://row.yonumen.top

[S05] C：字符串长度
来源：http://qxd.ydzc1.top

strlen(s)
来源：http://ycd.hfpthk.cn

[S06] C：字符串比较
来源：http://ziq.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://dgp.tianlin.xyz

[S07] C：数组遍历求和
来源：http://odd.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ipq.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://irc.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://thq.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://vra.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://enq.hnqzz.top

[S10] C：指针与解引用
来源：http://bcv.daria6918.cn

int *p = &a;  *p = 5;
来源：http://gta.316326.xyz

[S11] C：逐行读文件
来源：http://mlg.fengsongda.top

FILE *f = fopen("a.txt", "r");
来源：http://gsa.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bhk.cucudq.cn

fclose(f);
来源：http://swm.hnxiangtu.top

[S12] C：写文件
来源：http://yul.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zyq.ybcxt.top

[S13] C：宏定义
来源：http://box.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hqv.fanxiaobao.xyz

[S14] C：枚举
来源：http://jcw.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://mlm.hcnkem.com

[S15] C：类型转换
来源：http://qcz.redwolf501.top

(double) a / b
来源：http://zmn.jianghu66.top

[S16] C：位操作置位
来源：http://exb.jianghu66.top

x |= (1 << 3);
来源：http://vzl.tanke756.top

[S17] C：安全拼接字符串
来源：http://rdi.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hpf.daria6918.cn

[S18] C：命令行参数
来源：http://hdt.yj20258.top

int main(int argc, char **argv)
来源：http://trr.vqdsnc.cn

[S19] C：快速排序
来源：http://tig.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://yjl.hywenlv.cn

[S20] C：二分查找
来源：http://cbg.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vww.bbcook.cn

[S21] C：字符类别判断
来源：http://asg.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qut.yueranfly.top

[S22] C：字符串转数字
来源：http://nsk.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://jyv.hcnkem.com

[S23] C：随机数
来源：http://lqd.hammf.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nnw.tian-w.cn

[S24] C：获取本地时间
来源：http://pbi.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nsw.hcnkem.com

[S25] C：内存拷贝
来源：http://pdm.xinyue.icu

memcpy(dst, src, n);
来源：http://qxb.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://wpe.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://heq.yangfankeji.com

[S27] C：定义常量
来源：http://hnp.chenzaomai.com

const double PI = 3.14159;
来源：http://oro.kuanghao11.cn

[S28] C：静态变量
来源：http://oex.hysaishi.cn

static int counter = 0;
来源：http://bir.nwbrower.top

[S29] C：变参函数
来源：http://fmh.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fxg.aibaodan.cn

[S30] C：头文件保护
来源：http://dic.xylfe.cn

#ifndef X_H
来源：http://fri.yj202588.top

#define X_H
来源：http://knc.jinqigufen.top

#endif
来源：http://ftd.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://lgd.feifeiyinyue.top

#include <iostream>
来源：http://etq.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://ini.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://yrl.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://ubd.xuanzx.com

[S33] C++：vector 增删
来源：http://jyd.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fhk.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://opi.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://ioz.zdqjudy.top

[S35] C++：map
来源：http://sgq.xuanzx.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vaw.zhixingplan.top

[S36] C++：unordered_map
来源：http://ztm.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ffq.shanyushiyangkeji.top

[S37] C++：set
来源：http://izo.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tqp.andypj.xyz

[S38] C++：排序
来源：http://bsc.yj20258.top

std::sort(v.begin(), v.end());
来源：http://ngx.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://juq.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qxf.dashuyun.cn

[S40] C++：查找元素
来源：http://jsm.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vdd.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://gmm.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ymf.ybcxt.top

[S42] C++：继承与虚函数
来源：http://cpn.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://xdm.yonumen.top

[S43] C++：智能指针
来源：http://ljm.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://usv.shzxlz.cn

[S44] C++：引用传参
来源：http://nqi.bbcook.cn

void inc(int &x) { ++x; }
来源：http://ctf.hongshengwenyu.top

[S45] C++：lambda
来源：http://ndf.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://kva.svipenyu.cn

[S46] C++：函数模板
来源：http://kuo.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ekb.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://bmh.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tpu.zdqjudy.top

[S48] C++：逐行读文件
来源：http://tvn.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ymy.tarul.cn

while (std::getline(in, line)) { }
来源：http://kri.ehwqpu.com

[S49] C++：写文件
来源：http://xzi.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fmy.yj20258.top

[S50] C++：格式化数字
来源：http://erk.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kan.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://eug.jyoumei.cn

static_cast<double>(a) / b
来源：http://iet.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://weh.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://alo.guannengcc.top

[S53] C++：移动语义
来源：http://uls.cashguo.top

std::vector<int> w = std::move(v);
来源：http://aqw.zhixingplan.top

[S54] C++：异常处理
来源：http://vbr.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ryd.chenlongwang.top

[S55] C++：结构化绑定
来源：http://aoz.ppjwa.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rvq.zhoulong.xyz

[S56] C++：optional
来源：http://grh.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jqu.ivvv.top

[S57] C++：编译期常量
来源：http://vcf.shzxlz.cn

constexpr int N = 10;
来源：http://enf.zycfv.cn

[S58] C++：命名空间
来源：http://chc.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://hll.hcnkem.com

[S59] C++：静态断言
来源：http://qlu.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gxn.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://jlw.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rsi.daria6918.cn

================================================================================
来源：http://nds.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fkt.hammf.cn

================================================================================
来源：http://cgo.zhongyouzk.top

[T01] Kotlin：Hello World
来源：http://cal.pengpengdd.cyou

println("Hello")
来源：http://qjn.sxryk.cn

[T02] Kotlin：变量
来源：http://gmx.kuanghao11.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vuc.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://slz.bjfxy.top

"值: $b"
来源：http://akc.jiagoushi.top

[T04] Kotlin：空安全
来源：http://qic.bjfxy.top

val n: String? = null;  n?.length
来源：http://qrx.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://mhg.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uyp.dianchejie.cn

[T06] Kotlin：集合映射
来源：http://res.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yge.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://qhu.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mvg.pycfn.com

[T08] Kotlin：数据类
来源：http://abl.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://sdk.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://mvb.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://qnd.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://jqh.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bvd.havefunace.top

[T11] Kotlin：协程
来源：http://leg.zdbjq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nfk.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://jle.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://jgh.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://exs.iojbl.cn

val m = mapOf("a" to 1)
来源：http://lbf.zhengqikj.top

[T14] Kotlin：循环
来源：http://jpv.hcnkem.com

for (i in 1..10) println(i)
来源：http://vav.zhongyouzk.top

[T15] Kotlin：接口
来源：http://oky.havefunace.top

interface Shape { fun area(): Double }
来源：http://myq.redwolf501.top

[T16] Swift：Hello World
来源：http://els.shanyushiyangtech.top

print("Hello")
来源：http://opg.9152youxi.cn

[T17] Swift：变量与常量
来源：http://dyq.sufxvd.cn

var a = 1;  let b = 2
来源：http://mqg.zhixingplan.top

[T18] Swift：字符串插值
来源：http://vbx.pycfn.com

"值: \(b)"
来源：http://esq.daria6918.cn

[T19] Swift：可选绑定
来源：http://hih.hywenlv.cn

if let n = opt { print(n) }
来源：http://cnb.ydjk.org.cn

[T20] Swift：数组操作
来源：http://ofq.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://gcr.aizwys.cn

[T21] Swift：遍历
来源：http://obq.hammf.cn

for x in a { print(x) }
来源：http://iqw.hnqzz.top

[T22] Swift：字典
来源：http://pil.feifeiyinyue.top

var d = ["a": 1];  d["b"] = 2
来源：http://wqe.nanxuanxn.top

[T23] Swift：函数
来源：http://qdu.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vqu.guannengcc.top

[T24] Swift：闭包
来源：http://trn.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ytk.vqdsnc.cn

[T25] Swift：结构体
来源：http://joz.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://dox.cheryme.top

[T26] Swift：类与重写
来源：http://wqa.iojbl.cn

class A: Base { override func f() {} }
来源：http://raf.sjlbkw.cn

[T27] Swift：错误处理
来源：http://vmk.tarul.cn

do { try f() } catch { print(error) }
来源：http://qbe.andypj.xyz

[T28] Swift：枚举
来源：http://xlr.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://nqu.meibo888.top

[T29] Swift：guard 提前返回
来源：http://ghl.nanxuanxn.top

guard let x = opt else { return }
来源：http://gfs.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://nyl.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://iaz.nanxuanxn.top

[T31] Lua：Hello World
来源：http://ftl.xziqi.cn

print("Hello")
来源：http://rxv.yueranfly.top

[T32] Lua：局部变量
来源：http://waj.zhengqikj.top

local a = 1
来源：http://edw.yongpay.top

[T33] Lua：表（数组）
来源：http://pub.nanxinkj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zbr.dianchejie.cn

[T34] Lua：遍历表
来源：http://zlg.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://inv.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://sog.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://zen.feifeiyinyue.top

[T36] Lua：函数
来源：http://ayh.gotoacloud.top

function add(a, b) return a + b end
来源：http://neq.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://kib.shanyushiyangkeji.top

"a" .. "b"
来源：http://uht.haohaochexian.top

[T38] Lua：条件
来源：http://wpw.ybcxt.top

if x > 0 then print("正") end
来源：http://avv.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://xcv.zhoulong.xyz

string.find(s, "%d+")
来源：http://xfq.zhiwuduotai.top

[T40] Lua：元表
来源：http://ckt.xylfe.cn

setmetatable({}, { __index = base })
来源：http://whl.svipenyu.cn

[T41] Perl：Hello World
来源：http://ioq.sjlbkw.cn

print "Hello\n";
来源：http://jlz.cashguo.top

[T42] Perl：变量类型
来源：http://twk.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pbb.tian-w.cn

[T43] Perl：字符串插值
来源：http://nzr.bjfxy.top

"值: $a"
来源：http://voo.vqdsnc.cn

[T44] Perl：条件
来源：http://zpy.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://elz.sweek.top

[T45] Perl：数组遍历
来源：http://exr.birdmap.top

for my $x (@arr) { print $x; }
来源：http://lyq.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://fie.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dna.shzxlz.cn

[T47] Perl：正则捕获
来源：http://hnp.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pwz.tian-w.cn

[T48] Perl：正则替换
来源：http://zoz.hfpthk.cn

$s =~ s/old/new/g;
来源：http://uoe.shanyushiyangtech.top

[T49] Perl：函数
来源：http://bji.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://djc.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://peq.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cuo.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://eyj.epnwcf.com

[T51] Scala：Hello World
来源：http://zqr.zhijiandao.cn

println("Hello")
来源：http://geg.hysaishi.cn

[T52] Scala：变量
来源：http://nsu.havefunace.top

val a = 1;  var b = 2
来源：http://hfw.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://mke.ivvv.top

s"值: $b"
来源：http://hrp.yj20258.top

[T54] Scala：集合映射
来源：http://wvn.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://dit.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://wvo.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://akg.gogol.net.cn

[T56] Scala：样例类
来源：http://opn.cucudq.cn

case class User(name: String, age: Int)
来源：http://lgn.hywenlv.cn

[T57] Scala：模式匹配
来源：http://aev.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jtk.yj202588.top

[T58] Scala：函数定义
来源：http://aid.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qjr.ivvv.top

[T59] Scala：循环
来源：http://uet.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://pgr.vehdjk.com

[T60] Scala：折叠
来源：http://fbr.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wyq.zhengqikj.top

================================================================================
来源：http://lmw.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://swn.gotoacloud.top

================================================================================
来源：http://xns.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://snd.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://abo.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://htl.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vom.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://uly.xingfuxueyuan.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://zqv.52xcode.cn

[U04] Py：变量调试打印
来源：http://hhh.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vhw.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://yov.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://rbl.vehdjk.com

[U06] Py：合并两个字典
来源：http://pck.jyoumei.cn

{**a, **b}
来源：http://fcw.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://ycy.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://rrc.sjlbkw.cn

[U08] Py：展平二维列表
来源：http://uom.gzhubu.top

[y for x in nested for y in x]
来源：http://rah.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://zsp.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://rvi.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://ska.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dqu.xinyue.icu

[U11] Py：生成器表达式
来源：http://ckz.vehdjk.com

(x * 2 for x in arr)
来源：http://zte.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://lwo.yfazqb.com

Counter(arr).most_common(3)
来源：http://vve.ctjpmb.com

[U13] Py：固定长度队列
来源：http://yqx.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://cuy.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://dow.mhx1999.top

defaultdict(list)
来源：http://hap.gaohongyu789.top

[U15] Py：高精度计时
来源：http://jeh.xuetiantiany.cn

t = time.perf_counter()
来源：http://psb.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://jnb.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dnv.yvedp.cn

[U17] Py：初始化日志
来源：http://gkl.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ohm.cqqwz.cn

[U18] Py：预编译正则
来源：http://exg.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://mnd.hcnkem.com

[U19] Py：正则替换带回调
来源：http://xsm.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jzb.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://cgk.andypj.xyz

@functools.lru_cache(maxsize=None)
来源：http://mng.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://bko.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://ajo.xziqi.cn

[U22] Py：矩阵转置
来源：http://aen.ehwqpu.com

list(zip(*m))
来源：http://kca.shangyingyoupin.top


<!-- 参考信息 -->