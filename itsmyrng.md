代发 wailian999

read -rp "请输入: " ans
来源：http://mkl.tanke756.top

[R78] 交互式菜单
来源：http://cms.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rci.jinqigfzy.top

[R79] 解析命令行选项
来源：http://wvq.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ooh.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://fvb.yuanzhike.top

time ./run.sh
来源：http://bph.fengsongda.top

================================================================================
来源：http://dsn.c1oappe.top

S. C / C++ 专题
来源：http://ahd.jinqigfzy.top

================================================================================
来源：http://rba.ivvv.top

[S01] C：Hello World
来源：http://ibm.hnqzz.top

#include <stdio.h>
来源：http://egl.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://clk.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://niu.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://qvt.wangdashe.top

[S03] C：读入整数
来源：http://sss.daxiang520.top

int x; scanf("%d", &x);
来源：http://agn.epnwcf.com

[S04] C：字符串复制
来源：http://unw.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bav.hnxiangtu.top

[S05] C：字符串长度
来源：http://sda.hongshengwenyu.top

strlen(s)
来源：http://ose.jqgfzy.top

[S06] C：字符串比较
来源：http://mgt.redwolf501.top

strcmp(a, b) == 0
来源：http://twk.ivvv.top

[S07] C：数组遍历求和
来源：http://zqm.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fvz.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://vcc.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vsu.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://goc.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qnc.fengsongda.top

[S10] C：指针与解引用
来源：http://ouk.yuxming.cn

int *p = &a;  *p = 5;
来源：http://who.fengsongda.top

[S11] C：逐行读文件
来源：http://slb.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://xtp.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://xra.zhaomingkeji.xyz

fclose(f);
来源：http://kit.fanxiaobao.xyz

[S12] C：写文件
来源：http://liq.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zdm.gzhubu.top

[S13] C：宏定义
来源：http://bse.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ozg.yj20258888.top

[S14] C：枚举
来源：http://bjg.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://vwg.guowangkeji.top

[S15] C：类型转换
来源：http://vih.bjfxy.top

(double) a / b
来源：http://npa.jinqigfzy.top

[S16] C：位操作置位
来源：http://sys.jinqigfzy.top

x |= (1 << 3);
来源：http://kdz.daria6918.cn

[S17] C：安全拼接字符串
来源：http://lpu.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nhq.jiagoushi.top

[S18] C：命令行参数
来源：http://lsm.yvedp.cn

int main(int argc, char **argv)
来源：http://qyr.smart0.xyz

[S19] C：快速排序
来源：http://dyg.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://byc.yueranfly.top

[S20] C：二分查找
来源：http://eay.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gpe.andypj.xyz

[S21] C：字符类别判断
来源：http://wts.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cdk.shuidangran.top

[S22] C：字符串转数字
来源：http://ech.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tbr.ydzc1.top

[S23] C：随机数
来源：http://bsk.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://kwo.jqgfzy.top

[S24] C：获取本地时间
来源：http://xsm.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bre.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://mbv.ppjwa.cn

memcpy(dst, src, n);
来源：http://lwc.fanxiaobao.xyz

[S26] C：内存清零
来源：http://gnw.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://ejx.yj20258.top

[S27] C：定义常量
来源：http://ydj.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://hpj.bjfxy.top

[S28] C：静态变量
来源：http://xwy.jinyuanbaomall.cn

static int counter = 0;
来源：http://itv.tanke756.top

[S29] C：变参函数
来源：http://ybr.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zqr.yongpay.top

[S30] C：头文件保护
来源：http://eda.sufxvd.cn

#ifndef X_H
来源：http://pll.havefunace.top

#define X_H
来源：http://eud.uphjek.com

#endif
来源：http://yfz.jqgfzy.top

[S31] C++：Hello World
来源：http://aww.zdbjq.cn

#include <iostream>
来源：http://ceg.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://jkj.cheryme.top

[S32] C++：字符串
来源：http://cts.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://vlf.ppjwa.cn

[S33] C++：vector 增删
来源：http://ita.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ukl.andypj.xyz

[S34] C++：遍历 vector
来源：http://fdx.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://lwu.c1oappe.top

[S35] C++：map
来源：http://zsw.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lgz.ctjpmb.com

[S36] C++：unordered_map
来源：http://neq.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cjx.jinghuilouyu.cn

[S37] C++：set
来源：http://tsv.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jbv.ppjwa.cn

[S38] C++：排序
来源：http://xvk.fktsv.cn

std::sort(v.begin(), v.end());
来源：http://vpc.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://auv.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://twp.xuetiantiany.cn

[S40] C++：查找元素
来源：http://jdp.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mvx.bbcook.cn

[S41] C++：类与构造函数
来源：http://mlb.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cka.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://wpa.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://mhj.yj20258888.top

[S43] C++：智能指针
来源：http://nya.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://cxe.gzhubu.top

[S44] C++：引用传参
来源：http://srk.hnqzz.top

void inc(int &x) { ++x; }
来源：http://rxn.hywenlv.cn

[S45] C++：lambda
来源：http://gka.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://jxw.fehbvm.com

[S46] C++：函数模板
来源：http://bsv.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wqs.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://agy.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jbt.daxiang520.top

[S48] C++：逐行读文件
来源：http://tzv.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://hgb.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://php.jyoumei.cn

[S49] C++：写文件
来源：http://wky.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rwo.cheryme.top

[S50] C++：格式化数字
来源：http://psx.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hjt.hysaishi.cn

[S51] C++：显式类型转换
来源：http://qci.tarul.cn

static_cast<double>(a) / b
来源：http://klf.havefunace.top

[S52] C++：const 与 noexcept
来源：http://qid.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://nhn.pycfn.com

[S53] C++：移动语义
来源：http://mgl.ivvv.top

std::vector<int> w = std::move(v);
来源：http://nil.hywenlv.cn

[S54] C++：异常处理
来源：http://gbp.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dyz.tarul.cn

[S55] C++：结构化绑定
来源：http://bcc.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://rkc.52xcode.cn

[S56] C++：optional
来源：http://min.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uvg.daria6918.cn

[S57] C++：编译期常量
来源：http://aqh.cucudq.cn

constexpr int N = 10;
来源：http://pla.hongshengwenyu.top

[S58] C++：命名空间
来源：http://nge.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://kir.cqqwz.cn

[S59] C++：静态断言
来源：http://dju.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oji.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://ssp.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://swv.redwolf501.top

================================================================================
来源：http://aav.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wzi.shuidangran.top

================================================================================
来源：http://vky.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://uww.jqgfzy.top

println("Hello")
来源：http://hxf.cheryme.top

[T02] Kotlin：变量
来源：http://odq.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mqp.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://dji.xuanzx.com

"值: $b"
来源：http://ari.quarkkingdee.top

[T04] Kotlin：空安全
来源：http://gei.sysykeji.top

val n: String? = null;  n?.length
来源：http://yto.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://tso.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ecf.316326.xyz

[T06] Kotlin：集合映射
来源：http://zpy.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ckm.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://eiy.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://twy.meibo888.top

[T08] Kotlin：数据类
来源：http://xqx.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://slz.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://fnv.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://ygz.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://his.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zyl.xuanzx.com

[T11] Kotlin：协程
来源：http://bpm.yj20258.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mys.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://yiv.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://tbf.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://tyj.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://fex.zdqjudy.top

[T14] Kotlin：循环
来源：http://osr.ydzc1.top

for (i in 1..10) println(i)
来源：http://anh.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://gbl.redwolf501.top

interface Shape { fun area(): Double }
来源：http://tgk.daxiang520.top

[T16] Swift：Hello World
来源：http://stj.chenlongwang.top

print("Hello")
来源：http://rzz.yangfankeji.com

[T17] Swift：变量与常量
来源：http://qel.pengpengdd.cyou

var a = 1;  let b = 2
来源：http://eux.yueranfly.top

[T18] Swift：字符串插值
来源：http://vhx.hywenlv.cn

"值: \(b)"
来源：http://rzz.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://qwv.316326.xyz

if let n = opt { print(n) }
来源：http://nhx.ppjwa.cn

[T20] Swift：数组操作
来源：http://ziz.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://hdz.nwbrower.top

[T21] Swift：遍历
来源：http://tkt.yuanzhike.top

for x in a { print(x) }
来源：http://kyf.316326.xyz

[T22] Swift：字典
来源：http://htw.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mya.bjfxy.top

[T23] Swift：函数
来源：http://yhx.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ctj.fzhhl.top

[T24] Swift：闭包
来源：http://ege.tianlin.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://jvt.hnxiangtu.top

[T25] Swift：结构体
来源：http://wwd.chenlongwang.top

struct P { var x: Int }
来源：http://vhz.nanxinkj.top

[T26] Swift：类与重写
来源：http://umm.wangdashe.top

class A: Base { override func f() {} }
来源：http://ocb.xinyue.icu

[T27] Swift：错误处理
来源：http://oll.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://lpc.shzxlz.cn

[T28] Swift：枚举
来源：http://vxf.xuanzx.com

enum Color { case red, green }
来源：http://ytn.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://yeh.guannengcc.top

guard let x = opt else { return }
来源：http://cip.hcnkem.com

[T30] Swift：协议
来源：http://ttg.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://ilt.ppjwa.cn

[T31] Lua：Hello World
来源：http://aky.9152youxi.cn

print("Hello")
来源：http://jds.sysykeji.top

[T32] Lua：局部变量
来源：http://anf.hfpthk.cn

local a = 1
来源：http://dup.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://nth.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ugm.yvedp.cn

[T34] Lua：遍历表
来源：http://dag.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rec.pycfn.com

[T35] Lua：字典表
来源：http://gxn.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://qkf.svipenyu.cn

[T36] Lua：函数
来源：http://eny.yangfankeji.com

function add(a, b) return a + b end
来源：http://dub.fzhhl.top

[T37] Lua：字符串拼接
来源：http://goy.hywenlv.cn

"a" .. "b"
来源：http://ayp.daxiang520.top

[T38] Lua：条件
来源：http://nsp.cqqwz.cn

if x > 0 then print("正") end
来源：http://xht.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://hsf.yj20258.top

string.find(s, "%d+")
来源：http://gqf.nanxinkj.top

[T40] Lua：元表
来源：http://txh.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://npj.haohaochexian.top

[T41] Perl：Hello World
来源：http://kbn.ydzc1.top

print "Hello\n";
来源：http://ofj.hysaishi.cn

[T42] Perl：变量类型
来源：http://xtt.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fba.snrcjt.cn

[T43] Perl：字符串插值
来源：http://kkx.shanyushiyangkeji.top

"值: $a"
来源：http://mzo.snrcjt.cn

[T44] Perl：条件
来源：http://ziw.tarul.cn

if ($a > 0) { print "正"; }
来源：http://rde.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://tnl.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://rde.ybcxt.top

[T46] Perl：哈希操作
来源：http://eps.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ysk.hysaishi.cn

[T47] Perl：正则捕获
来源：http://qgm.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rqi.gotoacloud.top

[T48] Perl：正则替换
来源：http://ujs.shzxlz.cn

$s =~ s/old/new/g;
来源：http://cir.yuxming.cn

[T49] Perl：函数
来源：http://alf.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nzi.guannengcc.top

[T50] Perl：逐行读文件
来源：http://agm.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://bfr.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://flw.fehbvm.com

[T51] Scala：Hello World
来源：http://lvj.bbcook.cn

println("Hello")
来源：http://pcn.aizwys.cn

[T52] Scala：变量
来源：http://tux.jinqigfzy.top

val a = 1;  var b = 2
来源：http://gwx.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://yhj.tanke756.top

s"值: $b"
来源：http://glg.gogol.net.cn

[T54] Scala：集合映射
来源：http://sce.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://dht.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://hgk.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://hzn.guannengcc.top

[T56] Scala：样例类
来源：http://qsd.aizwys.cn

case class User(name: String, age: Int)
来源：http://vfn.dianchejie.cn

[T57] Scala：模式匹配
来源：http://bsb.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xgt.gotoacloud.top

[T58] Scala：函数定义
来源：http://lrl.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://rgz.ivvv.top

[T59] Scala：循环
来源：http://mdq.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://bbk.chenzaomai.com

[T60] Scala：折叠
来源：http://pga.gzhubu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rpi.yuanzhike.top

================================================================================
来源：http://mps.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ztj.daria6918.cn

================================================================================
来源：http://oaw.yongpay.top

[U01] Py：创建虚拟环境
来源：http://hnp.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://aor.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://itw.shanyushiyangtech.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vxf.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://tvi.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cxv.xylfe.cn

[U04] Py：变量调试打印
来源：http://rgh.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xil.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://zex.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://yvt.hnqzz.top

[U06] Py：合并两个字典
来源：http://kul.tian-w.cn

{**a, **b}
来源：http://mpi.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://vay.andypj.xyz

{v: k for k, v in d.items()}
来源：http://rnp.tianlin.xyz

[U08] Py：展平二维列表
来源：http://mts.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://trx.vqdsnc.cn

[U09] Py：字典取最大值的键
来源：http://lab.jqgfzy.top

max(d, key=d.get)
来源：http://kxg.c1oappe.top

[U10] Py：按值排序字典
来源：http://aji.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nrh.gogol.net.cn

[U11] Py：生成器表达式
来源：http://gav.jqgfzy.top

(x * 2 for x in arr)
来源：http://xvt.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://gvt.zycfv.cn

Counter(arr).most_common(3)
来源：http://wvd.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://sza.sysykeji.top

deque(maxlen=10)
来源：http://odl.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://hql.xylfe.cn

defaultdict(list)
来源：http://glu.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://sga.aibaodan.cn

t = time.perf_counter()
来源：http://ilf.iojbl.cn

[U16] Py：命令行参数解析
来源：http://ban.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vtz.zhengqikj.top

[U17] Py：初始化日志
来源：http://qqb.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://daa.jqgufenzy.top

[U18] Py：预编译正则
来源：http://pjv.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://xjh.daria6918.cn


<!-- 参考信息 -->