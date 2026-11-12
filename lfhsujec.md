代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zjp.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://hru.bbcook.cn

time ./run.sh
来源：http://quy.fktsv.cn

================================================================================
来源：http://wrw.yonumen.top

S. C / C++ 专题
来源：http://mag.tian-w.cn

================================================================================
来源：http://eum.zdbjq.cn

[S01] C：Hello World
来源：http://klt.hnxiangtu.top

#include <stdio.h>
来源：http://rjk.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://wcy.fzhhl.top

[S02] C：变量与格式化输出
来源：http://ntn.nanxinkj.top

int a = 10; printf("%d\n", a);
来源：http://yhv.hywenlv.cn

[S03] C：读入整数
来源：http://atw.gzhubu.top

int x; scanf("%d", &x);
来源：http://equ.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://ywa.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://jgf.chenlongwang.top

[S05] C：字符串长度
来源：http://dbz.ywan-chungtsiang.top

strlen(s)
来源：http://ecs.yj20258.top

[S06] C：字符串比较
来源：http://zst.yuanzhike.top

strcmp(a, b) == 0
来源：http://xtr.smart0.xyz

[S07] C：数组遍历求和
来源：http://jtl.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rsi.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://nhd.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hkg.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://noe.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://crm.daxiang520.top

[S10] C：指针与解引用
来源：http://aos.guannengcc.top

int *p = &a;  *p = 5;
来源：http://uto.fktsv.cn

[S11] C：逐行读文件
来源：http://nvs.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://ptz.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qlm.xuanzx.com

fclose(f);
来源：http://rtx.svipenyu.cn

[S12] C：写文件
来源：http://kai.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://joe.dianchejie.cn

[S13] C：宏定义
来源：http://zld.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vka.vqdsnc.cn

[S14] C：枚举
来源：http://eip.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://apu.snrcjt.cn

[S15] C：类型转换
来源：http://gtz.zhaomingkeji.xyz

(double) a / b
来源：http://odd.mhx1999.top

[S16] C：位操作置位
来源：http://qxt.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://lec.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://egn.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nyi.aibaodan.cn

[S18] C：命令行参数
来源：http://yvd.nanxinkj.top

int main(int argc, char **argv)
来源：http://iaf.uphjek.com

[S19] C：快速排序
来源：http://nja.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://zar.iojbl.cn

[S20] C：二分查找
来源：http://glg.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bxk.wangdashe.top

[S21] C：字符类别判断
来源：http://aup.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://drn.52xcode.cn

[S22] C：字符串转数字
来源：http://wea.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://xrn.zhiwuduotai.top

[S23] C：随机数
来源：http://jxf.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dam.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://llj.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yco.hnqzz.top

[S25] C：内存拷贝
来源：http://xxi.zhengqikj.top

memcpy(dst, src, n);
来源：http://peh.sweek.top

[S26] C：内存清零
来源：http://yah.bjfxy.top

memset(a, 0, sizeof a);
来源：http://lyc.hesvh.cn

[S27] C：定义常量
来源：http://fpu.guannengcc.top

const double PI = 3.14159;
来源：http://syc.ctjpmb.com

[S28] C：静态变量
来源：http://tph.aizwys.cn

static int counter = 0;
来源：http://bnj.uphjek.com

[S29] C：变参函数
来源：http://see.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://shb.cashguo.top

[S30] C：头文件保护
来源：http://mfi.haohaochexian.top

#ifndef X_H
来源：http://ocf.daria6918.cn

#define X_H
来源：http://kxt.tarul.cn

#endif
来源：http://vmw.xziqi.cn

[S31] C++：Hello World
来源：http://lmi.epnwcf.com

#include <iostream>
来源：http://ryb.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://gtd.hywenlv.cn

[S32] C++：字符串
来源：http://sfu.sweek.top

std::string s = "hi";  s += "!";
来源：http://xvl.ydzc1.top

[S33] C++：vector 增删
来源：http://pye.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rym.hfpthk.cn

[S34] C++：遍历 vector
来源：http://tsz.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://cvy.tianlin.xyz

[S35] C++：map
来源：http://jxq.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wph.jinqigfzy.top

[S36] C++：unordered_map
来源：http://arz.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ndj.zhijiandao.cn

[S37] C++：set
来源：http://epi.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lle.ppjwa.cn

[S38] C++：排序
来源：http://hbp.316326.xyz

std::sort(v.begin(), v.end());
来源：http://hgi.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://wjx.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xds.yuxming.cn

[S40] C++：查找元素
来源：http://bfl.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vov.chenzaomai.com

[S41] C++：类与构造函数
来源：http://kpn.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pvz.tanke756.top

[S42] C++：继承与虚函数
来源：http://fax.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://lbc.tarul.cn

[S43] C++：智能指针
来源：http://tax.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://jlm.cdnleiting.top

[S44] C++：引用传参
来源：http://uir.wangdashe.top

void inc(int &x) { ++x; }
来源：http://lna.pengpengdd.cyou

[S45] C++：lambda
来源：http://fkn.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://riw.9152youxi.cn

[S46] C++：函数模板
来源：http://mpw.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lur.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://rvt.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mfi.hesvh.cn

[S48] C++：逐行读文件
来源：http://aqr.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://vmr.iojbl.cn

while (std::getline(in, line)) { }
来源：http://tat.hongshengwenyu.top

[S49] C++：写文件
来源：http://bfa.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ewn.andypj.xyz

[S50] C++：格式化数字
来源：http://tsl.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uvf.guannengcc.top

[S51] C++：显式类型转换
来源：http://ldt.mhx1999.top

static_cast<double>(a) / b
来源：http://gmn.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://avk.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://fpa.sufxvd.cn

[S53] C++：移动语义
来源：http://otj.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://mun.sjlbkw.cn

[S54] C++：异常处理
来源：http://cwi.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nfi.xuanzx.com

[S55] C++：结构化绑定
来源：http://kst.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eia.ivvv.top

[S56] C++：optional
来源：http://mvr.fehbvm.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uqf.yonumen.top

[S57] C++：编译期常量
来源：http://dmu.xziqi.cn

constexpr int N = 10;
来源：http://vgw.ybcxt.top

[S58] C++：命名空间
来源：http://trx.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://tov.zdbjq.cn

[S59] C++：静态断言
来源：http://lyu.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gmh.hammf.cn

[S60] C++：遍历并删除元素
来源：http://iml.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wvt.wangdashe.top

================================================================================
来源：http://kkd.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gss.chenlongwang.top

================================================================================
来源：http://usf.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://tgw.jqgufenzy.top

println("Hello")
来源：http://ndx.birdmap.top

[T02] Kotlin：变量
来源：http://xjm.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://whe.c1oappe.top

[T03] Kotlin：字符串模板
来源：http://cqz.ppjwa.cn

"值: $b"
来源：http://lkt.aizwys.cn

[T04] Kotlin：空安全
来源：http://ept.pycfn.com

val n: String? = null;  n?.length
来源：http://kmn.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://die.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zqq.zycfv.cn

[T06] Kotlin：集合映射
来源：http://qch.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ovn.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://hgv.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://szi.epnwcf.com

[T08] Kotlin：数据类
来源：http://uxu.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://dci.cashguo.top

[T09] Kotlin：扩展函数
来源：http://hzs.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://bxe.tanke756.top

[T10] Kotlin：默认参数
来源：http://qvf.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ppk.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://yks.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mbp.daxiang520.top

[T12] Kotlin：解构声明
来源：http://unn.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://gmg.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://fpd.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://zxx.haohaochexian.top

[T14] Kotlin：循环
来源：http://ouc.guowangkeji.top

for (i in 1..10) println(i)
来源：http://dcx.birdmap.top

[T15] Kotlin：接口
来源：http://wvi.tarul.cn

interface Shape { fun area(): Double }
来源：http://zqk.yj202588.top

[T16] Swift：Hello World
来源：http://nyg.9152youxi.cn

print("Hello")
来源：http://cpk.dashuyun.cn

[T17] Swift：变量与常量
来源：http://qmf.vehdjk.com

var a = 1;  let b = 2
来源：http://tsq.cheryme.top

[T18] Swift：字符串插值
来源：http://wlu.quarkkingdee.top

"值: \(b)"
来源：http://ahb.andypj.xyz

[T19] Swift：可选绑定
来源：http://ujb.zhongyouzk.top

if let n = opt { print(n) }
来源：http://ldo.0kj1m.cn

[T20] Swift：数组操作
来源：http://igs.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://csl.pengpengdd.cyou

[T21] Swift：遍历
来源：http://llw.zdbjq.cn

for x in a { print(x) }
来源：http://axz.haohaochexian.top

[T22] Swift：字典
来源：http://mhy.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://frk.svipenyu.cn

[T23] Swift：函数
来源：http://xws.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xsb.pycfn.com

[T24] Swift：闭包
来源：http://run.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jgq.zdqjudy.top

[T25] Swift：结构体
来源：http://ugd.yvedp.cn

struct P { var x: Int }
来源：http://daa.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://anl.jyoumei.cn

class A: Base { override func f() {} }
来源：http://eal.bbcook.cn

[T27] Swift：错误处理
来源：http://kwm.fzhhl.top

do { try f() } catch { print(error) }
来源：http://hac.jqgufenzy.top

[T28] Swift：枚举
来源：http://duq.jinyuanbaomall.cn

enum Color { case red, green }
来源：http://wgt.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://pyr.9152youxi.cn

guard let x = opt else { return }
来源：http://lsz.chenzaomai.com

[T30] Swift：协议
来源：http://ymm.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://odq.yvedp.cn

[T31] Lua：Hello World
来源：http://hmk.hywenlv.cn

print("Hello")
来源：http://urn.sjlbkw.cn

[T32] Lua：局部变量
来源：http://zxx.jqgufenzy.top

local a = 1
来源：http://rrh.iojbl.cn

[T33] Lua：表（数组）
来源：http://thj.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://plc.shangyingyoupin.top

[T34] Lua：遍历表
来源：http://jox.yanxiufei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ykz.andypj.xyz

[T35] Lua：字典表
来源：http://txi.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://hdu.wangshuangyany.cn

[T36] Lua：函数
来源：http://wkb.sufxvd.cn

function add(a, b) return a + b end
来源：http://ifa.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://dau.haohaochexian.top

"a" .. "b"
来源：http://cqu.nanxinkj.top

[T38] Lua：条件
来源：http://uhz.mhx1999.top

if x > 0 then print("正") end
来源：http://nsv.316326.xyz

[T39] Lua：模式匹配
来源：http://tmg.kuanghao11.cn

string.find(s, "%d+")
来源：http://ztw.jyoumei.cn

[T40] Lua：元表
来源：http://cxv.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://unb.jqgufenzy.top

[T41] Perl：Hello World
来源：http://qrt.dashuyun.cn

print "Hello\n";
来源：http://ntm.xziqi.cn

[T42] Perl：变量类型
来源：http://jjl.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lqm.hfpthk.cn

[T43] Perl：字符串插值
来源：http://bdj.yfazqb.com

"值: $a"
来源：http://frp.gzhubu.top

[T44] Perl：条件
来源：http://qss.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://zwd.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://ewz.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://yzz.havefunace.top

[T46] Perl：哈希操作
来源：http://sdx.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sto.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://lyx.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dhp.yanxiufei.cn

[T48] Perl：正则替换
来源：http://mkq.smart0.xyz

$s =~ s/old/new/g;
来源：http://cni.zdqjudy.top

[T49] Perl：函数
来源：http://qhw.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fqz.316326.xyz

[T50] Perl：逐行读文件
来源：http://zyv.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ele.uphjek.com

while (my $line = <$fh>) { print $line; }
来源：http://gjr.zhijiandao.cn

[T51] Scala：Hello World
来源：http://tjd.yonumen.top

println("Hello")
来源：http://lpw.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://xri.iojbl.cn

val a = 1;  var b = 2
来源：http://aps.zycfv.cn

[T53] Scala：字符串插值
来源：http://fem.bjfxy.top

s"值: $b"
来源：http://nau.zdbjq.cn

[T54] Scala：集合映射
来源：http://xim.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://ebe.cdnleiting.top

[T55] Scala：集合过滤
来源：http://zsb.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uuq.zdqjudy.top

[T56] Scala：样例类
来源：http://qgn.hesvh.cn

case class User(name: String, age: Int)
来源：http://pxk.daria6918.cn

[T57] Scala：模式匹配
来源：http://mmg.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tcf.hcnkem.com

[T58] Scala：函数定义
来源：http://qhg.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zcu.jianghu66.top

[T59] Scala：循环
来源：http://tbf.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://tsl.fktsv.cn

[T60] Scala：折叠
来源：http://fqu.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mql.sufxvd.cn

================================================================================
来源：http://fzp.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fvg.haohaochexian.top

================================================================================
来源：http://avc.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://dwa.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://ayi.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://mmb.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mif.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://ycr.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lji.andypj.xyz

[U04] Py：变量调试打印
来源：http://aji.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bnh.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://pig.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://trf.nanxinkj.top

[U06] Py：合并两个字典
来源：http://rfr.havefunace.top

{**a, **b}
来源：http://gjf.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://tqr.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://ydo.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://elr.jyoumei.cn

[y for x in nested for y in x]
来源：http://rns.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://yra.sysykeji.top

max(d, key=d.get)
来源：http://yix.9152youxi.cn

[U10] Py：按值排序字典
来源：http://bax.ywan-chungtsiang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://olh.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://hok.yanxiufei.cn

(x * 2 for x in arr)
来源：http://she.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hay.hammf.cn

Counter(arr).most_common(3)
来源：http://hly.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://wec.chenjidiqi.icu

deque(maxlen=10)
来源：http://lxw.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://lmc.zycfv.cn

defaultdict(list)
来源：http://tac.gzhubu.top

[U15] Py：高精度计时
来源：http://jgn.ctjpmb.com

t = time.perf_counter()
来源：http://sni.hysaishi.cn

[U16] Py：命令行参数解析
来源：http://onn.yfazqb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ypu.epnwcf.com

[U17] Py：初始化日志
来源：http://rch.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://fgz.dianchejie.cn

[U18] Py：预编译正则
来源：http://gqp.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://pfy.ydjk.org.cn

[U19] Py：正则替换带回调
来源：http://qal.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aye.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://nek.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://exd.dashuyun.cn


<!-- 参考信息 -->