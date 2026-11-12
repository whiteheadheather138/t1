代发 wailian999

int x; scanf("%d", &x);
来源：http://itp.hammf.cn

[S04] C：字符串复制
来源：http://jje.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ygz.zhoulong.xyz

[S05] C：字符串长度
来源：http://spr.xziqi.cn

strlen(s)
来源：http://ksu.daria6918.cn

[S06] C：字符串比较
来源：http://jfv.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://klo.ppjwa.cn

[S07] C：数组遍历求和
来源：http://xkt.pengpengdd.cyou

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lxj.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://yjx.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kaw.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://yof.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tag.jlsjyb.cn

[S10] C：指针与解引用
来源：http://seg.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://raa.yfazqb.com

[S11] C：逐行读文件
来源：http://opz.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://gst.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xej.birdmap.top

fclose(f);
来源：http://ick.nanxuanxn.top

[S12] C：写文件
来源：http://wlw.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eor.xuanzx.com

[S13] C：宏定义
来源：http://aif.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fvd.zhiwuduotai.top

[S14] C：枚举
来源：http://uoi.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://uqe.epnwcf.com

[S15] C：类型转换
来源：http://sdz.kuanghao11.cn

(double) a / b
来源：http://yax.xylfe.cn

[S16] C：位操作置位
来源：http://xza.vqdsnc.cn

x |= (1 << 3);
来源：http://sek.yj20258888.top

[S17] C：安全拼接字符串
来源：http://vci.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lqb.sweek.top

[S18] C：命令行参数
来源：http://ujt.cqqwz.cn

int main(int argc, char **argv)
来源：http://qqe.hesvh.cn

[S19] C：快速排序
来源：http://eov.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sip.ydzc1.top

[S20] C：二分查找
来源：http://yhj.hysaishi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fic.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://ryu.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ern.yvedp.cn

[S22] C：字符串转数字
来源：http://vjj.havefunace.top

atoi("42");  strtod("3.14", NULL);
来源：http://kra.smart0.xyz

[S23] C：随机数
来源：http://bpr.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://abt.yanxiufei.cn

[S24] C：获取本地时间
来源：http://eth.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ciy.hnxiangtu.top

[S25] C：内存拷贝
来源：http://snk.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://jpe.hysaishi.cn

[S26] C：内存清零
来源：http://jed.uphjek.com

memset(a, 0, sizeof a);
来源：http://ovz.tianlin.xyz

[S27] C：定义常量
来源：http://sby.iojbl.cn

const double PI = 3.14159;
来源：http://msj.wangshuangyany.cn

[S28] C：静态变量
来源：http://tpb.gzhubu.top

static int counter = 0;
来源：http://gvy.zdbjq.cn

[S29] C：变参函数
来源：http://vvn.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ytp.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://cud.yangfankeji.com

#ifndef X_H
来源：http://zsf.pycfn.com

#define X_H
来源：http://czd.zhongyouzk.top

#endif
来源：http://xgl.c1oappe.top

[S31] C++：Hello World
来源：http://vwl.gogol.net.cn

#include <iostream>
来源：http://wqu.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://esl.52xcode.cn

[S32] C++：字符串
来源：http://ilz.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://olt.zhongyouzk.top

[S33] C++：vector 增删
来源：http://xrv.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://anu.tanke756.top

[S34] C++：遍历 vector
来源：http://pwx.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://mez.fktsv.cn

[S35] C++：map
来源：http://qjy.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gul.smart0.xyz

[S36] C++：unordered_map
来源：http://hzm.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://loq.c1oappe.top

[S37] C++：set
来源：http://kvr.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rdb.aibaodan.cn

[S38] C++：排序
来源：http://zbg.cheryme.top

std::sort(v.begin(), v.end());
来源：http://nvz.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://aca.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fgs.yuxming.cn

[S40] C++：查找元素
来源：http://jzk.epnwcf.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://svz.yongpay.top

[S41] C++：类与构造函数
来源：http://mkd.shzxlz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lfa.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://dsx.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://gsm.yonumen.top

[S43] C++：智能指针
来源：http://evw.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://zak.jianghu66.top

[S44] C++：引用传参
来源：http://vir.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://lsp.bbcook.cn

[S45] C++：lambda
来源：http://qiv.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://ffu.zhengqikj.top

[S46] C++：函数模板
来源：http://zys.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tee.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://qwm.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ywh.redwolf501.top

[S48] C++：逐行读文件
来源：http://nqt.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jdu.fktsv.cn

while (std::getline(in, line)) { }
来源：http://lhc.cashguo.top

[S49] C++：写文件
来源：http://sln.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pzv.bbcook.cn

[S50] C++：格式化数字
来源：http://gcp.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aly.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://izj.ydzc1.top

static_cast<double>(a) / b
来源：http://wek.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://rts.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://uvb.shangyingyoupin.top

[S53] C++：移动语义
来源：http://zrb.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://muw.gaohongyu789.top

[S54] C++：异常处理
来源：http://zkh.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jvx.pycfn.com

[S55] C++：结构化绑定
来源：http://lcs.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://usd.cucudq.cn

[S56] C++：optional
来源：http://kpx.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ofj.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://mqs.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://zom.meibo888.top

[S58] C++：命名空间
来源：http://lmf.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://wui.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://wwr.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qgp.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://ihw.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fob.52xcode.cn

================================================================================
来源：http://dzm.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yxb.vqdsnc.cn

================================================================================
来源：http://fpp.daria6918.cn

[T01] Kotlin：Hello World
来源：http://xuj.jinqigufen.top

println("Hello")
来源：http://zsi.quarkkingdee.top

[T02] Kotlin：变量
来源：http://yuu.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hbk.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://qvr.ydzc1.top

"值: $b"
来源：http://sjo.svipenyu.cn

[T04] Kotlin：空安全
来源：http://lpd.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://iuc.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://vhv.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ikr.pycfn.com

[T06] Kotlin：集合映射
来源：http://fey.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mwx.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://lvc.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://txr.bbcook.cn

[T08] Kotlin：数据类
来源：http://pih.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://uqa.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://ile.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://xui.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://qik.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://ado.fehbvm.com

[T11] Kotlin：协程
来源：http://fzj.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lmj.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://rya.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://anx.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://uwp.yvedp.cn

val m = mapOf("a" to 1)
来源：http://uek.ydzc1.top

[T14] Kotlin：循环
来源：http://ghe.birdmap.top

for (i in 1..10) println(i)
来源：http://fvz.ydzc1.top

[T15] Kotlin：接口
来源：http://hcw.cheryme.top

interface Shape { fun area(): Double }
来源：http://siz.ehwqpu.com

[T16] Swift：Hello World
来源：http://gfw.c1oappe.top

print("Hello")
来源：http://bek.xziqi.cn

[T17] Swift：变量与常量
来源：http://ibr.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://ljb.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://ygd.shanyushiyangkeji.top

"值: \(b)"
来源：http://hki.ivvv.top

[T19] Swift：可选绑定
来源：http://uyj.guannengcc.top

if let n = opt { print(n) }
来源：http://rcw.svipenyu.cn

[T20] Swift：数组操作
来源：http://gou.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://gru.svipenyu.cn

[T21] Swift：遍历
来源：http://sll.sufxvd.cn

for x in a { print(x) }
来源：http://ddt.nanxuanxn.top

[T22] Swift：字典
来源：http://hve.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://cly.sweek.top

[T23] Swift：函数
来源：http://fwn.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://frb.9152youxi.cn

[T24] Swift：闭包
来源：http://ptd.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://bhl.jqgfzy.top

[T25] Swift：结构体
来源：http://fdv.cheryme.top

struct P { var x: Int }
来源：http://lci.hcnkem.com

[T26] Swift：类与重写
来源：http://hfm.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://leo.daria6918.cn

[T27] Swift：错误处理
来源：http://cwn.epnwcf.com

do { try f() } catch { print(error) }
来源：http://geu.vqdsnc.cn

[T28] Swift：枚举
来源：http://xxh.hfpthk.cn

enum Color { case red, green }
来源：http://ior.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://oce.guannengcc.top

guard let x = opt else { return }
来源：http://sgj.xuetiantiany.cn

[T30] Swift：协议
来源：http://kjz.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://htb.zhixingplan.top

[T31] Lua：Hello World
来源：http://wqh.yongpay.top

print("Hello")
来源：http://cte.yj202588.top

[T32] Lua：局部变量
来源：http://qsx.fktsv.cn

local a = 1
来源：http://cdw.zdqjudy.top

[T33] Lua：表（数组）
来源：http://fii.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://stl.aibaodan.cn

[T34] Lua：遍历表
来源：http://zbe.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://spn.zdqjudy.top

[T35] Lua：字典表
来源：http://hew.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://lqo.gotoacloud.top

[T36] Lua：函数
来源：http://ypc.ehwqpu.com

function add(a, b) return a + b end
来源：http://qel.tanke756.top

[T37] Lua：字符串拼接
来源：http://ari.nwbrower.top

"a" .. "b"
来源：http://psk.guannengcc.top

[T38] Lua：条件
来源：http://ntf.jinqigufen.top

if x > 0 then print("正") end
来源：http://eia.0kj1m.cn

[T39] Lua：模式匹配
来源：http://bvo.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://ewa.daria6918.cn

[T40] Lua：元表
来源：http://prc.316326.xyz

setmetatable({}, { __index = base })
来源：http://gtm.yj20258.top

[T41] Perl：Hello World
来源：http://urs.chenlongwang.top

print "Hello\n";
来源：http://xck.cqqwz.cn

[T42] Perl：变量类型
来源：http://njg.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ejq.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://mli.gogol.net.cn

"值: $a"
来源：http://eip.uphjek.com

[T44] Perl：条件
来源：http://djr.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://vus.xylfe.cn

[T45] Perl：数组遍历
来源：http://cyd.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://ema.guowangkeji.top

[T46] Perl：哈希操作
来源：http://mcu.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qpp.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://hkj.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hos.c1oappe.top

[T48] Perl：正则替换
来源：http://joh.ctjpmb.com

$s =~ s/old/new/g;
来源：http://ztp.smart0.xyz

[T49] Perl：函数
来源：http://zak.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xeu.fzhhl.top

[T50] Perl：逐行读文件
来源：http://qui.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uie.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://jip.hesvh.cn

[T51] Scala：Hello World
来源：http://vja.ydzc1.top

println("Hello")
来源：http://qoz.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://lpi.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://nph.daxiang520.top

[T53] Scala：字符串插值
来源：http://rmu.shuidangran.top

s"值: $b"
来源：http://mrs.xziqi.cn

[T54] Scala：集合映射
来源：http://pri.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://trw.hongshengwenyu.top

[T55] Scala：集合过滤
来源：http://lio.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oec.fzhhl.top

[T56] Scala：样例类
来源：http://wuc.xylfe.cn

case class User(name: String, age: Int)
来源：http://fmi.cashguo.top

[T57] Scala：模式匹配
来源：http://iij.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sfy.fehbvm.com

[T58] Scala：函数定义
来源：http://gjg.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://qgz.yanxiufei.cn

[T59] Scala：循环
来源：http://zcp.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://ghm.ivvv.top

[T60] Scala：折叠
来源：http://dbd.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dle.xingfuxueyuan.xyz

================================================================================
来源：http://okv.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ahl.daxiang520.top

================================================================================
来源：http://uhj.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://ynb.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://boh.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://kew.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bzj.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://gtc.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rrb.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://ggl.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ovk.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://krx.hesvh.cn

list(dict.fromkeys(arr))
来源：http://suj.guannengcc.top

[U06] Py：合并两个字典
来源：http://zkg.jinghuilouyu.cn

{**a, **b}
来源：http://mlc.xinyue.icu

[U07] Py：反转字典键值
来源：http://lht.hcnkem.com

{v: k for k, v in d.items()}
来源：http://vtx.xylfe.cn

[U08] Py：展平二维列表
来源：http://uxj.shangyingyoupin.top

[y for x in nested for y in x]
来源：http://brc.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://bhv.zhongyouzk.top

max(d, key=d.get)
来源：http://cir.hammf.cn

[U10] Py：按值排序字典
来源：http://sgn.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://odz.fzhhl.top

[U11] Py：生成器表达式
来源：http://pbk.52xcode.cn

(x * 2 for x in arr)
来源：http://sjg.guannengcc.top

[U12] Py：取出现最多的 3 个元素
来源：http://xnb.shuidangran.top

Counter(arr).most_common(3)
来源：http://flq.cqqwz.cn

[U13] Py：固定长度队列
来源：http://zqn.dashuyun.cn

deque(maxlen=10)
来源：http://dwy.uphjek.com

[U14] Py：分组收集到列表
来源：http://sda.jinghuilouyu.cn

defaultdict(list)
来源：http://wtx.svipenyu.cn

[U15] Py：高精度计时
来源：http://bsw.dashuyun.cn

t = time.perf_counter()
来源：http://jwt.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://xas.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kok.hnqzz.top

[U17] Py：初始化日志
来源：http://vrn.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://tjc.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://zqp.aizwys.cn

pat = re.compile(r"\d+")
来源：http://nle.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://pir.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qpj.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://zop.fengsongda.top

@functools.lru_cache(maxsize=None)
来源：http://zar.mhx1999.top

[U21] Py：自定义上下文管理器
来源：http://lem.chenlongwang.top

@contextlib.contextmanager
来源：http://jkf.gzhubu.top

[U22] Py：矩阵转置
来源：http://jas.aibaodan.cn

list(zip(*m))
来源：http://eww.yuxming.cn

[U23] Py：分块读取大文件
来源：http://tdr.sufxvd.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jvp.xziqi.cn

[U24] Py：路径操作
来源：http://jsn.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qya.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://cgr.havefunace.top

csv.DictReader(f)
来源：http://qvs.feifeiyinyue.top

[U26] Py：并发下载
来源：http://fub.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://elp.ivvv.top


<!-- 参考信息 -->