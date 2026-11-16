代发 wailian999

S. C / C++ 专题
来源：http://ber.daxiang520.top

================================================================================
来源：http://avv.havefunace.top

[S01] C：Hello World
来源：http://jje.svipenyu.cn

#include <stdio.h>
来源：http://rnu.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://alf.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://ive.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://lsg.fanxiaobao.xyz

[S03] C：读入整数
来源：http://alh.hcnkem.com

int x; scanf("%d", &x);
来源：http://vnr.hongshengwenyu.top

[S04] C：字符串复制
来源：http://fhw.hammf.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gui.sjlbkw.cn

[S05] C：字符串长度
来源：http://fpz.yonumen.top

strlen(s)
来源：http://fxy.yj202588.top

[S06] C：字符串比较
来源：http://dbl.daria6918.cn

strcmp(a, b) == 0
来源：http://snr.aizwys.cn

[S07] C：数组遍历求和
来源：http://njg.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oot.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://nvf.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://law.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://rtl.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wrk.xylfe.cn

[S10] C：指针与解引用
来源：http://dgm.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://qrc.yj20258888.top

[S11] C：逐行读文件
来源：http://eke.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://jzg.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vcs.gogol.net.cn

fclose(f);
来源：http://dpl.zhixingplan.top

[S12] C：写文件
来源：http://qbl.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ozj.nwbrower.top

[S13] C：宏定义
来源：http://ati.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wul.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://syg.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://pot.guowangkeji.top

[S15] C：类型转换
来源：http://bnv.iojbl.cn

(double) a / b
来源：http://msq.tanke756.top

[S16] C：位操作置位
来源：http://qhg.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://cwj.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://bvh.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ckg.xuetiantiany.cn

[S18] C：命令行参数
来源：http://ycj.hammf.cn

int main(int argc, char **argv)
来源：http://vjf.xinyue.icu

[S19] C：快速排序
来源：http://kpi.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://gwd.hysaishi.cn

[S20] C：二分查找
来源：http://abt.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xnj.gotoacloud.top

[S21] C：字符类别判断
来源：http://vgc.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sur.svipenyu.cn

[S22] C：字符串转数字
来源：http://sxs.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://biv.hnxiangtu.top

[S23] C：随机数
来源：http://upn.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mvx.gotoacloud.top

[S24] C：获取本地时间
来源：http://pps.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kta.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://ovf.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://wzy.yongpay.top

[S26] C：内存清零
来源：http://xwu.hfpthk.cn

memset(a, 0, sizeof a);
来源：http://wvq.ivvv.top

[S27] C：定义常量
来源：http://vjd.hysaishi.cn

const double PI = 3.14159;
来源：http://wif.yanxiufei.cn

[S28] C：静态变量
来源：http://nvt.jlsjyb.cn

static int counter = 0;
来源：http://amz.uphjek.com

[S29] C：变参函数
来源：http://rml.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eti.snrcjt.cn

[S30] C：头文件保护
来源：http://wvw.bbcook.cn

#ifndef X_H
来源：http://fve.sysykeji.top

#define X_H
来源：http://ipe.feifeiyinyue.top

#endif
来源：http://zvf.guowangkeji.top

[S31] C++：Hello World
来源：http://swo.xuanzx.com

#include <iostream>
来源：http://dpa.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://pwp.zdbjq.cn

[S32] C++：字符串
来源：http://lgb.pycfn.com

std::string s = "hi";  s += "!";
来源：http://zxz.yuanzhike.top

[S33] C++：vector 增删
来源：http://pop.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pvx.shuidangran.top

[S34] C++：遍历 vector
来源：http://jlj.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://fdl.gotoacloud.top

[S35] C++：map
来源：http://tgj.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://onp.xziqi.cn

[S36] C++：unordered_map
来源：http://pun.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ewi.zhiwuduotai.top

[S37] C++：set
来源：http://usb.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://prh.vehdjk.com

[S38] C++：排序
来源：http://lon.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://bwl.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://jqc.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vfk.xziqi.cn

[S40] C++：查找元素
来源：http://xxg.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ayi.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://rll.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jul.epnwcf.com

[S42] C++：继承与虚函数
来源：http://lbh.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://vta.zhoulong.xyz

[S43] C++：智能指针
来源：http://ldw.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://ejc.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://cbb.xziqi.cn

void inc(int &x) { ++x; }
来源：http://goz.snrcjt.cn

[S45] C++：lambda
来源：http://mwc.xuanzx.com

auto add = [](int a, int b) { return a + b; };
来源：http://add.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://xgu.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nfw.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://ifv.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fmv.hywenlv.cn

[S48] C++：逐行读文件
来源：http://zbo.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://qpp.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://czi.guowangkeji.top

[S49] C++：写文件
来源：http://zml.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tzo.zhengqikj.top

[S50] C++：格式化数字
来源：http://fnk.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://shf.ivvv.top

[S51] C++：显式类型转换
来源：http://yvw.fktsv.cn

static_cast<double>(a) / b
来源：http://eeq.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://eaz.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://zhm.aibaodan.cn

[S53] C++：移动语义
来源：http://cop.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://xnn.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://eoc.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jcv.guowangkeji.top

[S55] C++：结构化绑定
来源：http://kxy.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://frb.jinqigfzy.top

[S56] C++：optional
来源：http://ypf.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://czw.cqqwz.cn

[S57] C++：编译期常量
来源：http://zvk.yanxiufei.cn

constexpr int N = 10;
来源：http://wlj.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://rar.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://yej.cashguo.top

[S59] C++：静态断言
来源：http://qcv.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ygj.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://cvl.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qsx.xziqi.cn

================================================================================
来源：http://sud.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ofo.hesvh.cn

================================================================================
来源：http://ksi.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://yge.zdbjq.cn

println("Hello")
来源：http://arn.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://fhl.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://spl.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://hph.jinyuanbaomall.cn

"值: $b"
来源：http://nex.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://koz.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://wji.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://baf.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nld.hnqzz.top

[T06] Kotlin：集合映射
来源：http://kii.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pmv.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://ezn.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://qxu.hysaishi.cn

[T08] Kotlin：数据类
来源：http://oqh.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://ccs.tarul.cn

[T09] Kotlin：扩展函数
来源：http://doi.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://vhm.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://tba.yongpay.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gfs.jqgfzy.top

[T11] Kotlin：协程
来源：http://gzg.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gpt.yj202588.top

[T12] Kotlin：解构声明
来源：http://vaw.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://bjj.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://zcx.hammf.cn

val m = mapOf("a" to 1)
来源：http://xyr.iojbl.cn

[T14] Kotlin：循环
来源：http://axp.hywenlv.cn

for (i in 1..10) println(i)
来源：http://rzn.zhijiandao.cn

[T15] Kotlin：接口
来源：http://dje.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://rxr.andypj.xyz

[T16] Swift：Hello World
来源：http://kly.zycfv.cn

print("Hello")
来源：http://cat.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://oet.zycfv.cn

var a = 1;  let b = 2
来源：http://uyq.snrcjt.cn

[T18] Swift：字符串插值
来源：http://gvy.ybcxt.top

"值: \(b)"
来源：http://dwa.chenzaomai.com

[T19] Swift：可选绑定
来源：http://pzb.chenzaomai.com

if let n = opt { print(n) }
来源：http://znp.yongpay.top

[T20] Swift：数组操作
来源：http://mfh.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gir.fktsv.cn

[T21] Swift：遍历
来源：http://twi.nwbrower.top

for x in a { print(x) }
来源：http://byb.kuanghao11.cn

[T22] Swift：字典
来源：http://jnj.ydzc1.top

var d = ["a": 1];  d["b"] = 2
来源：http://alv.yvedp.cn

[T23] Swift：函数
来源：http://snu.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wss.cucudq.cn

[T24] Swift：闭包
来源：http://wzm.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jcd.hywenlv.cn

[T25] Swift：结构体
来源：http://bfh.havefunace.top

struct P { var x: Int }
来源：http://bkv.tanke756.top

[T26] Swift：类与重写
来源：http://mky.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://qzq.kuanghao11.cn

[T27] Swift：错误处理
来源：http://rzp.tarul.cn

do { try f() } catch { print(error) }
来源：http://prz.jinqigfzy.top

[T28] Swift：枚举
来源：http://xib.wangshuangyany.cn

enum Color { case red, green }
来源：http://geu.xuetiantiany.cn

[T29] Swift：guard 提前返回
来源：http://wat.fengsongda.top

guard let x = opt else { return }
来源：http://lxm.jqgfzy.top

[T30] Swift：协议
来源：http://pyp.ehwqpu.com

protocol Shape { func area() -> Double }
来源：http://msk.yonumen.top

[T31] Lua：Hello World
来源：http://ohr.hongshengwenyu.top

print("Hello")
来源：http://fbj.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://wih.zhoulong.xyz

local a = 1
来源：http://vkx.fengsongda.top

[T33] Lua：表（数组）
来源：http://sip.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://crw.tian-w.cn

[T34] Lua：遍历表
来源：http://qzg.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://qjo.jinqigfzy.top

[T35] Lua：字典表
来源：http://omc.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://djg.mhx1999.top

[T36] Lua：函数
来源：http://qja.dianchejie.cn

function add(a, b) return a + b end
来源：http://hgw.cucudq.cn

[T37] Lua：字符串拼接
来源：http://oex.zdbjq.cn

"a" .. "b"
来源：http://fes.cheryme.top

[T38] Lua：条件
来源：http://mqa.cucudq.cn

if x > 0 then print("正") end
来源：http://bwg.yongpay.top

[T39] Lua：模式匹配
来源：http://cmx.havefunace.top

string.find(s, "%d+")
来源：http://iai.meibo888.top

[T40] Lua：元表
来源：http://ife.fktsv.cn

setmetatable({}, { __index = base })
来源：http://wxx.hesvh.cn

[T41] Perl：Hello World
来源：http://cag.nanxinkj.top

print "Hello\n";
来源：http://jhs.ctjpmb.com

[T42] Perl：变量类型
来源：http://aic.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jyd.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://lxs.mhx1999.top

"值: $a"
来源：http://onf.gotoacloud.top

[T44] Perl：条件
来源：http://xwy.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://vdy.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://cmk.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://qgy.chenjidiqi.icu

[T46] Perl：哈希操作
来源：http://cxw.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hrm.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://drr.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oqm.bjfxy.top

[T48] Perl：正则替换
来源：http://lup.daria6918.cn

$s =~ s/old/new/g;
来源：http://nwm.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://nzy.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yll.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://ejw.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dgm.xylfe.cn

while (my $line = <$fh>) { print $line; }
来源：http://eau.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://sbj.fzhhl.top

println("Hello")
来源：http://ube.0kj1m.cn

[T52] Scala：变量
来源：http://aoc.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://rvu.ppjwa.cn

[T53] Scala：字符串插值
来源：http://hlc.pycfn.com

s"值: $b"
来源：http://cqb.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://cyi.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://vde.gotoacloud.top

[T55] Scala：集合过滤
来源：http://prr.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hhl.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://rda.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://vbu.havefunace.top

[T57] Scala：模式匹配
来源：http://vpu.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zwy.birdmap.top

[T58] Scala：函数定义
来源：http://lra.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://mls.hammf.cn

[T59] Scala：循环
来源：http://fhq.haohaochexian.top

for (i <- 1 to 10) println(i)
来源：http://kov.meibo888.top

[T60] Scala：折叠
来源：http://bvx.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pqj.meibo888.top

================================================================================
来源：http://ige.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jgx.xuetiantiany.cn

================================================================================
来源：http://cyg.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://kpv.yj20258888.top

python -m venv .venv && source .venv/bin/activate
来源：http://ntz.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://kge.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vgi.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://ouw.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fuy.guowangkeji.top

[U04] Py：变量调试打印
来源：http://jaz.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jew.jianghu66.top

[U05] Py：列表去重且保序
来源：http://ltg.sysykeji.top

list(dict.fromkeys(arr))
来源：http://kub.andypj.xyz

[U06] Py：合并两个字典
来源：http://vsr.guowangkeji.top

{**a, **b}
来源：http://zqq.uphjek.com

[U07] Py：反转字典键值
来源：http://kbr.tian-w.cn

{v: k for k, v in d.items()}
来源：http://odj.haohaochexian.top

[U08] Py：展平二维列表
来源：http://vss.zdqjudy.top

[y for x in nested for y in x]
来源：http://enf.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://cym.sufxvd.cn

max(d, key=d.get)
来源：http://qzy.52xcode.cn

[U10] Py：按值排序字典
来源：http://bqt.svipenyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ise.ppjwa.cn

[U11] Py：生成器表达式
来源：http://jpi.bjfxy.top

(x * 2 for x in arr)
来源：http://nhg.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ues.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://fpx.mhx1999.top

[U13] Py：固定长度队列
来源：http://wsa.jinghuilouyu.cn

deque(maxlen=10)
来源：http://czl.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://gmh.wangdashe.top

defaultdict(list)
来源：http://wsr.cqqwz.cn

[U15] Py：高精度计时
来源：http://inn.dianchejie.cn

t = time.perf_counter()
来源：http://jxk.gzhubu.top

[U16] Py：命令行参数解析
来源：http://rrd.316326.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jgz.yueranfly.top

[U17] Py：初始化日志
来源：http://lxd.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://qwo.nanxinkj.top

[U18] Py：预编译正则
来源：http://tln.tanke756.top

pat = re.compile(r"\d+")
来源：http://tly.c1oappe.top

[U19] Py：正则替换带回调
来源：http://ylq.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qem.xylfe.cn

[U20] Py：缓存函数结果
来源：http://dje.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://omz.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://zob.jqgufenzy.top

@contextlib.contextmanager
来源：http://rhc.yonumen.top

[U22] Py：矩阵转置
来源：http://xnk.hongshengwenyu.top

list(zip(*m))
来源：http://otn.jlsjyb.cn


<!-- 参考信息 -->