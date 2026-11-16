代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zdp.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://zfe.ppjwa.cn

time ./run.sh
来源：http://tbm.yueranfly.top

================================================================================
来源：http://szf.guowangkeji.top

S. C / C++ 专题
来源：http://jzk.zhengqikj.top

================================================================================
来源：http://hag.quarkkingdee.top

[S01] C：Hello World
来源：http://goa.xuetiantiany.cn

#include <stdio.h>
来源：http://mkp.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pjd.52xcode.cn

[S02] C：变量与格式化输出
来源：http://ozi.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://udl.epnwcf.com

[S03] C：读入整数
来源：http://nnr.vehdjk.com

int x; scanf("%d", &x);
来源：http://xsc.yongpay.top

[S04] C：字符串复制
来源：http://dml.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://quw.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://pcw.yongpay.top

strlen(s)
来源：http://sci.meibo888.top

[S06] C：字符串比较
来源：http://olc.zhengqikj.top

strcmp(a, b) == 0
来源：http://dey.ctjpmb.com

[S07] C：数组遍历求和
来源：http://ypl.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hap.daxiang520.top

[S08] C：动态内存分配与释放
来源：http://pvz.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wit.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://gps.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tuq.daria6918.cn

[S10] C：指针与解引用
来源：http://emk.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://rgv.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://byr.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://uiw.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uki.chenzaomai.com

fclose(f);
来源：http://zfy.sweek.top

[S12] C：写文件
来源：http://fra.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jog.cqqwz.cn

[S13] C：宏定义
来源：http://icc.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iow.shanyushiyangtech.top

[S14] C：枚举
来源：http://sjr.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://frr.yuanzhike.top

[S15] C：类型转换
来源：http://zsi.zycfv.cn

(double) a / b
来源：http://zlv.yonumen.top

[S16] C：位操作置位
来源：http://lmx.shanyushiyangtech.top

x |= (1 << 3);
来源：http://rcy.hnqzz.top

[S17] C：安全拼接字符串
来源：http://qih.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sxj.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://wby.sufxvd.cn

int main(int argc, char **argv)
来源：http://cgu.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://gwz.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://rmg.fktsv.cn

[S20] C：二分查找
来源：http://lud.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sfs.zhengqikj.top

[S21] C：字符类别判断
来源：http://htw.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tpx.jiagoushi.top

[S22] C：字符串转数字
来源：http://ulb.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hns.haohaochexian.top

[S23] C：随机数
来源：http://iki.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zit.yangfankeji.com

[S24] C：获取本地时间
来源：http://tbv.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cri.hysaishi.cn

[S25] C：内存拷贝
来源：http://opt.ydjk.org.cn

memcpy(dst, src, n);
来源：http://xja.smart0.xyz

[S26] C：内存清零
来源：http://tgr.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://wtw.kuanghao11.cn

[S27] C：定义常量
来源：http://hey.nanxinkj.top

const double PI = 3.14159;
来源：http://ouz.9152youxi.cn

[S28] C：静态变量
来源：http://pxj.hesvh.cn

static int counter = 0;
来源：http://vkj.jinqigufen.top

[S29] C：变参函数
来源：http://twx.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nnf.shuidangran.top

[S30] C：头文件保护
来源：http://ahx.hnxiangtu.top

#ifndef X_H
来源：http://iik.sufxvd.cn

#define X_H
来源：http://dkh.gaohongyu789.top

#endif
来源：http://yja.yongpay.top

[S31] C++：Hello World
来源：http://gkc.yj20258.top

#include <iostream>
来源：http://wsn.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://dbl.zdqjudy.top

[S32] C++：字符串
来源：http://hwh.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://ujd.zhixingplan.top

[S33] C++：vector 增删
来源：http://zbf.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zvd.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://zwn.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://kbt.yanxiufei.cn

[S35] C++：map
来源：http://aii.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ecv.ybcxt.top

[S36] C++：unordered_map
来源：http://nbs.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://smk.tarul.cn

[S37] C++：set
来源：http://sth.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://por.shuidangran.top

[S38] C++：排序
来源：http://xpi.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://ata.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://bye.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ler.ehwqpu.com

[S40] C++：查找元素
来源：http://cid.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fnp.ivvv.top

[S41] C++：类与构造函数
来源：http://wca.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bdq.c1oappe.top

[S42] C++：继承与虚函数
来源：http://ely.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://zeq.wangshuangyany.cn

[S43] C++：智能指针
来源：http://qhb.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://vcw.zhixingplan.top

[S44] C++：引用传参
来源：http://cav.sysykeji.top

void inc(int &x) { ++x; }
来源：http://lug.zhijiandao.cn

[S45] C++：lambda
来源：http://omn.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://dym.yuanzhike.top

[S46] C++：函数模板
来源：http://vhu.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uha.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://crs.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qrs.aibaodan.cn

[S48] C++：逐行读文件
来源：http://sln.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://jab.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://wgs.yj20258888.top

[S49] C++：写文件
来源：http://smh.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://spa.hesvh.cn

[S50] C++：格式化数字
来源：http://wxt.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kql.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://lqo.zhengqikj.top

static_cast<double>(a) / b
来源：http://aoe.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://tyy.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://rca.dianchejie.cn

[S53] C++：移动语义
来源：http://jhx.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://gdc.yvedp.cn

[S54] C++：异常处理
来源：http://pkf.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wbo.yueranfly.top

[S55] C++：结构化绑定
来源：http://uwn.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lcm.cqqwz.cn

[S56] C++：optional
来源：http://enp.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qhv.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://ioj.ctjpmb.com

constexpr int N = 10;
来源：http://hfz.zhengqikj.top

[S58] C++：命名空间
来源：http://aqq.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://lsl.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://lqf.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mzw.yongpay.top

[S60] C++：遍历并删除元素
来源：http://mfc.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sje.ydjk.org.cn

================================================================================
来源：http://ktu.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gri.yj202588.top

================================================================================
来源：http://kmh.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://qgs.yj20258.top

println("Hello")
来源：http://gmg.jqgfzy.top

[T02] Kotlin：变量
来源：http://xwz.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jqn.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://nlz.yanxiufei.cn

"值: $b"
来源：http://atp.epnwcf.com

[T04] Kotlin：空安全
来源：http://fam.ctjpmb.com

val n: String? = null;  n?.length
来源：http://ffi.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://awu.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jib.hnqzz.top

[T06] Kotlin：集合映射
来源：http://ban.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hsb.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://gsu.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tvt.redwolf501.top

[T08] Kotlin：数据类
来源：http://ozq.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://dmp.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://tpw.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://ptx.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://wzi.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://fid.guowangkeji.top

[T11] Kotlin：协程
来源：http://brg.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kxi.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://liq.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://osi.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://dwp.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://poh.gzhubu.top

[T14] Kotlin：循环
来源：http://let.tianlin.xyz

for (i in 1..10) println(i)
来源：http://ciy.guowangkeji.top

[T15] Kotlin：接口
来源：http://nit.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://gnb.gotoacloud.top

[T16] Swift：Hello World
来源：http://ipu.jinqigufen.top

print("Hello")
来源：http://fbi.dashuyun.cn

[T17] Swift：变量与常量
来源：http://xga.yongpay.top

var a = 1;  let b = 2
来源：http://zqi.nanxinkj.top

[T18] Swift：字符串插值
来源：http://oxo.shanyushiyangkeji.top

"值: \(b)"
来源：http://zyg.vehdjk.com

[T19] Swift：可选绑定
来源：http://osl.cqqwz.cn

if let n = opt { print(n) }
来源：http://rsz.fzhhl.top

[T20] Swift：数组操作
来源：http://yxp.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://rbs.cheryme.top

[T21] Swift：遍历
来源：http://sle.bbcook.cn

for x in a { print(x) }
来源：http://uby.vqdsnc.cn

[T22] Swift：字典
来源：http://spp.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://lkv.hcnkem.com

[T23] Swift：函数
来源：http://gjy.ybcxt.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kay.nanxinkj.top

[T24] Swift：闭包
来源：http://jzb.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://wvc.wangdashe.top

[T25] Swift：结构体
来源：http://vqz.hfpthk.cn

struct P { var x: Int }
来源：http://mom.andypj.xyz

[T26] Swift：类与重写
来源：http://tnm.ydzc1.top

class A: Base { override func f() {} }
来源：http://ykh.xylfe.cn

[T27] Swift：错误处理
来源：http://vbq.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://hdr.52xcode.cn

[T28] Swift：枚举
来源：http://amo.birdmap.top

enum Color { case red, green }
来源：http://ixi.pycfn.com

[T29] Swift：guard 提前返回
来源：http://tqg.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://qpv.uphjek.com

[T30] Swift：协议
来源：http://dwf.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://qrw.xuanzx.com

[T31] Lua：Hello World
来源：http://msg.pengpengdd.cyou

print("Hello")
来源：http://pni.birdmap.top

[T32] Lua：局部变量
来源：http://ezc.hfpthk.cn

local a = 1
来源：http://xcj.daxiang520.top

[T33] Lua：表（数组）
来源：http://fbt.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://vdu.yj202588.top

[T34] Lua：遍历表
来源：http://wtg.ydzc1.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tcr.yuanzhike.top

[T35] Lua：字典表
来源：http://vcx.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://bta.0kj1m.cn

[T36] Lua：函数
来源：http://dyu.sweek.top

function add(a, b) return a + b end
来源：http://qrn.cheryme.top

[T37] Lua：字符串拼接
来源：http://zvb.yangfankeji.com

"a" .. "b"
来源：http://gpi.sxryk.cn

[T38] Lua：条件
来源：http://wmg.hesvh.cn

if x > 0 then print("正") end
来源：http://bhq.316326.xyz

[T39] Lua：模式匹配
来源：http://ozo.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://wqx.316326.xyz

[T40] Lua：元表
来源：http://dft.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://zjk.hesvh.cn

[T41] Perl：Hello World
来源：http://ddm.yfazqb.com

print "Hello\n";
来源：http://uls.epnwcf.com

[T42] Perl：变量类型
来源：http://zgd.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hls.xuanzx.com

[T43] Perl：字符串插值
来源：http://dco.c1oappe.top

"值: $a"
来源：http://zpu.shanyushiyangtech.top

[T44] Perl：条件
来源：http://mao.zycfv.cn

if ($a > 0) { print "正"; }
来源：http://dzh.nwbrower.top

[T45] Perl：数组遍历
来源：http://lll.jqgfzy.top

for my $x (@arr) { print $x; }
来源：http://llh.gogol.net.cn

[T46] Perl：哈希操作
来源：http://qpn.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mou.yj20258.top

[T47] Perl：正则捕获
来源：http://qdx.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rpv.cqqwz.cn

[T48] Perl：正则替换
来源：http://wxj.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://amj.jqgfzy.top

[T49] Perl：函数
来源：http://zrs.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lxa.yfazqb.com

[T50] Perl：逐行读文件
来源：http://qhz.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ppz.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://gca.hysaishi.cn

[T51] Scala：Hello World
来源：http://ksn.aizwys.cn

println("Hello")
来源：http://ncp.snrcjt.cn

[T52] Scala：变量
来源：http://wie.shuidangran.top

val a = 1;  var b = 2
来源：http://yqz.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://pnp.zycfv.cn

s"值: $b"
来源：http://evm.havefunace.top

[T54] Scala：集合映射
来源：http://hmw.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://nan.cashguo.top

[T55] Scala：集合过滤
来源：http://dpc.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://obs.bjfxy.top

[T56] Scala：样例类
来源：http://lfg.yj20258.top

case class User(name: String, age: Int)
来源：http://stb.chenlongwang.top

[T57] Scala：模式匹配
来源：http://qfj.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://add.gzhubu.top

[T58] Scala：函数定义
来源：http://cqz.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://pym.wangdashe.top

[T59] Scala：循环
来源：http://fnd.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://ugc.vehdjk.com

[T60] Scala：折叠
来源：http://hmf.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xfx.hongshengwenyu.top

================================================================================
来源：http://lgi.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mbf.aibaodan.cn

================================================================================
来源：http://xpg.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://hop.snrcjt.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sfp.ybcxt.top

[U02] Py：导出 / 安装依赖
来源：http://fxu.meibo888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fpp.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://gbb.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lab.jiagoushi.top

[U04] Py：变量调试打印
来源：http://bws.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hno.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://kzw.yvedp.cn

list(dict.fromkeys(arr))
来源：http://kxi.xziqi.cn

[U06] Py：合并两个字典
来源：http://aoi.ivvv.top

{**a, **b}
来源：http://lbt.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://zlf.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://kmr.sysykeji.top

[U08] Py：展平二维列表
来源：http://got.daxiang520.top

[y for x in nested for y in x]
来源：http://nic.cqqwz.cn

[U09] Py：字典取最大值的键
来源：http://nho.epnwcf.com

max(d, key=d.get)
来源：http://xjf.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://jaf.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://izg.sufxvd.cn

[U11] Py：生成器表达式
来源：http://mli.chenlongwang.top

(x * 2 for x in arr)
来源：http://eop.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wtj.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://cgf.jqgfzy.top

[U13] Py：固定长度队列
来源：http://kws.daxiang520.top

deque(maxlen=10)
来源：http://czp.havefunace.top

[U14] Py：分组收集到列表
来源：http://mmh.aibaodan.cn

defaultdict(list)
来源：http://rxg.shzxlz.cn

[U15] Py：高精度计时
来源：http://hys.uphjek.com

t = time.perf_counter()
来源：http://qdo.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://tbs.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fav.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://ivw.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://dqc.redwolf501.top

[U18] Py：预编译正则
来源：http://axr.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://gbx.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://aft.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vgf.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://lmu.wangshuangyany.cn

@functools.lru_cache(maxsize=None)
来源：http://cnj.zhengqikj.top


<!-- 参考信息 -->