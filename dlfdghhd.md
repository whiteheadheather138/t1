代发 wailian999

strlen(s)
来源：http://ghe.mhx1999.top

[S06] C：字符串比较
来源：http://fmi.tianlin.xyz

strcmp(a, b) == 0
来源：http://dig.cdnleiting.top

[S07] C：数组遍历求和
来源：http://smz.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cyp.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://icp.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fgt.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://ohg.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xco.daria6918.cn

[S10] C：指针与解引用
来源：http://ubx.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://ors.zdbjq.cn

[S11] C：逐行读文件
来源：http://ewo.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://yit.shangyingyoupin.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ixj.smart0.xyz

fclose(f);
来源：http://gvv.zhongyouzk.top

[S12] C：写文件
来源：http://uus.sxryk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cim.zhiwuduotai.top

[S13] C：宏定义
来源：http://ysc.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://stq.zycfv.cn

[S14] C：枚举
来源：http://xod.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://olh.cucudq.cn

[S15] C：类型转换
来源：http://kee.jianghu66.top

(double) a / b
来源：http://mxh.zhiwuduotai.top

[S16] C：位操作置位
来源：http://qcz.0kj1m.cn

x |= (1 << 3);
来源：http://ncd.zycfv.cn

[S17] C：安全拼接字符串
来源：http://wev.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gnq.zhiwuduotai.top

[S18] C：命令行参数
来源：http://wml.cucudq.cn

int main(int argc, char **argv)
来源：http://low.chenjidiqi.icu

[S19] C：快速排序
来源：http://szl.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://uby.hcnkem.com

[S20] C：二分查找
来源：http://jsx.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ofi.sweek.top

[S21] C：字符类别判断
来源：http://gou.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bgn.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://cws.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://trc.zhiwuduotai.top

[S23] C：随机数
来源：http://nlh.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zqp.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://unp.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ppu.tarul.cn

[S25] C：内存拷贝
来源：http://iff.zhongyouzk.top

memcpy(dst, src, n);
来源：http://rzk.ydjk.org.cn

[S26] C：内存清零
来源：http://xlu.tarul.cn

memset(a, 0, sizeof a);
来源：http://gat.chenzaomai.com

[S27] C：定义常量
来源：http://ddl.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://bgs.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://gpw.uphjek.com

static int counter = 0;
来源：http://ahl.kuanghao11.cn

[S29] C：变参函数
来源：http://qig.ppjwa.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jtp.316326.xyz

[S30] C：头文件保护
来源：http://guv.zycfv.cn

#ifndef X_H
来源：http://bbs.nwbrower.top

#define X_H
来源：http://xxl.gzhubu.top

#endif
来源：http://yah.ctjpmb.com

[S31] C++：Hello World
来源：http://jqn.pycfn.com

#include <iostream>
来源：http://hng.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://ppy.gzhubu.top

[S32] C++：字符串
来源：http://prd.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://hbc.zdbjq.cn

[S33] C++：vector 增删
来源：http://igl.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://frj.jianghu66.top

[S34] C++：遍历 vector
来源：http://sce.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://qif.tian-w.cn

[S35] C++：map
来源：http://dzb.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://izl.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://sui.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mva.vehdjk.com

[S37] C++：set
来源：http://zfc.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bya.quarkkingdee.top

[S38] C++：排序
来源：http://qap.tanke756.top

std::sort(v.begin(), v.end());
来源：http://gdb.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://ixq.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://stc.gaohongyu789.top

[S40] C++：查找元素
来源：http://uwc.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vrl.tianlin.xyz

[S41] C++：类与构造函数
来源：http://rgo.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ewi.pycfn.com

[S42] C++：继承与虚函数
来源：http://mwg.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://wkd.daxiang520.top

[S43] C++：智能指针
来源：http://ozk.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://esq.birdmap.top

[S44] C++：引用传参
来源：http://sqh.redwolf501.top

void inc(int &x) { ++x; }
来源：http://vhs.0kj1m.cn

[S45] C++：lambda
来源：http://rba.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://hfn.daria6918.cn

[S46] C++：函数模板
来源：http://prr.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://csy.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://byd.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dvl.iojbl.cn

[S48] C++：逐行读文件
来源：http://baj.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://sgh.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://wea.zhiwuduotai.top

[S49] C++：写文件
来源：http://ocj.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://szi.yfazqb.com

[S50] C++：格式化数字
来源：http://lls.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://irl.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://ipo.shuidangran.top

static_cast<double>(a) / b
来源：http://rdz.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://gsj.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://iad.hammf.cn

[S53] C++：移动语义
来源：http://ixv.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://vsn.zhengqikj.top

[S54] C++：异常处理
来源：http://qtv.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ehd.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://idl.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://plm.cucudq.cn

[S56] C++：optional
来源：http://baz.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zhb.dashuyun.cn

[S57] C++：编译期常量
来源：http://rey.zhijiandao.cn

constexpr int N = 10;
来源：http://apz.daxiang520.top

[S58] C++：命名空间
来源：http://okt.sweek.top

namespace ns { int f() { return 1; } }
来源：http://vcu.redwolf501.top

[S59] C++：静态断言
来源：http://cua.zdqjudy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://elm.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://gvr.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nyw.shzxlz.cn

================================================================================
来源：http://phs.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cai.xuanzx.com

================================================================================
来源：http://ydr.hammf.cn

[T01] Kotlin：Hello World
来源：http://agg.hywenlv.cn

println("Hello")
来源：http://zga.snrcjt.cn

[T02] Kotlin：变量
来源：http://gzp.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ulr.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://wlv.jinqigfzy.top

"值: $b"
来源：http://bif.ydzc1.top

[T04] Kotlin：空安全
来源：http://pfa.shzxlz.cn

val n: String? = null;  n?.length
来源：http://gdq.tanke756.top

[T05] Kotlin：when 表达式
来源：http://qko.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vbm.hongshengwenyu.top

[T06] Kotlin：集合映射
来源：http://yma.svipenyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zrr.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://qpx.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lyr.xingfuxueyuan.xyz

[T08] Kotlin：数据类
来源：http://dnz.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://jep.nanxinkj.top

[T09] Kotlin：扩展函数
来源：http://typ.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://xwf.gzhubu.top

[T10] Kotlin：默认参数
来源：http://zcj.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qut.sjlbkw.cn

[T11] Kotlin：协程
来源：http://yja.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xzu.tian-w.cn

[T12] Kotlin：解构声明
来源：http://ckq.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://ngk.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://tzv.redwolf501.top

val m = mapOf("a" to 1)
来源：http://xkj.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://buw.fktsv.cn

for (i in 1..10) println(i)
来源：http://xtq.meibo888.top

[T15] Kotlin：接口
来源：http://hty.hesvh.cn

interface Shape { fun area(): Double }
来源：http://muh.yangfankeji.com

[T16] Swift：Hello World
来源：http://ecv.zhaomingkeji.xyz

print("Hello")
来源：http://ewm.xylfe.cn

[T17] Swift：变量与常量
来源：http://lvd.zhongyouzk.top

var a = 1;  let b = 2
来源：http://ipk.ppjwa.cn

[T18] Swift：字符串插值
来源：http://tzi.zhixingplan.top

"值: \(b)"
来源：http://fhm.yangfankeji.com

[T19] Swift：可选绑定
来源：http://tkh.xinyue.icu

if let n = opt { print(n) }
来源：http://ysl.52xcode.cn

[T20] Swift：数组操作
来源：http://mxk.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vqq.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://tgp.iojbl.cn

for x in a { print(x) }
来源：http://bsg.vehdjk.com

[T22] Swift：字典
来源：http://kno.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pwk.guannengcc.top

[T23] Swift：函数
来源：http://rjy.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ohk.sysykeji.top

[T24] Swift：闭包
来源：http://lwr.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bgj.yanxiufei.cn

[T25] Swift：结构体
来源：http://bqu.chenzaomai.com

struct P { var x: Int }
来源：http://uab.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://qzu.hnqzz.top

class A: Base { override func f() {} }
来源：http://bsv.shuidangran.top

[T27] Swift：错误处理
来源：http://zst.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://qmy.havefunace.top

[T28] Swift：枚举
来源：http://exu.316326.xyz

enum Color { case red, green }
来源：http://nce.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://sjr.andypj.xyz

guard let x = opt else { return }
来源：http://pah.vehdjk.com

[T30] Swift：协议
来源：http://vok.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://dcp.pycfn.com

[T31] Lua：Hello World
来源：http://awn.hywenlv.cn

print("Hello")
来源：http://awz.jyoumei.cn

[T32] Lua：局部变量
来源：http://aqc.zhoulong.xyz

local a = 1
来源：http://wit.hywenlv.cn

[T33] Lua：表（数组）
来源：http://ydy.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ket.hesvh.cn

[T34] Lua：遍历表
来源：http://maj.yanxiufei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lzr.gotoacloud.top

[T35] Lua：字典表
来源：http://iyb.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://ekm.52xcode.cn

[T36] Lua：函数
来源：http://jgw.fengsongda.top

function add(a, b) return a + b end
来源：http://gkq.hammf.cn

[T37] Lua：字符串拼接
来源：http://lth.ydzc1.top

"a" .. "b"
来源：http://uct.nanxuanxn.top

[T38] Lua：条件
来源：http://bwd.daria6918.cn

if x > 0 then print("正") end
来源：http://nuu.andypj.xyz

[T39] Lua：模式匹配
来源：http://mjy.andypj.xyz

string.find(s, "%d+")
来源：http://liz.ehwqpu.com

[T40] Lua：元表
来源：http://lik.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://lul.kuanghao11.cn

[T41] Perl：Hello World
来源：http://jgb.uphjek.com

print "Hello\n";
来源：http://xxa.316326.xyz

[T42] Perl：变量类型
来源：http://qao.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rvs.ybcxt.top

[T43] Perl：字符串插值
来源：http://bfg.yanxiufei.cn

"值: $a"
来源：http://apc.hcnkem.com

[T44] Perl：条件
来源：http://zxm.316326.xyz

if ($a > 0) { print "正"; }
来源：http://vsk.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://fkp.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://uer.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://fym.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://axq.sysykeji.top

[T47] Perl：正则捕获
来源：http://qbn.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://but.hysaishi.cn

[T48] Perl：正则替换
来源：http://jyk.bjfxy.top

$s =~ s/old/new/g;
来源：http://qmh.zhixingplan.top

[T49] Perl：函数
来源：http://unk.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sbk.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://hmg.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yet.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://olm.shuidangran.top

[T51] Scala：Hello World
来源：http://scg.vehdjk.com

println("Hello")
来源：http://jal.svipenyu.cn

[T52] Scala：变量
来源：http://edy.shzxlz.cn

val a = 1;  var b = 2
来源：http://bhu.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://lqq.gaohongyu789.top

s"值: $b"
来源：http://qxd.hywenlv.cn

[T54] Scala：集合映射
来源：http://isg.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://diu.pycfn.com

[T55] Scala：集合过滤
来源：http://oib.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://vhy.yanxiufei.cn

[T56] Scala：样例类
来源：http://tqj.haohaochexian.top

case class User(name: String, age: Int)
来源：http://rsl.sufxvd.cn

[T57] Scala：模式匹配
来源：http://kwq.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hvp.jyoumei.cn

[T58] Scala：函数定义
来源：http://ukl.xziqi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lpb.c1oappe.top

[T59] Scala：循环
来源：http://oab.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://xgz.hesvh.cn

[T60] Scala：折叠
来源：http://ycp.yueranfly.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xnr.ehwqpu.com

================================================================================
来源：http://whn.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lnc.ppjwa.cn

================================================================================
来源：http://xdn.guannengcc.top

[U01] Py：创建虚拟环境
来源：http://kle.nanxinkj.top

python -m venv .venv && source .venv/bin/activate
来源：http://aag.zhaomingkeji.xyz

[U02] Py：导出 / 安装依赖
来源：http://cvl.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hbe.xylfe.cn

[U03] Py：加载 .env 配置
来源：http://mjw.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cpy.gotoacloud.top

[U04] Py：变量调试打印
来源：http://zho.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mcj.yj202588.top

[U05] Py：列表去重且保序
来源：http://rud.xziqi.cn

list(dict.fromkeys(arr))
来源：http://kmg.cheryme.top

[U06] Py：合并两个字典
来源：http://ajn.316326.xyz

{**a, **b}
来源：http://yee.snrcjt.cn

[U07] Py：反转字典键值
来源：http://uom.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://agf.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://yww.redwolf501.top

[y for x in nested for y in x]
来源：http://hwj.yj20258.top

[U09] Py：字典取最大值的键
来源：http://pps.daxiang520.top

max(d, key=d.get)
来源：http://cia.zdbjq.cn

[U10] Py：按值排序字典
来源：http://lkx.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mzk.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://yxi.zhaomingkeji.xyz

(x * 2 for x in arr)
来源：http://nyi.bbcook.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hbj.yj20258.top

Counter(arr).most_common(3)
来源：http://kkr.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://yhr.jianghu66.top

deque(maxlen=10)
来源：http://szh.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://ppf.sysykeji.top

defaultdict(list)
来源：http://tmk.jinyuanbaomall.cn

[U15] Py：高精度计时
来源：http://tzx.gaohongyu789.top

t = time.perf_counter()
来源：http://wog.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://yvq.nanxuanxn.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qyk.havefunace.top

[U17] Py：初始化日志
来源：http://tqn.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://dqe.chenzaomai.com

[U18] Py：预编译正则
来源：http://cnb.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://ymb.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://xfg.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zxx.sxryk.cn

[U20] Py：缓存函数结果
来源：http://pgb.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://mxo.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://owq.chenjidiqi.icu

@contextlib.contextmanager
来源：http://yfd.redwolf501.top

[U22] Py：矩阵转置
来源：http://jog.cdnleiting.top

list(zip(*m))
来源：http://riz.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://kap.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qjf.dashuyun.cn

[U24] Py：路径操作
来源：http://hxc.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://noj.chenjidiqi.icu

[U25] Py：CSV 按字典读
来源：http://tav.jinghuilouyu.cn

csv.DictReader(f)
来源：http://cgy.yvedp.cn

[U26] Py：并发下载
来源：http://jta.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://laf.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://gzw.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://iip.fktsv.cn

[U28] Py：类型别名
来源：http://gfv.wangshuangyany.cn

UserId = int
来源：http://nuv.316326.xyz


<!-- 参考信息 -->