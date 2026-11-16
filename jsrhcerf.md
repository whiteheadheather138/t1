代发 wailian999

S. C / C++ 专题
来源：http://mjk.52xcode.cn

================================================================================
来源：http://fky.jqgfzy.top

[S01] C：Hello World
来源：http://lno.ivvv.top

#include <stdio.h>
来源：http://nia.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://csy.nwbrower.top

[S02] C：变量与格式化输出
来源：http://fvc.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://tvv.ctjpmb.com

[S03] C：读入整数
来源：http://ofl.c1oappe.top

int x; scanf("%d", &x);
来源：http://eor.gzhubu.top

[S04] C：字符串复制
来源：http://hkf.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pyy.zhixingplan.top

[S05] C：字符串长度
来源：http://bco.jqgfzy.top

strlen(s)
来源：http://fgv.xylfe.cn

[S06] C：字符串比较
来源：http://ehb.iojbl.cn

strcmp(a, b) == 0
来源：http://nqf.gotoacloud.top

[S07] C：数组遍历求和
来源：http://sqi.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rqa.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://zyd.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ocu.cashguo.top

[S09] C：结构体定义与初始化
来源：http://xaf.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rcz.gogol.net.cn

[S10] C：指针与解引用
来源：http://dth.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://erg.316326.xyz

[S11] C：逐行读文件
来源：http://fpy.yanxiufei.cn

FILE *f = fopen("a.txt", "r");
来源：http://aud.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dbl.hywenlv.cn

fclose(f);
来源：http://ssr.guannengcc.top

[S12] C：写文件
来源：http://wbz.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qnl.hnqzz.top

[S13] C：宏定义
来源：http://geg.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yis.xziqi.cn

[S14] C：枚举
来源：http://mxv.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://aea.gotoacloud.top

[S15] C：类型转换
来源：http://qwm.wangdashe.top

(double) a / b
来源：http://ntc.0kj1m.cn

[S16] C：位操作置位
来源：http://ena.nanxinkj.top

x |= (1 << 3);
来源：http://hkr.cucudq.cn

[S17] C：安全拼接字符串
来源：http://fvi.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ryc.ydjk.org.cn

[S18] C：命令行参数
来源：http://ohn.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://luh.xuetiantiany.cn

[S19] C：快速排序
来源：http://hsm.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rvl.jyoumei.cn

[S20] C：二分查找
来源：http://eoq.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zef.pycfn.com

[S21] C：字符类别判断
来源：http://mkk.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gbn.yonumen.top

[S22] C：字符串转数字
来源：http://ygy.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://edd.tian-w.cn

[S23] C：随机数
来源：http://zvb.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://kjz.cashguo.top

[S24] C：获取本地时间
来源：http://qly.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://edg.9152youxi.cn

[S25] C：内存拷贝
来源：http://sjl.c1oappe.top

memcpy(dst, src, n);
来源：http://xqj.hfpthk.cn

[S26] C：内存清零
来源：http://xbd.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://oqp.feifeiyinyue.top

[S27] C：定义常量
来源：http://pos.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://okt.redwolf501.top

[S28] C：静态变量
来源：http://giu.52xcode.cn

static int counter = 0;
来源：http://hfu.redwolf501.top

[S29] C：变参函数
来源：http://qao.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ehn.sxryk.cn

[S30] C：头文件保护
来源：http://qao.cdnleiting.top

#ifndef X_H
来源：http://rmx.jlsjyb.cn

#define X_H
来源：http://olk.zhaomingkeji.xyz

#endif
来源：http://idv.aibaodan.cn

[S31] C++：Hello World
来源：http://eei.zhongyouzk.top

#include <iostream>
来源：http://vpd.shuidangran.top

int main() { std::cout << "Hello\n"; }
来源：http://sxp.jiagoushi.top

[S32] C++：字符串
来源：http://tzy.316326.xyz

std::string s = "hi";  s += "!";
来源：http://ibs.sjlbkw.cn

[S33] C++：vector 增删
来源：http://ffo.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ozo.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://mty.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://hyo.ywan-chungtsiang.top

[S35] C++：map
来源：http://vnh.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mio.jinqigfzy.top

[S36] C++：unordered_map
来源：http://mrl.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://phw.cashguo.top

[S37] C++：set
来源：http://ego.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hrf.yfazqb.com

[S38] C++：排序
来源：http://glf.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://lnd.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://hlw.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cbs.zhiwuduotai.top

[S40] C++：查找元素
来源：http://nid.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zhv.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://woa.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sjx.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://zwa.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://onm.yuxming.cn

[S43] C++：智能指针
来源：http://qnc.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://rsh.xinyue.icu

[S44] C++：引用传参
来源：http://iow.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://wvd.guannengcc.top

[S45] C++：lambda
来源：http://nnq.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://ypq.cheryme.top

[S46] C++：函数模板
来源：http://raj.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://brx.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://mxl.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ehn.epnwcf.com

[S48] C++：逐行读文件
来源：http://eun.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://omf.havefunace.top

while (std::getline(in, line)) { }
来源：http://rol.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://nrh.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ljv.yangfankeji.com

[S50] C++：格式化数字
来源：http://nte.svipenyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rcu.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://rqe.yongpay.top

static_cast<double>(a) / b
来源：http://qhm.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://sfw.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://eih.yanxiufei.cn

[S53] C++：移动语义
来源：http://psp.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://dth.iojbl.cn

[S54] C++：异常处理
来源：http://kvp.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://maw.sufxvd.cn

[S55] C++：结构化绑定
来源：http://vzc.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://haj.yvedp.cn

[S56] C++：optional
来源：http://lxp.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sck.yj20258888.top

[S57] C++：编译期常量
来源：http://czz.guowangkeji.top

constexpr int N = 10;
来源：http://bgq.fehbvm.com

[S58] C++：命名空间
来源：http://mlm.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://tpw.jlsjyb.cn

[S59] C++：静态断言
来源：http://buc.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bgh.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://jnh.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vif.chenlongwang.top

================================================================================
来源：http://zaw.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sid.tanke756.top

================================================================================
来源：http://dzr.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://otg.gzhubu.top

println("Hello")
来源：http://lmu.chenlongwang.top

[T02] Kotlin：变量
来源：http://ojq.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://urp.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://lyc.guowangkeji.top

"值: $b"
来源：http://xxe.guowangkeji.top

[T04] Kotlin：空安全
来源：http://bul.c1oappe.top

val n: String? = null;  n?.length
来源：http://rut.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://xtl.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://phy.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://fpy.sxryk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rid.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://zbn.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vnk.tanke756.top

[T08] Kotlin：数据类
来源：http://vab.gotoacloud.top

data class User(val name: String, val age: Int)
来源：http://htg.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://mze.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://zyu.ydjk.org.cn

[T10] Kotlin：默认参数
来源：http://vvx.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://isj.52xcode.cn

[T11] Kotlin：协程
来源：http://atv.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bqh.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://jvp.aizwys.cn

val (a, b) = Pair(1, 2)
来源：http://wum.guowangkeji.top

[T13] Kotlin：只读 Map
来源：http://uxa.yuxming.cn

val m = mapOf("a" to 1)
来源：http://pnt.ehwqpu.com

[T14] Kotlin：循环
来源：http://uli.gotoacloud.top

for (i in 1..10) println(i)
来源：http://emk.aibaodan.cn

[T15] Kotlin：接口
来源：http://ohf.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://xdm.jinqigufen.top

[T16] Swift：Hello World
来源：http://jkv.mhx1999.top

print("Hello")
来源：http://qlk.gotoacloud.top

[T17] Swift：变量与常量
来源：http://uhf.52xcode.cn

var a = 1;  let b = 2
来源：http://shq.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://nfm.sxryk.cn

"值: \(b)"
来源：http://dha.uphjek.com

[T19] Swift：可选绑定
来源：http://xeb.redwolf501.top

if let n = opt { print(n) }
来源：http://vkf.chenlongwang.top

[T20] Swift：数组操作
来源：http://ewl.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dte.hesvh.cn

[T21] Swift：遍历
来源：http://dgx.guowangkeji.top

for x in a { print(x) }
来源：http://wda.bjfxy.top

[T22] Swift：字典
来源：http://vwu.vqdsnc.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mgn.hesvh.cn

[T23] Swift：函数
来源：http://cfz.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kgu.snrcjt.cn

[T24] Swift：闭包
来源：http://jqw.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iow.xylfe.cn

[T25] Swift：结构体
来源：http://lys.vehdjk.com

struct P { var x: Int }
来源：http://chn.aizwys.cn

[T26] Swift：类与重写
来源：http://ioh.0kj1m.cn

class A: Base { override func f() {} }
来源：http://coe.sufxvd.cn

[T27] Swift：错误处理
来源：http://kpr.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://kmx.jqgfzy.top

[T28] Swift：枚举
来源：http://rtz.daxiang520.top

enum Color { case red, green }
来源：http://keo.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://wzo.52xcode.cn

guard let x = opt else { return }
来源：http://cgv.uphjek.com

[T30] Swift：协议
来源：http://ggq.xylfe.cn

protocol Shape { func area() -> Double }
来源：http://uud.nanxinkj.top

[T31] Lua：Hello World
来源：http://nhc.zhengqikj.top

print("Hello")
来源：http://soz.xziqi.cn

[T32] Lua：局部变量
来源：http://weh.ywan-chungtsiang.top

local a = 1
来源：http://jom.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://mva.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://laz.aibaodan.cn

[T34] Lua：遍历表
来源：http://ych.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bxo.cashguo.top

[T35] Lua：字典表
来源：http://fbk.ydjk.org.cn

local d = { a = 1 };  d.b = 2
来源：http://fos.chenzaomai.com

[T36] Lua：函数
来源：http://sel.shuidangran.top

function add(a, b) return a + b end
来源：http://pij.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://kdq.aizwys.cn

"a" .. "b"
来源：http://ags.shanyushiyangtech.top

[T38] Lua：条件
来源：http://apf.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://mdb.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://hrb.aibaodan.cn

string.find(s, "%d+")
来源：http://awe.iojbl.cn

[T40] Lua：元表
来源：http://afc.bjfxy.top

setmetatable({}, { __index = base })
来源：http://gxt.gogol.net.cn

[T41] Perl：Hello World
来源：http://pna.ctjpmb.com

print "Hello\n";
来源：http://aqv.hysaishi.cn

[T42] Perl：变量类型
来源：http://dci.shuidangran.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kjo.ivvv.top

[T43] Perl：字符串插值
来源：http://kvs.hnqzz.top

"值: $a"
来源：http://vfi.tianlin.xyz

[T44] Perl：条件
来源：http://amu.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://usj.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://hln.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://wdg.zhoulong.xyz

[T46] Perl：哈希操作
来源：http://rlu.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jne.guowangkeji.top

[T47] Perl：正则捕获
来源：http://boh.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qbh.ivvv.top

[T48] Perl：正则替换
来源：http://wkf.yj20258888.top

$s =~ s/old/new/g;
来源：http://gpp.zhengqikj.top

[T49] Perl：函数
来源：http://css.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rnt.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://ixx.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://agr.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://czb.jinqigfzy.top

[T51] Scala：Hello World
来源：http://vug.quarkkingdee.top

println("Hello")
来源：http://mfi.zhengqikj.top

[T52] Scala：变量
来源：http://zrw.c1oappe.top

val a = 1;  var b = 2
来源：http://tnl.ybcxt.top

[T53] Scala：字符串插值
来源：http://eol.xinyue.icu

s"值: $b"
来源：http://zud.fzhhl.top

[T54] Scala：集合映射
来源：http://soj.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://xhz.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://qqd.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lgl.hammf.cn

[T56] Scala：样例类
来源：http://jme.hywenlv.cn

case class User(name: String, age: Int)
来源：http://dqy.dianchejie.cn

[T57] Scala：模式匹配
来源：http://chj.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://dcb.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://zml.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wux.yonumen.top

[T59] Scala：循环
来源：http://clb.daria6918.cn

for (i <- 1 to 10) println(i)
来源：http://qhl.sxryk.cn

[T60] Scala：折叠
来源：http://lvo.tarul.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://luw.hfpthk.cn

================================================================================
来源：http://xjt.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hdl.cheryme.top

================================================================================
来源：http://ceg.zhengqikj.top

[U01] Py：创建虚拟环境
来源：http://msp.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://exc.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://pwq.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://brd.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://cug.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yrf.meibo888.top

[U04] Py：变量调试打印
来源：http://ood.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nqa.shanyushiyangtech.top

[U05] Py：列表去重且保序
来源：http://hob.yj202588.top

list(dict.fromkeys(arr))
来源：http://otn.yj20258888.top

[U06] Py：合并两个字典
来源：http://gmp.gaohongyu789.top

{**a, **b}
来源：http://ciq.yangfankeji.com

[U07] Py：反转字典键值
来源：http://egj.yueranfly.top

{v: k for k, v in d.items()}
来源：http://omo.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://aep.zhiwuduotai.top

[y for x in nested for y in x]
来源：http://ajn.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://ynr.shuidangran.top

max(d, key=d.get)
来源：http://lic.hfpthk.cn

[U10] Py：按值排序字典
来源：http://dkg.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lft.yvedp.cn

[U11] Py：生成器表达式
来源：http://cgu.yj202588.top

(x * 2 for x in arr)
来源：http://kjl.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://wdy.bjfxy.top

Counter(arr).most_common(3)
来源：http://hbr.svipenyu.cn

[U13] Py：固定长度队列
来源：http://pvo.jinqigufen.top

deque(maxlen=10)
来源：http://ony.fehbvm.com

[U14] Py：分组收集到列表
来源：http://lfq.shanyushiyangkeji.top

defaultdict(list)
来源：http://wxg.yueranfly.top

[U15] Py：高精度计时
来源：http://nsv.fzhhl.top

t = time.perf_counter()
来源：http://jsp.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://cib.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gfc.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://ygv.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://rfn.xuanzx.com

[U18] Py：预编译正则
来源：http://kfk.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://inp.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://rxi.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hmv.daria6918.cn

[U20] Py：缓存函数结果
来源：http://hlp.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://shz.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://hvc.ydzc1.top

@contextlib.contextmanager
来源：http://hwj.wangdashe.top

[U22] Py：矩阵转置
来源：http://vyx.jqgfzy.top

list(zip(*m))
来源：http://drc.jyoumei.cn


<!-- 参考信息 -->