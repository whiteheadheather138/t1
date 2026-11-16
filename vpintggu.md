代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tpk.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://ska.c1oappe.top

time ./run.sh
来源：http://daw.c1oappe.top

================================================================================
来源：http://xsh.c1oappe.top

S. C / C++ 专题
来源：http://zkz.yj20258.top

================================================================================
来源：http://idd.cdnleiting.top

[S01] C：Hello World
来源：http://dqk.bjfxy.top

#include <stdio.h>
来源：http://gms.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gpg.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://ymx.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://wst.nanxinkj.top

[S03] C：读入整数
来源：http://rwy.tarul.cn

int x; scanf("%d", &x);
来源：http://nvt.wangdashe.top

[S04] C：字符串复制
来源：http://sgp.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://jun.tanke756.top

[S05] C：字符串长度
来源：http://dus.aibaodan.cn

strlen(s)
来源：http://ahg.xylfe.cn

[S06] C：字符串比较
来源：http://uwj.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://vmn.haohaochexian.top

[S07] C：数组遍历求和
来源：http://hdk.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zgj.havefunace.top

[S08] C：动态内存分配与释放
来源：http://jbc.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jsh.zdqjudy.top

[S09] C：结构体定义与初始化
来源：http://nvs.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kie.c1oappe.top

[S10] C：指针与解引用
来源：http://bhh.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://nrl.c1oappe.top

[S11] C：逐行读文件
来源：http://jao.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://pgy.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://lcl.sysykeji.top

fclose(f);
来源：http://mrc.quarkkingdee.top

[S12] C：写文件
来源：http://xqr.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ivo.zycfv.cn

[S13] C：宏定义
来源：http://gts.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iak.tianlin.xyz

[S14] C：枚举
来源：http://gmq.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://xph.fktsv.cn

[S15] C：类型转换
来源：http://xyh.chenlongwang.top

(double) a / b
来源：http://piv.316326.xyz

[S16] C：位操作置位
来源：http://mrs.gzhubu.top

x |= (1 << 3);
来源：http://tka.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://jlh.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jva.c1oappe.top

[S18] C：命令行参数
来源：http://yqv.shuidangran.top

int main(int argc, char **argv)
来源：http://gza.shangyingyoupin.top

[S19] C：快速排序
来源：http://far.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xdt.jqgfzy.top

[S20] C：二分查找
来源：http://ulf.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uur.sufxvd.cn

[S21] C：字符类别判断
来源：http://qmn.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bzu.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://bqk.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://ndc.zhongyouzk.top

[S23] C：随机数
来源：http://npe.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cul.yueranfly.top

[S24] C：获取本地时间
来源：http://ccg.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gyb.nanxinkj.top

[S25] C：内存拷贝
来源：http://yxr.ivvv.top

memcpy(dst, src, n);
来源：http://ddo.cdnleiting.top

[S26] C：内存清零
来源：http://ikw.yuxming.cn

memset(a, 0, sizeof a);
来源：http://qax.vqdsnc.cn

[S27] C：定义常量
来源：http://jxp.yj20258.top

const double PI = 3.14159;
来源：http://jpr.jinqigufen.top

[S28] C：静态变量
来源：http://ftf.xylfe.cn

static int counter = 0;
来源：http://ciy.yuxming.cn

[S29] C：变参函数
来源：http://kiu.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rdt.dianchejie.cn

[S30] C：头文件保护
来源：http://pki.zycfv.cn

#ifndef X_H
来源：http://mjq.ctjpmb.com

#define X_H
来源：http://slh.redwolf501.top

#endif
来源：http://wyh.gaohongyu789.top

[S31] C++：Hello World
来源：http://jok.nwbrower.top

#include <iostream>
来源：http://txb.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://hrq.9152youxi.cn

[S32] C++：字符串
来源：http://lyd.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://iks.hesvh.cn

[S33] C++：vector 增删
来源：http://dls.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wgm.hnqzz.top

[S34] C++：遍历 vector
来源：http://wzb.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://xyp.guowangkeji.top

[S35] C++：map
来源：http://beu.sweek.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vxm.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://kft.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ags.hammf.cn

[S37] C++：set
来源：http://qpx.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lsh.guannengcc.top

[S38] C++：排序
来源：http://dmx.zdbjq.cn

std::sort(v.begin(), v.end());
来源：http://ayb.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://zjr.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://szk.chenzaomai.com

[S40] C++：查找元素
来源：http://rnq.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pib.hysaishi.cn

[S41] C++：类与构造函数
来源：http://onn.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oaa.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://zgi.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://acb.pengpengdd.cyou

[S43] C++：智能指针
来源：http://dty.yueranfly.top

auto p = std::make_unique<int>(5);
来源：http://aod.sweek.top

[S44] C++：引用传参
来源：http://xid.gzhubu.top

void inc(int &x) { ++x; }
来源：http://qre.ywan-chungtsiang.top

[S45] C++：lambda
来源：http://dil.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ryk.gogol.net.cn

[S46] C++：函数模板
来源：http://xal.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zue.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://avf.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ypu.yuanzhike.top

[S48] C++：逐行读文件
来源：http://fgs.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://fpd.tanke756.top

while (std::getline(in, line)) { }
来源：http://jai.xuetiantiany.cn

[S49] C++：写文件
来源：http://lvm.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xqm.ybcxt.top

[S50] C++：格式化数字
来源：http://zud.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://epw.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://gos.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://tqp.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://jhp.fzhhl.top

int size() const noexcept { return n_; }
来源：http://iom.nwbrower.top

[S53] C++：移动语义
来源：http://tjv.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://xhi.bjfxy.top

[S54] C++：异常处理
来源：http://vua.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kun.daxiang520.top

[S55] C++：结构化绑定
来源：http://rad.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gxg.gzhubu.top

[S56] C++：optional
来源：http://kgl.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ldy.fehbvm.com

[S57] C++：编译期常量
来源：http://ddv.guowangkeji.top

constexpr int N = 10;
来源：http://axd.shuidangran.top

[S58] C++：命名空间
来源：http://dor.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://lii.dianchejie.cn

[S59] C++：静态断言
来源：http://wou.sxryk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hlf.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://cdp.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ruw.yuanzhike.top

================================================================================
来源：http://rck.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jby.svipenyu.cn

================================================================================
来源：http://gtk.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://ets.smart0.xyz

println("Hello")
来源：http://ieb.iojbl.cn

[T02] Kotlin：变量
来源：http://vcd.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ktj.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://svf.sysykeji.top

"值: $b"
来源：http://qhg.meibo888.top

[T04] Kotlin：空安全
来源：http://yvc.meibo888.top

val n: String? = null;  n?.length
来源：http://akb.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://mwg.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nov.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://rfe.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eva.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://ouz.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vqg.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://kyl.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://hds.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://ccr.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://bso.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://jre.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hok.aizwys.cn

[T11] Kotlin：协程
来源：http://klv.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jjq.yongpay.top

[T12] Kotlin：解构声明
来源：http://ano.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://zra.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://zhx.sxryk.cn

val m = mapOf("a" to 1)
来源：http://adp.fengsongda.top

[T14] Kotlin：循环
来源：http://zrm.sjlbkw.cn

for (i in 1..10) println(i)
来源：http://quk.cheryme.top

[T15] Kotlin：接口
来源：http://ibr.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://qsy.gaohongyu789.top

[T16] Swift：Hello World
来源：http://ogw.yuanzhike.top

print("Hello")
来源：http://srw.chenlongwang.top

[T17] Swift：变量与常量
来源：http://wgj.jinqigfzy.top

var a = 1;  let b = 2
来源：http://kev.shzxlz.cn

[T18] Swift：字符串插值
来源：http://zqc.tian-w.cn

"值: \(b)"
来源：http://upm.uphjek.com

[T19] Swift：可选绑定
来源：http://bpn.yonumen.top

if let n = opt { print(n) }
来源：http://dof.c1oappe.top

[T20] Swift：数组操作
来源：http://itv.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://ydw.redwolf501.top

[T21] Swift：遍历
来源：http://wrk.hongshengwenyu.top

for x in a { print(x) }
来源：http://dcr.hnxiangtu.top

[T22] Swift：字典
来源：http://wln.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://src.zdqjudy.top

[T23] Swift：函数
来源：http://tca.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ckt.yangfankeji.com

[T24] Swift：闭包
来源：http://dqv.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://noc.vehdjk.com

[T25] Swift：结构体
来源：http://vut.bjfxy.top

struct P { var x: Int }
来源：http://xot.nanxinkj.top

[T26] Swift：类与重写
来源：http://bax.haohaochexian.top

class A: Base { override func f() {} }
来源：http://mkw.fengsongda.top

[T27] Swift：错误处理
来源：http://jzn.ybcxt.top

do { try f() } catch { print(error) }
来源：http://usy.gzhubu.top

[T28] Swift：枚举
来源：http://kff.bjfxy.top

enum Color { case red, green }
来源：http://bnq.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://azj.cashguo.top

guard let x = opt else { return }
来源：http://xew.epnwcf.com

[T30] Swift：协议
来源：http://xsn.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://bpq.uphjek.com

[T31] Lua：Hello World
来源：http://akb.bjfxy.top

print("Hello")
来源：http://fye.mhx1999.top

[T32] Lua：局部变量
来源：http://xtj.aizwys.cn

local a = 1
来源：http://xrw.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://pit.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://trw.epnwcf.com

[T34] Lua：遍历表
来源：http://eke.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qlk.316326.xyz

[T35] Lua：字典表
来源：http://ome.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://ffw.hesvh.cn

[T36] Lua：函数
来源：http://fwc.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://mfe.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://nir.cqqwz.cn

"a" .. "b"
来源：http://kss.xylfe.cn

[T38] Lua：条件
来源：http://hhq.zhijiandao.cn

if x > 0 then print("正") end
来源：http://abe.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://axu.daria6918.cn

string.find(s, "%d+")
来源：http://djq.cheryme.top

[T40] Lua：元表
来源：http://bwl.ydjk.org.cn

setmetatable({}, { __index = base })
来源：http://vqu.yj202588.top

[T41] Perl：Hello World
来源：http://eas.chenzaomai.com

print "Hello\n";
来源：http://mni.quarkkingdee.top

[T42] Perl：变量类型
来源：http://wln.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nvw.zdqjudy.top

[T43] Perl：字符串插值
来源：http://odv.hfpthk.cn

"值: $a"
来源：http://qee.wangdashe.top

[T44] Perl：条件
来源：http://soi.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://oxt.fzhhl.top

[T45] Perl：数组遍历
来源：http://qjm.uphjek.com

for my $x (@arr) { print $x; }
来源：http://uds.9152youxi.cn

[T46] Perl：哈希操作
来源：http://hin.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wwp.sweek.top

[T47] Perl：正则捕获
来源：http://yzf.0kj1m.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ilu.nanxuanxn.top

[T48] Perl：正则替换
来源：http://cvw.tianlin.xyz

$s =~ s/old/new/g;
来源：http://mng.shanyushiyangtech.top

[T49] Perl：函数
来源：http://sob.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tso.hcnkem.com

[T50] Perl：逐行读文件
来源：http://rjl.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bkd.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://uoy.vqdsnc.cn

[T51] Scala：Hello World
来源：http://whd.hcnkem.com

println("Hello")
来源：http://rck.cucudq.cn

[T52] Scala：变量
来源：http://cnx.ctjpmb.com

val a = 1;  var b = 2
来源：http://thc.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://nos.ydjk.org.cn

s"值: $b"
来源：http://vwr.quarkkingdee.top

[T54] Scala：集合映射
来源：http://aju.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://sqp.yuxming.cn

[T55] Scala：集合过滤
来源：http://ihv.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://gpc.snrcjt.cn

[T56] Scala：样例类
来源：http://bzj.yvedp.cn

case class User(name: String, age: Int)
来源：http://ios.pycfn.com

[T57] Scala：模式匹配
来源：http://zxl.dashuyun.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bjz.zhengqikj.top

[T58] Scala：函数定义
来源：http://etk.sweek.top

def add(a: Int, b: Int): Int = a + b
来源：http://ali.sufxvd.cn

[T59] Scala：循环
来源：http://rpv.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://pdd.cqqwz.cn

[T60] Scala：折叠
来源：http://tqi.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://unk.jlsjyb.cn

================================================================================
来源：http://vzo.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pid.chenjidiqi.icu

================================================================================
来源：http://zjp.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://ycc.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dvk.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://gvk.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zmp.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://loc.gzhubu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hdy.hesvh.cn

[U04] Py：变量调试打印
来源：http://vzx.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jbx.sxryk.cn

[U05] Py：列表去重且保序
来源：http://mke.mhx1999.top

list(dict.fromkeys(arr))
来源：http://qbc.yj20258.top

[U06] Py：合并两个字典
来源：http://hqf.ywan-chungtsiang.top

{**a, **b}
来源：http://eop.cdnleiting.top

[U07] Py：反转字典键值
来源：http://jwk.daxiang520.top

{v: k for k, v in d.items()}
来源：http://wvy.wangdashe.top

[U08] Py：展平二维列表
来源：http://ktq.mhx1999.top

[y for x in nested for y in x]
来源：http://vfx.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://znc.tian-w.cn

max(d, key=d.get)
来源：http://uid.daxiang520.top

[U10] Py：按值排序字典
来源：http://xgw.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xcw.daria6918.cn

[U11] Py：生成器表达式
来源：http://zud.52xcode.cn

(x * 2 for x in arr)
来源：http://jkx.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rei.ppjwa.cn

Counter(arr).most_common(3)
来源：http://tfw.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://nfg.zhongyouzk.top

deque(maxlen=10)
来源：http://ywl.xinyue.icu

[U14] Py：分组收集到列表
来源：http://add.fengsongda.top

defaultdict(list)
来源：http://odf.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://ots.0kj1m.cn

t = time.perf_counter()
来源：http://vas.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://qxn.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wvj.shanyushiyangtech.top

[U17] Py：初始化日志
来源：http://uhy.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://vgm.daria6918.cn

[U18] Py：预编译正则
来源：http://mmq.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://myn.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://auo.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fnj.ehwqpu.com

[U20] Py：缓存函数结果
来源：http://azf.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://xzw.daria6918.cn


<!-- 参考信息 -->