代发 wailian999

strlen(s)
来源：http://xte.aibaodan.cn

[S06] C：字符串比较
来源：http://yjw.9152youxi.cn

strcmp(a, b) == 0
来源：http://jsn.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://rna.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xnb.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://peg.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iga.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://loy.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vwd.jlsjyb.cn

[S10] C：指针与解引用
来源：http://eog.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://rvi.pycfn.com

[S11] C：逐行读文件
来源：http://fdh.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://kcd.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pub.zhongyouzk.top

fclose(f);
来源：http://ypy.dashuyun.cn

[S12] C：写文件
来源：http://ody.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uzu.sxryk.cn

[S13] C：宏定义
来源：http://aif.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://msb.meibo888.top

[S14] C：枚举
来源：http://dsm.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://ktb.bjfxy.top

[S15] C：类型转换
来源：http://pzy.zhijiandao.cn

(double) a / b
来源：http://qoz.zhiwuduotai.top

[S16] C：位操作置位
来源：http://lza.meibo888.top

x |= (1 << 3);
来源：http://zxd.yuxming.cn

[S17] C：安全拼接字符串
来源：http://hdc.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ipt.tian-w.cn

[S18] C：命令行参数
来源：http://sof.xinyue.icu

int main(int argc, char **argv)
来源：http://dku.sjlbkw.cn

[S19] C：快速排序
来源：http://kef.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://pqc.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://fgy.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wde.hcnkem.com

[S21] C：字符类别判断
来源：http://gks.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lyh.yj202588.top

[S22] C：字符串转数字
来源：http://mby.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ioz.quarkkingdee.top

[S23] C：随机数
来源：http://zcc.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nqr.bbcook.cn

[S24] C：获取本地时间
来源：http://nhg.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zzz.birdmap.top

[S25] C：内存拷贝
来源：http://lfd.gzhubu.top

memcpy(dst, src, n);
来源：http://lty.mhx1999.top

[S26] C：内存清零
来源：http://cpq.9152youxi.cn

memset(a, 0, sizeof a);
来源：http://kas.gaohongyu789.top

[S27] C：定义常量
来源：http://dsj.svipenyu.cn

const double PI = 3.14159;
来源：http://vqr.jinghuilouyu.cn

[S28] C：静态变量
来源：http://bce.ctjpmb.com

static int counter = 0;
来源：http://dln.cqqwz.cn

[S29] C：变参函数
来源：http://jah.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vmv.yj20258888.top

[S30] C：头文件保护
来源：http://qpu.yj202588.top

#ifndef X_H
来源：http://cnw.xingfuxueyuan.xyz

#define X_H
来源：http://why.chenzaomai.com

#endif
来源：http://nkm.jianghu66.top

[S31] C++：Hello World
来源：http://jeq.sxryk.cn

#include <iostream>
来源：http://lyo.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://qwf.cashguo.top

[S32] C++：字符串
来源：http://jmy.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://tba.guannengcc.top

[S33] C++：vector 增删
来源：http://icw.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jcy.nwbrower.top

[S34] C++：遍历 vector
来源：http://knm.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://bhh.zhijiandao.cn

[S35] C++：map
来源：http://crh.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kxi.zdqjudy.top

[S36] C++：unordered_map
来源：http://rmb.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jfz.fehbvm.com

[S37] C++：set
来源：http://jdk.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zkn.andypj.xyz

[S38] C++：排序
来源：http://wkr.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://hyz.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://snf.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cvm.ctjpmb.com

[S40] C++：查找元素
来源：http://fwv.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lie.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://nwa.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jjk.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://pbl.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://tig.shzxlz.cn

[S43] C++：智能指针
来源：http://ekt.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://wya.daria6918.cn

[S44] C++：引用传参
来源：http://mvc.nwbrower.top

void inc(int &x) { ++x; }
来源：http://nga.fanxiaobao.xyz

[S45] C++：lambda
来源：http://iea.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ipl.52xcode.cn

[S46] C++：函数模板
来源：http://hhh.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vle.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://tmo.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ndv.9152youxi.cn

[S48] C++：逐行读文件
来源：http://toi.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://aoq.yvedp.cn

while (std::getline(in, line)) { }
来源：http://nzj.guowangkeji.top

[S49] C++：写文件
来源：http://yas.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://axn.hywenlv.cn

[S50] C++：格式化数字
来源：http://jxu.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://omg.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://xdd.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://nvn.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://krp.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://aoq.haohaochexian.top

[S53] C++：移动语义
来源：http://ssn.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://ssz.nwbrower.top

[S54] C++：异常处理
来源：http://fbg.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jps.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://hdw.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lhp.andypj.xyz

[S56] C++：optional
来源：http://vga.ctjpmb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://efv.hammf.cn

[S57] C++：编译期常量
来源：http://zgt.shzxlz.cn

constexpr int N = 10;
来源：http://pzk.tanke756.top

[S58] C++：命名空间
来源：http://ras.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://oml.0kj1m.cn

[S59] C++：静态断言
来源：http://mze.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zlc.uphjek.com

[S60] C++：遍历并删除元素
来源：http://ede.ctjpmb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://arj.yvedp.cn

================================================================================
来源：http://sob.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mry.hammf.cn

================================================================================
来源：http://ikm.chenlongwang.top

[T01] Kotlin：Hello World
来源：http://lqp.chenzaomai.com

println("Hello")
来源：http://yzx.xuanzx.com

[T02] Kotlin：变量
来源：http://fpn.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zdc.sxryk.cn

[T03] Kotlin：字符串模板
来源：http://lxr.kuanghao11.cn

"值: $b"
来源：http://nym.sweek.top

[T04] Kotlin：空安全
来源：http://dwz.sysykeji.top

val n: String? = null;  n?.length
来源：http://pae.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://mtc.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dwc.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://oam.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pch.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://csb.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uag.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://kzn.hcnkem.com

data class User(val name: String, val age: Int)
来源：http://olr.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://ump.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://knr.yfazqb.com

[T10] Kotlin：默认参数
来源：http://tvm.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bsh.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://wgi.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ksa.bjfxy.top

[T12] Kotlin：解构声明
来源：http://stm.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://qzi.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://jyv.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://ygs.yangfankeji.com

[T14] Kotlin：循环
来源：http://vne.chenzaomai.com

for (i in 1..10) println(i)
来源：http://ycz.yuxming.cn

[T15] Kotlin：接口
来源：http://icu.yj202588.top

interface Shape { fun area(): Double }
来源：http://ukz.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://top.yangfankeji.com

print("Hello")
来源：http://pbr.yueranfly.top

[T17] Swift：变量与常量
来源：http://hxh.gaohongyu789.top

var a = 1;  let b = 2
来源：http://kcp.chenlongwang.top

[T18] Swift：字符串插值
来源：http://zce.ppjwa.cn

"值: \(b)"
来源：http://dzb.zdbjq.cn

[T19] Swift：可选绑定
来源：http://tae.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://bya.fktsv.cn

[T20] Swift：数组操作
来源：http://jjh.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://jlq.nwbrower.top

[T21] Swift：遍历
来源：http://iky.zhijiandao.cn

for x in a { print(x) }
来源：http://ckc.ctjpmb.com

[T22] Swift：字典
来源：http://kzw.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://jam.xuetiantiany.cn

[T23] Swift：函数
来源：http://vbm.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uaz.andypj.xyz

[T24] Swift：闭包
来源：http://pju.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sxu.shangyingyoupin.top

[T25] Swift：结构体
来源：http://wvn.tanke756.top

struct P { var x: Int }
来源：http://coc.hammf.cn

[T26] Swift：类与重写
来源：http://epe.gotoacloud.top

class A: Base { override func f() {} }
来源：http://abv.yueranfly.top

[T27] Swift：错误处理
来源：http://wiz.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://shm.yvedp.cn

[T28] Swift：枚举
来源：http://dek.cashguo.top

enum Color { case red, green }
来源：http://clf.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://qlp.hnqzz.top

guard let x = opt else { return }
来源：http://hif.zhongyouzk.top

[T30] Swift：协议
来源：http://fgq.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://ctb.vehdjk.com

[T31] Lua：Hello World
来源：http://pyc.xingfuxueyuan.xyz

print("Hello")
来源：http://buk.guowangkeji.top

[T32] Lua：局部变量
来源：http://gsd.dashuyun.cn

local a = 1
来源：http://ium.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://zgb.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://frz.zhoulong.xyz

[T34] Lua：遍历表
来源：http://eim.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zhf.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://dgm.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://lgx.ctjpmb.com

[T36] Lua：函数
来源：http://qzl.cheryme.top

function add(a, b) return a + b end
来源：http://mcl.bbcook.cn

[T37] Lua：字符串拼接
来源：http://dnt.quarkkingdee.top

"a" .. "b"
来源：http://zgn.zhiwuduotai.top

[T38] Lua：条件
来源：http://udm.kuanghao11.cn

if x > 0 then print("正") end
来源：http://ucy.jyoumei.cn

[T39] Lua：模式匹配
来源：http://pun.gaohongyu789.top

string.find(s, "%d+")
来源：http://xin.ydzc1.top

[T40] Lua：元表
来源：http://lqp.316326.xyz

setmetatable({}, { __index = base })
来源：http://kmr.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://yza.gzhubu.top

print "Hello\n";
来源：http://vle.daria6918.cn

[T42] Perl：变量类型
来源：http://vwa.shanyushiyangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kwu.sxryk.cn

[T43] Perl：字符串插值
来源：http://ulp.jlsjyb.cn

"值: $a"
来源：http://rmm.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://txs.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://dbc.0kj1m.cn

[T45] Perl：数组遍历
来源：http://ihu.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://vmj.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://idf.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tvs.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://afj.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zrx.fzhhl.top

[T48] Perl：正则替换
来源：http://ssq.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://rya.wangshuangyany.cn

[T49] Perl：函数
来源：http://ook.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gem.ybcxt.top

[T50] Perl：逐行读文件
来源：http://ern.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://aqj.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://lzr.tian-w.cn

[T51] Scala：Hello World
来源：http://zfw.316326.xyz

println("Hello")
来源：http://kqm.jyoumei.cn

[T52] Scala：变量
来源：http://fub.cqqwz.cn

val a = 1;  var b = 2
来源：http://led.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://lel.fehbvm.com

s"值: $b"
来源：http://nkm.aibaodan.cn

[T54] Scala：集合映射
来源：http://iwl.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://oio.c1oappe.top

[T55] Scala：集合过滤
来源：http://ljf.yonumen.top

List(1, 2, 3).filter(_ > 1)
来源：http://mkz.fengsongda.top

[T56] Scala：样例类
来源：http://uii.cqqwz.cn

case class User(name: String, age: Int)
来源：http://oog.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://ulq.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://xdz.shuidangran.top

[T58] Scala：函数定义
来源：http://gkn.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://paw.ivvv.top

[T59] Scala：循环
来源：http://bxa.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://zrv.zhixingplan.top

[T60] Scala：折叠
来源：http://xyp.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iad.ctjpmb.com

================================================================================
来源：http://hzp.sweek.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xcm.fzhhl.top

================================================================================
来源：http://zvk.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://wmk.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oei.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://luk.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://slf.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://gbq.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://grl.jqgfzy.top

[U04] Py：变量调试打印
来源：http://aov.zycfv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ngv.hesvh.cn

[U05] Py：列表去重且保序
来源：http://gng.daxiang520.top

list(dict.fromkeys(arr))
来源：http://pli.snrcjt.cn

[U06] Py：合并两个字典
来源：http://wkl.vqdsnc.cn

{**a, **b}
来源：http://uym.smart0.xyz

[U07] Py：反转字典键值
来源：http://rjs.yuxming.cn

{v: k for k, v in d.items()}
来源：http://agw.yuxming.cn

[U08] Py：展平二维列表
来源：http://exg.chenlongwang.top

[y for x in nested for y in x]
来源：http://yxn.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://vxa.kuanghao11.cn

max(d, key=d.get)
来源：http://kvj.yuxming.cn

[U10] Py：按值排序字典
来源：http://byi.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kiw.daxiang520.top

[U11] Py：生成器表达式
来源：http://uqh.redwolf501.top

(x * 2 for x in arr)
来源：http://ncz.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://vej.daxiang520.top

Counter(arr).most_common(3)
来源：http://vsq.zhengqikj.top

[U13] Py：固定长度队列
来源：http://ogx.jiagoushi.top

deque(maxlen=10)
来源：http://rbl.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://psm.quarkkingdee.top

defaultdict(list)
来源：http://jvt.hysaishi.cn

[U15] Py：高精度计时
来源：http://mic.9152youxi.cn

t = time.perf_counter()
来源：http://pxd.iojbl.cn

[U16] Py：命令行参数解析
来源：http://bqi.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uki.gogol.net.cn

[U17] Py：初始化日志
来源：http://dko.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://svy.cqqwz.cn

[U18] Py：预编译正则
来源：http://dss.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://mnm.hammf.cn

[U19] Py：正则替换带回调
来源：http://pfn.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tvy.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://oap.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://vkg.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://elr.havefunace.top

@contextlib.contextmanager
来源：http://puu.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://xbm.dashuyun.cn

list(zip(*m))
来源：http://fif.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://pav.haohaochexian.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://boe.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://kxz.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://euf.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://xkp.316326.xyz

csv.DictReader(f)
来源：http://kuj.yuxming.cn

[U26] Py：并发下载
来源：http://ivf.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://htz.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://okk.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://jpg.hnqzz.top

[U28] Py：类型别名
来源：http://mvl.fktsv.cn

UserId = int
来源：http://djl.aibaodan.cn


<!-- 参考信息 -->