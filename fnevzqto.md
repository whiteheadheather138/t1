代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://jyc.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://wlv.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://mli.ctjpmb.com

[S03] C：读入整数
来源：http://nqk.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://rkq.mhx1999.top

[S04] C：字符串复制
来源：http://ibw.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oee.birdmap.top

[S05] C：字符串长度
来源：http://yih.vqdsnc.cn

strlen(s)
来源：http://myr.tanke756.top

[S06] C：字符串比较
来源：http://qvk.ctjpmb.com

strcmp(a, b) == 0
来源：http://boz.ydzc1.top

[S07] C：数组遍历求和
来源：http://ruj.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dsk.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://yib.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qof.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://myn.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://afe.nwbrower.top

[S10] C：指针与解引用
来源：http://ezj.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://jig.zycfv.cn

[S11] C：逐行读文件
来源：http://zkp.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://quv.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nuy.sweek.top

fclose(f);
来源：http://bku.haohaochexian.top

[S12] C：写文件
来源：http://reo.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://myl.zdqjudy.top

[S13] C：宏定义
来源：http://ysk.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tfv.gzhubu.top

[S14] C：枚举
来源：http://rmq.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://xce.havefunace.top

[S15] C：类型转换
来源：http://zmx.0kj1m.cn

(double) a / b
来源：http://iob.hcnkem.com

[S16] C：位操作置位
来源：http://nda.zhijiandao.cn

x |= (1 << 3);
来源：http://vyi.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://izc.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jpv.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://lbl.xuanzx.com

int main(int argc, char **argv)
来源：http://bdp.smart0.xyz

[S19] C：快速排序
来源：http://emi.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://mxw.hnqzz.top

[S20] C：二分查找
来源：http://kly.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ybh.shzxlz.cn

[S21] C：字符类别判断
来源：http://uwz.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eue.yongpay.top

[S22] C：字符串转数字
来源：http://mpk.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://fxg.sweek.top

[S23] C：随机数
来源：http://hvj.jqgfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ynn.yj20258888.top

[S24] C：获取本地时间
来源：http://tsi.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mzl.yj20258.top

[S25] C：内存拷贝
来源：http://ure.jinqigufen.top

memcpy(dst, src, n);
来源：http://ucs.redwolf501.top

[S26] C：内存清零
来源：http://jjj.fehbvm.com

memset(a, 0, sizeof a);
来源：http://mnt.pycfn.com

[S27] C：定义常量
来源：http://whr.zhixingplan.top

const double PI = 3.14159;
来源：http://dqw.zhixingplan.top

[S28] C：静态变量
来源：http://ejt.haohaochexian.top

static int counter = 0;
来源：http://eui.gaohongyu789.top

[S29] C：变参函数
来源：http://gcg.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mpz.shuidangran.top

[S30] C：头文件保护
来源：http://rjv.birdmap.top

#ifndef X_H
来源：http://sae.smart0.xyz

#define X_H
来源：http://jin.gotoacloud.top

#endif
来源：http://wow.hcnkem.com

[S31] C++：Hello World
来源：http://fzg.nanxinkj.top

#include <iostream>
来源：http://tpk.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://nve.chenlongwang.top

[S32] C++：字符串
来源：http://fae.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://icb.ybcxt.top

[S33] C++：vector 增删
来源：http://hlk.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tcg.yuxming.cn

[S34] C++：遍历 vector
来源：http://oox.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://grb.jqgfzy.top

[S35] C++：map
来源：http://evs.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dot.smart0.xyz

[S36] C++：unordered_map
来源：http://yjp.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qpy.yuanzhike.top

[S37] C++：set
来源：http://mtr.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zvb.sweek.top

[S38] C++：排序
来源：http://wtq.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://hqv.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://vup.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yjs.hysaishi.cn

[S40] C++：查找元素
来源：http://wxe.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oir.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://kjy.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dzy.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://zrb.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://evi.hongshengwenyu.top

[S43] C++：智能指针
来源：http://lpg.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://qxb.bbcook.cn

[S44] C++：引用传参
来源：http://mtv.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://pcl.jlsjyb.cn

[S45] C++：lambda
来源：http://kgy.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fni.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://rbv.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://imv.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://uqy.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sbt.bjfxy.top

[S48] C++：逐行读文件
来源：http://zdc.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://jjv.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://mrw.daria6918.cn

[S49] C++：写文件
来源：http://ctf.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kxq.jlsjyb.cn

[S50] C++：格式化数字
来源：http://naz.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mno.jianghu66.top

[S51] C++：显式类型转换
来源：http://rdv.yanxiufei.cn

static_cast<double>(a) / b
来源：http://kyh.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://ggb.meibo888.top

int size() const noexcept { return n_; }
来源：http://ugk.guowangkeji.top

[S53] C++：移动语义
来源：http://aiz.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://tvv.zhoulong.xyz

[S54] C++：异常处理
来源：http://jxy.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bvw.zhixingplan.top

[S55] C++：结构化绑定
来源：http://bgt.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tli.yangfankeji.com

[S56] C++：optional
来源：http://uxj.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hdd.yangfankeji.com

[S57] C++：编译期常量
来源：http://oyn.yongpay.top

constexpr int N = 10;
来源：http://uxu.sysykeji.top

[S58] C++：命名空间
来源：http://qqy.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://bzx.shuidangran.top

[S59] C++：静态断言
来源：http://mad.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://soi.hcnkem.com

[S60] C++：遍历并删除元素
来源：http://pef.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ygx.316326.xyz

================================================================================
来源：http://yoz.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qtg.ybcxt.top

================================================================================
来源：http://riu.yj202588.top

[T01] Kotlin：Hello World
来源：http://onp.316326.xyz

println("Hello")
来源：http://flj.shanyushiyangkeji.top

[T02] Kotlin：变量
来源：http://cyh.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cpt.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://qie.hfpthk.cn

"值: $b"
来源：http://ulf.mhx1999.top

[T04] Kotlin：空安全
来源：http://oaz.dianchejie.cn

val n: String? = null;  n?.length
来源：http://bxw.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://ehy.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fan.cucudq.cn

[T06] Kotlin：集合映射
来源：http://lny.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jpu.xuetiantiany.cn

[T07] Kotlin：集合过滤
来源：http://vlj.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qsq.iojbl.cn

[T08] Kotlin：数据类
来源：http://rfz.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://ykf.tarul.cn

[T09] Kotlin：扩展函数
来源：http://hxz.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://kjg.yj20258888.top

[T10] Kotlin：默认参数
来源：http://qmn.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uqn.hfpthk.cn

[T11] Kotlin：协程
来源：http://jzx.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wzr.sysykeji.top

[T12] Kotlin：解构声明
来源：http://byx.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://njg.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://vwa.xziqi.cn

val m = mapOf("a" to 1)
来源：http://qkm.vehdjk.com

[T14] Kotlin：循环
来源：http://zgl.xuanzx.com

for (i in 1..10) println(i)
来源：http://yko.sufxvd.cn

[T15] Kotlin：接口
来源：http://rhg.yj20258.top

interface Shape { fun area(): Double }
来源：http://dqn.bbcook.cn

[T16] Swift：Hello World
来源：http://fpz.hesvh.cn

print("Hello")
来源：http://tjs.chenlongwang.top

[T17] Swift：变量与常量
来源：http://saw.jqgufenzy.top

var a = 1;  let b = 2
来源：http://tlm.pycfn.com

[T18] Swift：字符串插值
来源：http://qcn.tarul.cn

"值: \(b)"
来源：http://htr.yj202588.top

[T19] Swift：可选绑定
来源：http://piu.jiagoushi.top

if let n = opt { print(n) }
来源：http://aip.jinqigfzy.top

[T20] Swift：数组操作
来源：http://tgr.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://jxr.ehwqpu.com

[T21] Swift：遍历
来源：http://wfu.sxryk.cn

for x in a { print(x) }
来源：http://fcs.chenjidiqi.icu

[T22] Swift：字典
来源：http://qjz.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xlk.jinghuilouyu.cn

[T23] Swift：函数
来源：http://uqq.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jmn.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://mhn.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xqv.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://ght.yonumen.top

struct P { var x: Int }
来源：http://ipq.zdqjudy.top

[T26] Swift：类与重写
来源：http://jsx.yj20258888.top

class A: Base { override func f() {} }
来源：http://ehg.jinqigfzy.top

[T27] Swift：错误处理
来源：http://ijs.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://zbh.yvedp.cn

[T28] Swift：枚举
来源：http://alf.hesvh.cn

enum Color { case red, green }
来源：http://twr.yvedp.cn

[T29] Swift：guard 提前返回
来源：http://wem.xuanzx.com

guard let x = opt else { return }
来源：http://bpu.0kj1m.cn

[T30] Swift：协议
来源：http://ppl.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://wzf.chenzaomai.com

[T31] Lua：Hello World
来源：http://bvi.hammf.cn

print("Hello")
来源：http://guw.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://hvh.yueranfly.top

local a = 1
来源：http://jyn.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://qih.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ehh.svipenyu.cn

[T34] Lua：遍历表
来源：http://fvu.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://syt.yj20258.top

[T35] Lua：字典表
来源：http://hin.tianlin.xyz

local d = { a = 1 };  d.b = 2
来源：http://kdj.fanxiaobao.xyz

[T36] Lua：函数
来源：http://ztb.jianghu66.top

function add(a, b) return a + b end
来源：http://irh.hesvh.cn

[T37] Lua：字符串拼接
来源：http://bjv.yuanzhike.top

"a" .. "b"
来源：http://dlq.chenzaomai.com

[T38] Lua：条件
来源：http://rne.jinqigfzy.top

if x > 0 then print("正") end
来源：http://egp.yueranfly.top

[T39] Lua：模式匹配
来源：http://oov.aizwys.cn

string.find(s, "%d+")
来源：http://hmg.nanxinkj.top

[T40] Lua：元表
来源：http://rja.daria6918.cn

setmetatable({}, { __index = base })
来源：http://ymf.yuanzhike.top

[T41] Perl：Hello World
来源：http://rfl.hysaishi.cn

print "Hello\n";
来源：http://tie.mhx1999.top

[T42] Perl：变量类型
来源：http://drp.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kce.nanxuanxn.top

[T43] Perl：字符串插值
来源：http://hin.yueranfly.top

"值: $a"
来源：http://rsk.hnqzz.top

[T44] Perl：条件
来源：http://pjc.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://iac.iojbl.cn

[T45] Perl：数组遍历
来源：http://ihp.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://aoj.ivvv.top

[T46] Perl：哈希操作
来源：http://kms.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yib.guowangkeji.top

[T47] Perl：正则捕获
来源：http://mmg.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xxc.ehwqpu.com

[T48] Perl：正则替换
来源：http://lrf.zhixingplan.top

$s =~ s/old/new/g;
来源：http://yrj.nanxinkj.top

[T49] Perl：函数
来源：http://ibo.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xdb.ybcxt.top

[T50] Perl：逐行读文件
来源：http://wcd.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qdt.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://xdj.fengsongda.top

[T51] Scala：Hello World
来源：http://ybx.jinqigufen.top

println("Hello")
来源：http://reb.zycfv.cn

[T52] Scala：变量
来源：http://rlg.xuanzx.com

val a = 1;  var b = 2
来源：http://xta.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://hfy.tarul.cn

s"值: $b"
来源：http://zwc.cashguo.top

[T54] Scala：集合映射
来源：http://vaj.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://oxu.zycfv.cn

[T55] Scala：集合过滤
来源：http://ygk.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://xkv.sweek.top

[T56] Scala：样例类
来源：http://zpg.snrcjt.cn

case class User(name: String, age: Int)
来源：http://jqn.hcnkem.com

[T57] Scala：模式匹配
来源：http://jzz.jqgufenzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jbb.ydjk.org.cn

[T58] Scala：函数定义
来源：http://fya.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://gsv.nwbrower.top

[T59] Scala：循环
来源：http://igv.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://sjr.cheryme.top

[T60] Scala：折叠
来源：http://hxk.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mnj.jqgfzy.top

================================================================================
来源：http://jdo.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://map.9152youxi.cn

================================================================================
来源：http://vev.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://ddt.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://adh.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://mjg.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bjq.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://xuf.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rdd.yongpay.top

[U04] Py：变量调试打印
来源：http://hnq.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cyw.andypj.xyz

[U05] Py：列表去重且保序
来源：http://phw.bjfxy.top

list(dict.fromkeys(arr))
来源：http://cui.svipenyu.cn

[U06] Py：合并两个字典
来源：http://emp.tianlin.xyz

{**a, **b}
来源：http://qgg.zdqjudy.top

[U07] Py：反转字典键值
来源：http://brv.yonumen.top

{v: k for k, v in d.items()}
来源：http://ujm.epnwcf.com

[U08] Py：展平二维列表
来源：http://fwm.cheryme.top

[y for x in nested for y in x]
来源：http://vtf.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://dek.zhixingplan.top

max(d, key=d.get)
来源：http://ikr.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://une.bbcook.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://diz.mhx1999.top

[U11] Py：生成器表达式
来源：http://mzw.guowangkeji.top

(x * 2 for x in arr)
来源：http://rap.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://plq.shzxlz.cn

Counter(arr).most_common(3)
来源：http://jol.tarul.cn

[U13] Py：固定长度队列
来源：http://sgy.andypj.xyz

deque(maxlen=10)
来源：http://ege.sysykeji.top

[U14] Py：分组收集到列表
来源：http://esu.chenjidiqi.icu

defaultdict(list)
来源：http://ydi.dianchejie.cn

[U15] Py：高精度计时
来源：http://aro.snrcjt.cn

t = time.perf_counter()
来源：http://gpm.ybcxt.top

[U16] Py：命令行参数解析
来源：http://pop.zhixingplan.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qwa.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://pnq.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://rgy.uphjek.com

[U18] Py：预编译正则
来源：http://jbb.tarul.cn

pat = re.compile(r"\d+")
来源：http://vmv.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://joy.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gmi.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://jen.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://vid.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://ych.redwolf501.top

@contextlib.contextmanager
来源：http://pbn.birdmap.top

[U22] Py：矩阵转置
来源：http://ikb.fengsongda.top

list(zip(*m))
来源：http://lsx.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://nnq.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://krz.yonumen.top

[U24] Py：路径操作
来源：http://wmb.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lfd.sufxvd.cn


<!-- 参考信息 -->