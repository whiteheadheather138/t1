代发 wailian999

int x; scanf("%d", &x);
来源：http://krx.jianghu66.top

[S04] C：字符串复制
来源：http://spb.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://jbj.chenjidiqi.icu

[S05] C：字符串长度
来源：http://pgf.zhengqikj.top

strlen(s)
来源：http://gyl.yuanzhike.top

[S06] C：字符串比较
来源：http://ukc.daxiang520.top

strcmp(a, b) == 0
来源：http://ftn.cdnleiting.top

[S07] C：数组遍历求和
来源：http://tyy.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lgw.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://wyk.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hik.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://pyo.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bad.bjfxy.top

[S10] C：指针与解引用
来源：http://cbb.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://mzv.mhx1999.top

[S11] C：逐行读文件
来源：http://usv.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://ogx.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://gzb.yuanzhike.top

fclose(f);
来源：http://fvu.snrcjt.cn

[S12] C：写文件
来源：http://nju.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rlc.feifeiyinyue.top

[S13] C：宏定义
来源：http://kax.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nlw.yueranfly.top

[S14] C：枚举
来源：http://obc.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://grv.zhoulong.xyz

[S15] C：类型转换
来源：http://wjz.aibaodan.cn

(double) a / b
来源：http://utz.xziqi.cn

[S16] C：位操作置位
来源：http://xxl.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://ltc.andypj.xyz

[S17] C：安全拼接字符串
来源：http://ijn.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ezu.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://rks.andypj.xyz

int main(int argc, char **argv)
来源：http://ato.vqdsnc.cn

[S19] C：快速排序
来源：http://ukk.xinyue.icu

qsort(a, n, sizeof(int), cmp);
来源：http://hdr.wangshuangyany.cn

[S20] C：二分查找
来源：http://kih.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kpp.hnqzz.top

[S21] C：字符类别判断
来源：http://kff.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jpk.jinqigfzy.top

[S22] C：字符串转数字
来源：http://smu.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://diu.hesvh.cn

[S23] C：随机数
来源：http://yut.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://kbp.pycfn.com

[S24] C：获取本地时间
来源：http://ona.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nyb.hnqzz.top

[S25] C：内存拷贝
来源：http://xhh.fengsongda.top

memcpy(dst, src, n);
来源：http://yqg.haohaochexian.top

[S26] C：内存清零
来源：http://qvj.yj202588.top

memset(a, 0, sizeof a);
来源：http://ejs.aizwys.cn

[S27] C：定义常量
来源：http://psj.0kj1m.cn

const double PI = 3.14159;
来源：http://kgy.yuxming.cn

[S28] C：静态变量
来源：http://tap.tanke756.top

static int counter = 0;
来源：http://mby.yuxming.cn

[S29] C：变参函数
来源：http://gye.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gcb.nwbrower.top

[S30] C：头文件保护
来源：http://hdg.jinyuanbaomall.cn

#ifndef X_H
来源：http://pjc.tian-w.cn

#define X_H
来源：http://fqa.aibaodan.cn

#endif
来源：http://vrz.yuxming.cn

[S31] C++：Hello World
来源：http://gil.hfpthk.cn

#include <iostream>
来源：http://ema.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://jrk.zycfv.cn

[S32] C++：字符串
来源：http://nnw.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://rtr.c1oappe.top

[S33] C++：vector 增删
来源：http://xtj.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://feo.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://kem.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://jat.yonumen.top

[S35] C++：map
来源：http://snr.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qjk.cqqwz.cn

[S36] C++：unordered_map
来源：http://xad.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uyw.jyoumei.cn

[S37] C++：set
来源：http://gqo.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uzl.epnwcf.com

[S38] C++：排序
来源：http://ugv.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://dpn.uphjek.com

[S39] C++：自定义比较器排序
来源：http://yjd.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zli.svipenyu.cn

[S40] C++：查找元素
来源：http://dfz.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cev.pycfn.com

[S41] C++：类与构造函数
来源：http://wqq.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eth.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://snp.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://bxk.svipenyu.cn

[S43] C++：智能指针
来源：http://kpy.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://eya.ctjpmb.com

[S44] C++：引用传参
来源：http://szj.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://vxg.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://hkk.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qvb.ydjk.org.cn

[S46] C++：函数模板
来源：http://umj.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lso.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://pdy.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iiq.dianchejie.cn

[S48] C++：逐行读文件
来源：http://nyj.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://vup.redwolf501.top

while (std::getline(in, line)) { }
来源：http://hiy.chenlongwang.top

[S49] C++：写文件
来源：http://xvn.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sby.jinqigufen.top

[S50] C++：格式化数字
来源：http://mdf.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rrj.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://wtc.tianlin.xyz

static_cast<double>(a) / b
来源：http://bkq.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://ldd.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://xue.zhijiandao.cn

[S53] C++：移动语义
来源：http://hnz.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://nsa.gogol.net.cn

[S54] C++：异常处理
来源：http://vti.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cwv.yvedp.cn

[S55] C++：结构化绑定
来源：http://utt.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://buu.hesvh.cn

[S56] C++：optional
来源：http://ybh.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ety.xuanzx.com

[S57] C++：编译期常量
来源：http://npu.shanyushiyangtech.top

constexpr int N = 10;
来源：http://sly.xziqi.cn

[S58] C++：命名空间
来源：http://ias.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://tch.zhoulong.xyz

[S59] C++：静态断言
来源：http://xon.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wpq.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://nno.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hzs.zhixingplan.top

================================================================================
来源：http://fur.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://icc.havefunace.top

================================================================================
来源：http://oie.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://eqn.fengsongda.top

println("Hello")
来源：http://xpj.hywenlv.cn

[T02] Kotlin：变量
来源：http://gwp.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gum.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://zdc.c1oappe.top

"值: $b"
来源：http://cyb.shuidangran.top

[T04] Kotlin：空安全
来源：http://egx.yj20258888.top

val n: String? = null;  n?.length
来源：http://kqo.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://zkd.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ajd.yfazqb.com

[T06] Kotlin：集合映射
来源：http://khk.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ind.yonumen.top

[T07] Kotlin：集合过滤
来源：http://csf.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://sgl.nanxinkj.top

[T08] Kotlin：数据类
来源：http://rto.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://zby.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://rxt.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://kkq.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://kvr.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ote.havefunace.top

[T11] Kotlin：协程
来源：http://ipr.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qer.fehbvm.com

[T12] Kotlin：解构声明
来源：http://qvr.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://ihr.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://qbt.birdmap.top

val m = mapOf("a" to 1)
来源：http://elv.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://kki.nwbrower.top

for (i in 1..10) println(i)
来源：http://ner.hnxiangtu.top

[T15] Kotlin：接口
来源：http://yad.redwolf501.top

interface Shape { fun area(): Double }
来源：http://xpl.aizwys.cn

[T16] Swift：Hello World
来源：http://moa.jinyuanbaomall.cn

print("Hello")
来源：http://bef.bjfxy.top

[T17] Swift：变量与常量
来源：http://xsq.ppjwa.cn

var a = 1;  let b = 2
来源：http://pbt.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://war.hfpthk.cn

"值: \(b)"
来源：http://ovb.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://gwz.vehdjk.com

if let n = opt { print(n) }
来源：http://sab.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://unn.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cmg.zhoulong.xyz

[T21] Swift：遍历
来源：http://cav.52xcode.cn

for x in a { print(x) }
来源：http://rbm.52xcode.cn

[T22] Swift：字典
来源：http://qdc.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://cqg.gotoacloud.top

[T23] Swift：函数
来源：http://onf.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://icd.yonumen.top

[T24] Swift：闭包
来源：http://spd.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://mxq.yfazqb.com

[T25] Swift：结构体
来源：http://bps.ppjwa.cn

struct P { var x: Int }
来源：http://trs.zhixingplan.top

[T26] Swift：类与重写
来源：http://imi.fzhhl.top

class A: Base { override func f() {} }
来源：http://cny.zdqjudy.top

[T27] Swift：错误处理
来源：http://gno.cheryme.top

do { try f() } catch { print(error) }
来源：http://kpp.hysaishi.cn

[T28] Swift：枚举
来源：http://uii.yanxiufei.cn

enum Color { case red, green }
来源：http://kqj.tarul.cn

[T29] Swift：guard 提前返回
来源：http://vkb.gaohongyu789.top

guard let x = opt else { return }
来源：http://yye.bbcook.cn

[T30] Swift：协议
来源：http://rso.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://cnj.jinqigfzy.top

[T31] Lua：Hello World
来源：http://wgn.aibaodan.cn

print("Hello")
来源：http://nyi.sxryk.cn

[T32] Lua：局部变量
来源：http://ipf.yfazqb.com

local a = 1
来源：http://ujw.hywenlv.cn

[T33] Lua：表（数组）
来源：http://rxp.nwbrower.top

local t = {1, 2, 3};  t[4] = 4
来源：http://adj.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://ago.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ptd.hnqzz.top

[T35] Lua：字典表
来源：http://hks.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://eyn.andypj.xyz

[T36] Lua：函数
来源：http://ckb.tarul.cn

function add(a, b) return a + b end
来源：http://kdb.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://vii.sweek.top

"a" .. "b"
来源：http://qjf.shanyushiyangtech.top

[T38] Lua：条件
来源：http://mai.birdmap.top

if x > 0 then print("正") end
来源：http://tvk.jqgfzy.top

[T39] Lua：模式匹配
来源：http://cih.feifeiyinyue.top

string.find(s, "%d+")
来源：http://lbu.yanxiufei.cn

[T40] Lua：元表
来源：http://xmz.yj20258888.top

setmetatable({}, { __index = base })
来源：http://lpf.fehbvm.com

[T41] Perl：Hello World
来源：http://pks.ydzc1.top

print "Hello\n";
来源：http://wok.gaohongyu789.top

[T42] Perl：变量类型
来源：http://hdk.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nft.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://ghj.shanyushiyangkeji.top

"值: $a"
来源：http://ftf.yonumen.top

[T44] Perl：条件
来源：http://tbd.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://jsc.yuxming.cn

[T45] Perl：数组遍历
来源：http://lqb.uphjek.com

for my $x (@arr) { print $x; }
来源：http://tvw.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://yqc.bbcook.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bhh.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://qgh.0kj1m.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dih.daria6918.cn

[T48] Perl：正则替换
来源：http://ggz.hysaishi.cn

$s =~ s/old/new/g;
来源：http://dqv.yongpay.top

[T49] Perl：函数
来源：http://fqh.sxryk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jms.hnxiangtu.top

[T50] Perl：逐行读文件
来源：http://zpl.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vxt.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://yie.fengsongda.top

[T51] Scala：Hello World
来源：http://fvu.jinyuanbaomall.cn

println("Hello")
来源：http://vge.guannengcc.top

[T52] Scala：变量
来源：http://ndh.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://mve.mhx1999.top

[T53] Scala：字符串插值
来源：http://lmc.hammf.cn

s"值: $b"
来源：http://cqz.zhengqikj.top

[T54] Scala：集合映射
来源：http://let.yanxiufei.cn

List(1, 2, 3).map(_ * 2)
来源：http://mxj.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://oek.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sdn.c1oappe.top

[T56] Scala：样例类
来源：http://ncy.cashguo.top

case class User(name: String, age: Int)
来源：http://rha.svipenyu.cn

[T57] Scala：模式匹配
来源：http://mqh.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://cby.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://aot.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://zvo.jianghu66.top

[T59] Scala：循环
来源：http://lvz.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://roj.guannengcc.top

[T60] Scala：折叠
来源：http://efl.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zin.xinyue.icu

================================================================================
来源：http://rmy.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rab.jinqigufen.top

================================================================================
来源：http://sua.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://zzi.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://jbu.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://yoh.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cdr.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://yuv.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://azw.smart0.xyz

[U04] Py：变量调试打印
来源：http://hsb.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vth.gaohongyu789.top

[U05] Py：列表去重且保序
来源：http://ubn.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://pba.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://fsb.zhixingplan.top

{**a, **b}
来源：http://aip.bbcook.cn

[U07] Py：反转字典键值
来源：http://yog.gzhubu.top

{v: k for k, v in d.items()}
来源：http://dvj.yangfankeji.com

[U08] Py：展平二维列表
来源：http://jme.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://own.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://xwx.zdbjq.cn

max(d, key=d.get)
来源：http://lpe.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://tmb.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sum.pycfn.com

[U11] Py：生成器表达式
来源：http://ohb.cucudq.cn

(x * 2 for x in arr)
来源：http://rvd.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ltf.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://onc.cqqwz.cn

[U13] Py：固定长度队列
来源：http://rjt.smart0.xyz

deque(maxlen=10)
来源：http://nvk.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://llg.snrcjt.cn

defaultdict(list)
来源：http://kcy.jqgufenzy.top

[U15] Py：高精度计时
来源：http://yjs.meibo888.top

t = time.perf_counter()
来源：http://qbl.andypj.xyz

[U16] Py：命令行参数解析
来源：http://pzs.cqqwz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fbs.birdmap.top

[U17] Py：初始化日志
来源：http://cfe.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://znb.yonumen.top

[U18] Py：预编译正则
来源：http://zdr.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://pus.zycfv.cn

[U19] Py：正则替换带回调
来源：http://itd.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vig.zhiwuduotai.top

[U20] Py：缓存函数结果
来源：http://iiq.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://xtn.sweek.top

[U21] Py：自定义上下文管理器
来源：http://oqe.shuidangran.top

@contextlib.contextmanager
来源：http://izg.daxiang520.top

[U22] Py：矩阵转置
来源：http://vto.yanxiufei.cn

list(zip(*m))
来源：http://htw.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://ibi.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xsj.jiagoushi.top

[U24] Py：路径操作
来源：http://rti.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aiu.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://mkh.fanxiaobao.xyz

csv.DictReader(f)
来源：http://osk.kuanghao11.cn

[U26] Py：并发下载
来源：http://ncj.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rnd.nwbrower.top


<!-- 参考信息 -->