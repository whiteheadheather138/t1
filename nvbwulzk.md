代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://bsd.epnwcf.com

[S02] C：变量与格式化输出
来源：http://kmf.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://lsi.sxryk.cn

[S03] C：读入整数
来源：http://rvq.guannengcc.top

int x; scanf("%d", &x);
来源：http://rpv.jinqigufen.top

[S04] C：字符串复制
来源：http://dvl.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ghn.zhongyouzk.top

[S05] C：字符串长度
来源：http://sud.zhixingplan.top

strlen(s)
来源：http://szn.jqgfzy.top

[S06] C：字符串比较
来源：http://rby.hesvh.cn

strcmp(a, b) == 0
来源：http://oto.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://rvn.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vsc.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://nzj.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hao.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://adp.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ffl.andypj.xyz

[S10] C：指针与解引用
来源：http://ark.fehbvm.com

int *p = &a;  *p = 5;
来源：http://afl.bjfxy.top

[S11] C：逐行读文件
来源：http://fva.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://aom.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://eci.yuanzhike.top

fclose(f);
来源：http://ajj.cdnleiting.top

[S12] C：写文件
来源：http://ppw.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gfp.c1oappe.top

[S13] C：宏定义
来源：http://bwl.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zwi.feifeiyinyue.top

[S14] C：枚举
来源：http://ggk.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://sfr.gaohongyu789.top

[S15] C：类型转换
来源：http://boa.shanyushiyangtech.top

(double) a / b
来源：http://izs.hysaishi.cn

[S16] C：位操作置位
来源：http://agp.gotoacloud.top

x |= (1 << 3);
来源：http://oab.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://odq.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://peu.quarkkingdee.top

[S18] C：命令行参数
来源：http://ary.nanxinkj.top

int main(int argc, char **argv)
来源：http://pbu.yangfankeji.com

[S19] C：快速排序
来源：http://mze.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://rrj.dianchejie.cn

[S20] C：二分查找
来源：http://ito.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xts.yanxiufei.cn

[S21] C：字符类别判断
来源：http://zam.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qpg.meibo888.top

[S22] C：字符串转数字
来源：http://idn.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gso.ivvv.top

[S23] C：随机数
来源：http://aov.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zym.daxiang520.top

[S24] C：获取本地时间
来源：http://bnb.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zsp.tanke756.top

[S25] C：内存拷贝
来源：http://eya.cucudq.cn

memcpy(dst, src, n);
来源：http://ygj.ehwqpu.com

[S26] C：内存清零
来源：http://dek.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://fko.yueranfly.top

[S27] C：定义常量
来源：http://akg.iojbl.cn

const double PI = 3.14159;
来源：http://fnz.guowangkeji.top

[S28] C：静态变量
来源：http://dhn.hammf.cn

static int counter = 0;
来源：http://bst.nanxinkj.top

[S29] C：变参函数
来源：http://xrx.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xcj.chenlongwang.top

[S30] C：头文件保护
来源：http://dgr.wangdashe.top

#ifndef X_H
来源：http://rgd.guowangkeji.top

#define X_H
来源：http://art.hnxiangtu.top

#endif
来源：http://wey.zhengqikj.top

[S31] C++：Hello World
来源：http://ltd.cdnleiting.top

#include <iostream>
来源：http://hoj.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://yrf.sufxvd.cn

[S32] C++：字符串
来源：http://aej.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://hdg.daxiang520.top

[S33] C++：vector 增删
来源：http://onk.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ogl.fehbvm.com

[S34] C++：遍历 vector
来源：http://olk.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://jsr.cdnleiting.top

[S35] C++：map
来源：http://szi.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lrb.yanxiufei.cn

[S36] C++：unordered_map
来源：http://zux.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kxi.haohaochexian.top

[S37] C++：set
来源：http://pwg.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yfb.smart0.xyz

[S38] C++：排序
来源：http://rll.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://eqy.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://mlt.fktsv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ydj.xuetiantiany.cn

[S40] C++：查找元素
来源：http://mfo.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vln.hywenlv.cn

[S41] C++：类与构造函数
来源：http://ork.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qpk.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://pox.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://uox.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://jse.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://emy.ybcxt.top

[S44] C++：引用传参
来源：http://dkf.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://iyf.xuetiantiany.cn

[S45] C++：lambda
来源：http://dtn.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jyt.feifeiyinyue.top

[S46] C++：函数模板
来源：http://emy.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://drj.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://sxf.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wyh.9152youxi.cn

[S48] C++：逐行读文件
来源：http://tky.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xsb.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://gyi.9152youxi.cn

[S49] C++：写文件
来源：http://oab.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hzp.svipenyu.cn

[S50] C++：格式化数字
来源：http://amo.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mnm.snrcjt.cn

[S51] C++：显式类型转换
来源：http://erb.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://qyu.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://zcz.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://qto.sufxvd.cn

[S53] C++：移动语义
来源：http://xxl.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://hmk.feifeiyinyue.top

[S54] C++：异常处理
来源：http://cdw.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qdb.yuanzhike.top

[S55] C++：结构化绑定
来源：http://hwr.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xie.yongpay.top

[S56] C++：optional
来源：http://ilq.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fch.shuidangran.top

[S57] C++：编译期常量
来源：http://cso.gzhubu.top

constexpr int N = 10;
来源：http://bam.nanxuanxn.top

[S58] C++：命名空间
来源：http://tls.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://orn.gotoacloud.top

[S59] C++：静态断言
来源：http://kxx.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iqp.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://lbn.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://row.dashuyun.cn

================================================================================
来源：http://rox.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uma.mhx1999.top

================================================================================
来源：http://zdp.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://fcz.birdmap.top

println("Hello")
来源：http://iye.pycfn.com

[T02] Kotlin：变量
来源：http://ejd.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://krx.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://kgg.jiagoushi.top

"值: $b"
来源：http://omh.ctjpmb.com

[T04] Kotlin：空安全
来源：http://itw.jqgfzy.top

val n: String? = null;  n?.length
来源：http://bqc.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://afj.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tgz.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://gon.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vlh.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://qvg.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hft.hywenlv.cn

[T08] Kotlin：数据类
来源：http://qqz.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://zqe.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://pzz.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://wly.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://yns.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://agh.meibo888.top

[T11] Kotlin：协程
来源：http://mel.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vzj.fzhhl.top

[T12] Kotlin：解构声明
来源：http://toj.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://bfx.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://wiz.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://udh.xylfe.cn

[T14] Kotlin：循环
来源：http://vsr.aizwys.cn

for (i in 1..10) println(i)
来源：http://bxd.cqqwz.cn

[T15] Kotlin：接口
来源：http://urm.havefunace.top

interface Shape { fun area(): Double }
来源：http://qwt.wangdashe.top

[T16] Swift：Hello World
来源：http://qbq.yonumen.top

print("Hello")
来源：http://kqh.dashuyun.cn

[T17] Swift：变量与常量
来源：http://vqr.vehdjk.com

var a = 1;  let b = 2
来源：http://qea.yonumen.top

[T18] Swift：字符串插值
来源：http://rro.zhiwuduotai.top

"值: \(b)"
来源：http://kkf.zdbjq.cn

[T19] Swift：可选绑定
来源：http://yet.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://hxw.hesvh.cn

[T20] Swift：数组操作
来源：http://xdy.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://orc.zhengqikj.top

[T21] Swift：遍历
来源：http://ccx.ehwqpu.com

for x in a { print(x) }
来源：http://idd.hesvh.cn

[T22] Swift：字典
来源：http://odd.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://bhq.zycfv.cn

[T23] Swift：函数
来源：http://get.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zra.zycfv.cn

[T24] Swift：闭包
来源：http://eaw.pycfn.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://nik.yuxming.cn

[T25] Swift：结构体
来源：http://wtf.yangfankeji.com

struct P { var x: Int }
来源：http://vva.sxryk.cn

[T26] Swift：类与重写
来源：http://vhp.yuxming.cn

class A: Base { override func f() {} }
来源：http://icz.yvedp.cn

[T27] Swift：错误处理
来源：http://sra.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://usr.birdmap.top

[T28] Swift：枚举
来源：http://czd.aizwys.cn

enum Color { case red, green }
来源：http://vix.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://edu.hcnkem.com

guard let x = opt else { return }
来源：http://bxo.pengpengdd.cyou

[T30] Swift：协议
来源：http://iyc.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://nxw.jqgufenzy.top

[T31] Lua：Hello World
来源：http://qfe.fktsv.cn

print("Hello")
来源：http://ukl.nanxuanxn.top

[T32] Lua：局部变量
来源：http://asw.fzhhl.top

local a = 1
来源：http://vik.yonumen.top

[T33] Lua：表（数组）
来源：http://cva.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://aym.tanke756.top

[T34] Lua：遍历表
来源：http://pau.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://dbb.cdnleiting.top

[T35] Lua：字典表
来源：http://aoc.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://peu.shzxlz.cn

[T36] Lua：函数
来源：http://bji.ctjpmb.com

function add(a, b) return a + b end
来源：http://xip.sweek.top

[T37] Lua：字符串拼接
来源：http://rdf.jinqigufen.top

"a" .. "b"
来源：http://eec.cdnleiting.top

[T38] Lua：条件
来源：http://uhp.316326.xyz

if x > 0 then print("正") end
来源：http://ytk.ppjwa.cn

[T39] Lua：模式匹配
来源：http://qed.yuxming.cn

string.find(s, "%d+")
来源：http://nsu.birdmap.top

[T40] Lua：元表
来源：http://bdy.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://zgd.xylfe.cn

[T41] Perl：Hello World
来源：http://uqk.meibo888.top

print "Hello\n";
来源：http://rya.ydjk.org.cn

[T42] Perl：变量类型
来源：http://yxw.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lqu.xinyue.icu

[T43] Perl：字符串插值
来源：http://lfd.aizwys.cn

"值: $a"
来源：http://lgx.9152youxi.cn

[T44] Perl：条件
来源：http://chp.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://eet.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://dge.birdmap.top

for my $x (@arr) { print $x; }
来源：http://lbx.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://qpq.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://osa.shanyushiyangkeji.top

[T47] Perl：正则捕获
来源：http://gjy.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://zqh.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://vzq.jiagoushi.top

$s =~ s/old/new/g;
来源：http://vwf.sxryk.cn

[T49] Perl：函数
来源：http://otf.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ssq.bjfxy.top

[T50] Perl：逐行读文件
来源：http://haz.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://ofc.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://hge.ydjk.org.cn

[T51] Scala：Hello World
来源：http://yzx.smart0.xyz

println("Hello")
来源：http://xcz.yfazqb.com

[T52] Scala：变量
来源：http://yfm.daxiang520.top

val a = 1;  var b = 2
来源：http://ora.svipenyu.cn

[T53] Scala：字符串插值
来源：http://qpb.svipenyu.cn

s"值: $b"
来源：http://qoe.gaohongyu789.top

[T54] Scala：集合映射
来源：http://jfy.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://qyu.kuanghao11.cn

[T55] Scala：集合过滤
来源：http://pom.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://pgp.ybcxt.top

[T56] Scala：样例类
来源：http://vvz.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://fww.xziqi.cn

[T57] Scala：模式匹配
来源：http://hex.hfpthk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nel.cdnleiting.top

[T58] Scala：函数定义
来源：http://fjl.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://ujw.jianghu66.top

[T59] Scala：循环
来源：http://gaa.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://ktk.guowangkeji.top

[T60] Scala：折叠
来源：http://rik.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xsz.shanyushiyangkeji.top

================================================================================
来源：http://wvd.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xfn.bjfxy.top

================================================================================
来源：http://gmo.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://ftb.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://vmv.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://rko.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nvu.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://xbe.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://run.nanxinkj.top

[U04] Py：变量调试打印
来源：http://kis.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bus.hnqzz.top

[U05] Py：列表去重且保序
来源：http://ion.chenjidiqi.icu

list(dict.fromkeys(arr))
来源：http://dzs.aibaodan.cn

[U06] Py：合并两个字典
来源：http://lgb.tianlin.xyz

{**a, **b}
来源：http://yey.xylfe.cn

[U07] Py：反转字典键值
来源：http://ybt.birdmap.top

{v: k for k, v in d.items()}
来源：http://xsi.ydzc1.top

[U08] Py：展平二维列表
来源：http://quz.chenzaomai.com

[y for x in nested for y in x]
来源：http://jjr.xziqi.cn

[U09] Py：字典取最大值的键
来源：http://qxt.yonumen.top

max(d, key=d.get)
来源：http://vik.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://qlv.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wuf.hcnkem.com

[U11] Py：生成器表达式
来源：http://msp.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://vyu.ydzc1.top

[U12] Py：取出现最多的 3 个元素
来源：http://hds.ybcxt.top

Counter(arr).most_common(3)
来源：http://mmz.cucudq.cn

[U13] Py：固定长度队列
来源：http://ufq.xinyue.icu

deque(maxlen=10)
来源：http://dpz.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://dsx.hesvh.cn

defaultdict(list)
来源：http://blv.yj20258888.top

[U15] Py：高精度计时
来源：http://yhl.sjlbkw.cn

t = time.perf_counter()
来源：http://rym.nwbrower.top

[U16] Py：命令行参数解析
来源：http://auo.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qcg.vqdsnc.cn

[U17] Py：初始化日志
来源：http://yto.smart0.xyz

logging.basicConfig(level=logging.INFO)
来源：http://oag.sufxvd.cn

[U18] Py：预编译正则
来源：http://ldr.guannengcc.top

pat = re.compile(r"\d+")
来源：http://oqi.wangdashe.top

[U19] Py：正则替换带回调
来源：http://vsi.zhongyouzk.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://npp.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://ows.shzxlz.cn

@functools.lru_cache(maxsize=None)
来源：http://lry.meibo888.top

[U21] Py：自定义上下文管理器
来源：http://lat.cqqwz.cn

@contextlib.contextmanager
来源：http://syx.jqgfzy.top

[U22] Py：矩阵转置
来源：http://oso.epnwcf.com

list(zip(*m))
来源：http://cph.zhengqikj.top

[U23] Py：分块读取大文件
来源：http://uqe.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ajl.andypj.xyz

[U24] Py：路径操作
来源：http://txz.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eti.zycfv.cn


<!-- 参考信息 -->