代发 wailian999

strlen(s)
来源：http://fhd.ydjk.org.cn

[S06] C：字符串比较
来源：http://ugj.gaohongyu789.top

strcmp(a, b) == 0
来源：http://uvi.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://lqj.ybcxt.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fxn.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://dll.aizwys.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sve.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://rsr.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bat.xuanzx.com

[S10] C：指针与解引用
来源：http://ukd.gzhubu.top

int *p = &a;  *p = 5;
来源：http://ecm.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://juq.meibo888.top

FILE *f = fopen("a.txt", "r");
来源：http://qqa.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iwo.yongpay.top

fclose(f);
来源：http://otf.52xcode.cn

[S12] C：写文件
来源：http://urb.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://umx.guowangkeji.top

[S13] C：宏定义
来源：http://awt.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rhy.fengsongda.top

[S14] C：枚举
来源：http://emd.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://ysv.jqgufenzy.top

[S15] C：类型转换
来源：http://khz.cucudq.cn

(double) a / b
来源：http://jeg.ivvv.top

[S16] C：位操作置位
来源：http://tey.zhixingplan.top

x |= (1 << 3);
来源：http://loj.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://ruj.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://thv.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://nqh.bjfxy.top

int main(int argc, char **argv)
来源：http://yox.yvedp.cn

[S19] C：快速排序
来源：http://yte.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://asd.bjfxy.top

[S20] C：二分查找
来源：http://nhi.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nwc.iojbl.cn

[S21] C：字符类别判断
来源：http://nlz.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xou.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://vrh.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cwp.shanyushiyangtech.top

[S23] C：随机数
来源：http://qob.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hmk.svipenyu.cn

[S24] C：获取本地时间
来源：http://dgr.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sim.aizwys.cn

[S25] C：内存拷贝
来源：http://lyt.jinqigfzy.top

memcpy(dst, src, n);
来源：http://aca.yj202588.top

[S26] C：内存清零
来源：http://mkg.daria6918.cn

memset(a, 0, sizeof a);
来源：http://rmh.ivvv.top

[S27] C：定义常量
来源：http://pbo.wangshuangyany.cn

const double PI = 3.14159;
来源：http://fev.chenlongwang.top

[S28] C：静态变量
来源：http://vzu.tarul.cn

static int counter = 0;
来源：http://meg.gotoacloud.top

[S29] C：变参函数
来源：http://pap.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bgw.havefunace.top

[S30] C：头文件保护
来源：http://bzo.ydjk.org.cn

#ifndef X_H
来源：http://qst.zhongyouzk.top

#define X_H
来源：http://yxk.0kj1m.cn

#endif
来源：http://npt.nanxuanxn.top

[S31] C++：Hello World
来源：http://yor.zdqjudy.top

#include <iostream>
来源：http://qld.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://nwx.hammf.cn

[S32] C++：字符串
来源：http://mdp.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://umq.sjlbkw.cn

[S33] C++：vector 增删
来源：http://ulk.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ehm.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://wjo.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://kpj.gotoacloud.top

[S35] C++：map
来源：http://csy.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zgk.chenlongwang.top

[S36] C++：unordered_map
来源：http://lef.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://itt.fzhhl.top

[S37] C++：set
来源：http://vjx.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eqz.daria6918.cn

[S38] C++：排序
来源：http://axm.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://ksc.daria6918.cn

[S39] C++：自定义比较器排序
来源：http://dyx.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nze.ehwqpu.com

[S40] C++：查找元素
来源：http://ugz.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pmw.aibaodan.cn

[S41] C++：类与构造函数
来源：http://prp.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rzy.cheryme.top

[S42] C++：继承与虚函数
来源：http://igf.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://lpj.yj20258.top

[S43] C++：智能指针
来源：http://hnx.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://isl.yonumen.top

[S44] C++：引用传参
来源：http://viv.52xcode.cn

void inc(int &x) { ++x; }
来源：http://ggd.fengsongda.top

[S45] C++：lambda
来源：http://xor.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://uqu.zhoulong.xyz

[S46] C++：函数模板
来源：http://wfo.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wks.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://qlk.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vbv.hfpthk.cn

[S48] C++：逐行读文件
来源：http://pot.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://ipd.hammf.cn

while (std::getline(in, line)) { }
来源：http://ill.gaohongyu789.top

[S49] C++：写文件
来源：http://dye.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://obt.gaohongyu789.top

[S50] C++：格式化数字
来源：http://ffd.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tqq.redwolf501.top

[S51] C++：显式类型转换
来源：http://iec.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://zwl.yongpay.top

[S52] C++：const 与 noexcept
来源：http://ghe.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://bbq.wangshuangyany.cn

[S53] C++：移动语义
来源：http://jkg.9152youxi.cn

std::vector<int> w = std::move(v);
来源：http://fya.9152youxi.cn

[S54] C++：异常处理
来源：http://isk.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sla.dianchejie.cn

[S55] C++：结构化绑定
来源：http://xsu.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cnd.cucudq.cn

[S56] C++：optional
来源：http://fim.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uzc.52xcode.cn

[S57] C++：编译期常量
来源：http://twt.ctjpmb.com

constexpr int N = 10;
来源：http://dpz.0kj1m.cn

[S58] C++：命名空间
来源：http://baq.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://ozr.jinqigufen.top

[S59] C++：静态断言
来源：http://twk.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qka.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://die.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pod.hammf.cn

================================================================================
来源：http://mud.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://irc.cqqwz.cn

================================================================================
来源：http://wim.zycfv.cn

[T01] Kotlin：Hello World
来源：http://fvj.epnwcf.com

println("Hello")
来源：http://toy.hcnkem.com

[T02] Kotlin：变量
来源：http://ijr.yfazqb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bvr.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://vwf.hfpthk.cn

"值: $b"
来源：http://dru.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://ghf.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://qrn.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://cfq.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zph.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://mci.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://exw.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://yjo.andypj.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://fly.yvedp.cn

[T08] Kotlin：数据类
来源：http://vmq.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://fsc.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://kfd.pycfn.com

fun String.exclaim() = this + "!"
来源：http://nax.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://wya.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://akc.vqdsnc.cn

[T11] Kotlin：协程
来源：http://kxa.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cjc.wangdashe.top

[T12] Kotlin：解构声明
来源：http://kjs.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://zcq.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://fin.bjfxy.top

val m = mapOf("a" to 1)
来源：http://cdd.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://izr.shuidangran.top

for (i in 1..10) println(i)
来源：http://aiv.yangfankeji.com

[T15] Kotlin：接口
来源：http://iim.sysykeji.top

interface Shape { fun area(): Double }
来源：http://pck.wangdashe.top

[T16] Swift：Hello World
来源：http://zwi.wangdashe.top

print("Hello")
来源：http://ozp.hnqzz.top

[T17] Swift：变量与常量
来源：http://urd.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://den.guannengcc.top

[T18] Swift：字符串插值
来源：http://dnu.zdqjudy.top

"值: \(b)"
来源：http://xcg.zhengqikj.top

[T19] Swift：可选绑定
来源：http://zhi.sufxvd.cn

if let n = opt { print(n) }
来源：http://jlj.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://qwp.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nvu.cqqwz.cn

[T21] Swift：遍历
来源：http://ijf.zhijiandao.cn

for x in a { print(x) }
来源：http://ivj.ehwqpu.com

[T22] Swift：字典
来源：http://owp.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://nle.52xcode.cn

[T23] Swift：函数
来源：http://npn.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fjc.meibo888.top

[T24] Swift：闭包
来源：http://iyk.guannengcc.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://snl.dianchejie.cn

[T25] Swift：结构体
来源：http://uup.daria6918.cn

struct P { var x: Int }
来源：http://uce.hammf.cn

[T26] Swift：类与重写
来源：http://fgf.pycfn.com

class A: Base { override func f() {} }
来源：http://ist.hcnkem.com

[T27] Swift：错误处理
来源：http://kwy.hesvh.cn

do { try f() } catch { print(error) }
来源：http://yrb.316326.xyz

[T28] Swift：枚举
来源：http://ruh.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://zbr.hammf.cn

[T29] Swift：guard 提前返回
来源：http://xog.zhiwuduotai.top

guard let x = opt else { return }
来源：http://wnx.fktsv.cn

[T30] Swift：协议
来源：http://qtm.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://uvf.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://uhy.ydzc1.top

print("Hello")
来源：http://pok.ppjwa.cn

[T32] Lua：局部变量
来源：http://xmm.zhiwuduotai.top

local a = 1
来源：http://nba.fktsv.cn

[T33] Lua：表（数组）
来源：http://kjv.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yvo.fzhhl.top

[T34] Lua：遍历表
来源：http://nmk.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hgd.chenjidiqi.icu

[T35] Lua：字典表
来源：http://hcj.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://cbh.yueranfly.top

[T36] Lua：函数
来源：http://sdi.sufxvd.cn

function add(a, b) return a + b end
来源：http://xjz.yueranfly.top

[T37] Lua：字符串拼接
来源：http://hco.jinghuilouyu.cn

"a" .. "b"
来源：http://joa.zhongyouzk.top

[T38] Lua：条件
来源：http://qds.jinqigfzy.top

if x > 0 then print("正") end
来源：http://wdm.hfpthk.cn

[T39] Lua：模式匹配
来源：http://utm.birdmap.top

string.find(s, "%d+")
来源：http://cvx.daria6918.cn

[T40] Lua：元表
来源：http://bwv.316326.xyz

setmetatable({}, { __index = base })
来源：http://pmb.xuetiantiany.cn

[T41] Perl：Hello World
来源：http://ttt.tianlin.xyz

print "Hello\n";
来源：http://fyd.hnqzz.top

[T42] Perl：变量类型
来源：http://sdh.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jfy.cashguo.top

[T43] Perl：字符串插值
来源：http://yle.yuanzhike.top

"值: $a"
来源：http://zsg.xylfe.cn

[T44] Perl：条件
来源：http://oja.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://sgm.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://rpe.ywan-chungtsiang.top

for my $x (@arr) { print $x; }
来源：http://eor.jiagoushi.top

[T46] Perl：哈希操作
来源：http://lvi.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mvs.yuanzhike.top

[T47] Perl：正则捕获
来源：http://wmm.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://awm.jqgfzy.top

[T48] Perl：正则替换
来源：http://shf.jyoumei.cn

$s =~ s/old/new/g;
来源：http://svi.fktsv.cn

[T49] Perl：函数
来源：http://lob.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tes.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://oai.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://oeo.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://izr.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://vjk.cdnleiting.top

println("Hello")
来源：http://fmu.shangyingyoupin.top

[T52] Scala：变量
来源：http://xrr.cdnleiting.top

val a = 1;  var b = 2
来源：http://mzk.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://pwl.cdnleiting.top

s"值: $b"
来源：http://uuq.zhongyouzk.top

[T54] Scala：集合映射
来源：http://ygn.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://pvw.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://ost.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://kqw.wangshuangyany.cn

[T56] Scala：样例类
来源：http://ski.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://owt.c1oappe.top

[T57] Scala：模式匹配
来源：http://mis.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://afc.ppjwa.cn

[T58] Scala：函数定义
来源：http://sgn.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://ibo.tian-w.cn

[T59] Scala：循环
来源：http://wfv.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://bet.zhoulong.xyz

[T60] Scala：折叠
来源：http://enw.chenjidiqi.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sbi.zhongyouzk.top

================================================================================
来源：http://hcq.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xgb.hnqzz.top

================================================================================
来源：http://msy.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://qvm.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://ejh.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://jqd.jlsjyb.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bwo.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://wlk.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://vtb.gzhubu.top

[U04] Py：变量调试打印
来源：http://ffo.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mvw.zhengqikj.top

[U05] Py：列表去重且保序
来源：http://avy.tian-w.cn

list(dict.fromkeys(arr))
来源：http://kzu.haohaochexian.top

[U06] Py：合并两个字典
来源：http://asv.zdbjq.cn

{**a, **b}
来源：http://zow.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://tqh.bjfxy.top

{v: k for k, v in d.items()}
来源：http://kad.hnqzz.top

[U08] Py：展平二维列表
来源：http://rnm.yuanzhike.top

[y for x in nested for y in x]
来源：http://nyj.havefunace.top

[U09] Py：字典取最大值的键
来源：http://com.aibaodan.cn

max(d, key=d.get)
来源：http://yvr.cqqwz.cn

[U10] Py：按值排序字典
来源：http://ntz.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yqf.dianchejie.cn

[U11] Py：生成器表达式
来源：http://xdp.chenzaomai.com

(x * 2 for x in arr)
来源：http://usl.ppjwa.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zjo.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://koc.yj202588.top

[U13] Py：固定长度队列
来源：http://rpz.chenzaomai.com

deque(maxlen=10)
来源：http://brh.jianghu66.top

[U14] Py：分组收集到列表
来源：http://nru.c1oappe.top

defaultdict(list)
来源：http://frr.cucudq.cn

[U15] Py：高精度计时
来源：http://cqi.yj20258888.top

t = time.perf_counter()
来源：http://exz.sjlbkw.cn

[U16] Py：命令行参数解析
来源：http://mlw.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://thn.smart0.xyz

[U17] Py：初始化日志
来源：http://tsh.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://ewe.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://pxl.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://rph.yueranfly.top

[U19] Py：正则替换带回调
来源：http://uka.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mrv.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://hip.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://dra.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://mfq.ydzc1.top

@contextlib.contextmanager
来源：http://ivq.chenzaomai.com

[U22] Py：矩阵转置
来源：http://sdf.ivvv.top

list(zip(*m))
来源：http://vuh.shuidangran.top

[U23] Py：分块读取大文件
来源：http://ham.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qke.jinqigfzy.top

[U24] Py：路径操作
来源：http://slj.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ewy.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://faw.kuanghao11.cn

csv.DictReader(f)
来源：http://hop.yj20258888.top

[U26] Py：并发下载
来源：http://znj.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mfp.fktsv.cn

[U27] Py：异步 HTTP
来源：http://mrb.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://opc.haohaochexian.top

[U28] Py：类型别名
来源：http://nfi.daxiang520.top

UserId = int
来源：http://sij.9152youxi.cn


<!-- 参考信息 -->