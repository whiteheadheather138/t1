代发 wailian999

int x; scanf("%d", &x);
来源：http://slf.zhoulong.xyz

[S04] C：字符串复制
来源：http://qhq.feifeiyinyue.top

char dst[32]; strcpy(dst, "hi");
来源：http://yvp.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://ghp.ybcxt.top

strlen(s)
来源：http://der.pengpengdd.cyou

[S06] C：字符串比较
来源：http://rcu.tianlin.xyz

strcmp(a, b) == 0
来源：http://acc.wangdashe.top

[S07] C：数组遍历求和
来源：http://oby.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tvu.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://leq.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uda.gzhubu.top

[S09] C：结构体定义与初始化
来源：http://lrv.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://exm.guannengcc.top

[S10] C：指针与解引用
来源：http://edf.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://bxp.aizwys.cn

[S11] C：逐行读文件
来源：http://ovo.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://obb.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://trg.hcnkem.com

fclose(f);
来源：http://cuk.guowangkeji.top

[S12] C：写文件
来源：http://wsq.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qlf.ivvv.top

[S13] C：宏定义
来源：http://wzo.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qgi.feifeiyinyue.top

[S14] C：枚举
来源：http://tiv.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://hkq.aizwys.cn

[S15] C：类型转换
来源：http://tue.yvedp.cn

(double) a / b
来源：http://xhk.hesvh.cn

[S16] C：位操作置位
来源：http://rzs.fktsv.cn

x |= (1 << 3);
来源：http://grb.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://prw.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://elk.cheryme.top

[S18] C：命令行参数
来源：http://gpi.ydzc1.top

int main(int argc, char **argv)
来源：http://ygh.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://qdp.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rvh.zdqjudy.top

[S20] C：二分查找
来源：http://wxo.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mhq.yongpay.top

[S21] C：字符类别判断
来源：http://pud.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ksf.sxryk.cn

[S22] C：字符串转数字
来源：http://fld.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://stu.jiagoushi.top

[S23] C：随机数
来源：http://nza.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qfb.ctjpmb.com

[S24] C：获取本地时间
来源：http://ggy.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fia.iojbl.cn

[S25] C：内存拷贝
来源：http://vpa.hcnkem.com

memcpy(dst, src, n);
来源：http://nax.tian-w.cn

[S26] C：内存清零
来源：http://lih.cheryme.top

memset(a, 0, sizeof a);
来源：http://sem.redwolf501.top

[S27] C：定义常量
来源：http://fkk.meibo888.top

const double PI = 3.14159;
来源：http://irf.tian-w.cn

[S28] C：静态变量
来源：http://kif.ywan-chungtsiang.top

static int counter = 0;
来源：http://xzo.hnqzz.top

[S29] C：变参函数
来源：http://kho.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fzr.mhx1999.top

[S30] C：头文件保护
来源：http://zvd.tarul.cn

#ifndef X_H
来源：http://waz.jyoumei.cn

#define X_H
来源：http://zrj.jianghu66.top

#endif
来源：http://qzd.ehwqpu.com

[S31] C++：Hello World
来源：http://gjr.jianghu66.top

#include <iostream>
来源：http://lkc.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://alc.ydjk.org.cn

[S32] C++：字符串
来源：http://wfm.316326.xyz

std::string s = "hi";  s += "!";
来源：http://jbp.fzhhl.top

[S33] C++：vector 增删
来源：http://sem.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dhl.sufxvd.cn

[S34] C++：遍历 vector
来源：http://kya.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://twc.hywenlv.cn

[S35] C++：map
来源：http://mnw.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lym.tanke756.top

[S36] C++：unordered_map
来源：http://iis.andypj.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lxn.52xcode.cn

[S37] C++：set
来源：http://nqe.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xxv.yj202588.top

[S38] C++：排序
来源：http://zhw.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://vbc.yongpay.top

[S39] C++：自定义比较器排序
来源：http://evy.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dek.yvedp.cn

[S40] C++：查找元素
来源：http://wjc.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ppt.fengsongda.top

[S41] C++：类与构造函数
来源：http://yuu.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://loz.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://rim.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://gqx.hesvh.cn

[S43] C++：智能指针
来源：http://qqv.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://afb.fktsv.cn

[S44] C++：引用传参
来源：http://jfy.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://uxf.zhijiandao.cn

[S45] C++：lambda
来源：http://jdk.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nnq.jinqigfzy.top

[S46] C++：函数模板
来源：http://bpk.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pan.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://rmx.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rnm.bbcook.cn

[S48] C++：逐行读文件
来源：http://ctr.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://yki.c1oappe.top

while (std::getline(in, line)) { }
来源：http://uoc.yuxming.cn

[S49] C++：写文件
来源：http://hgc.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bht.cdnleiting.top

[S50] C++：格式化数字
来源：http://ddd.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ndv.mhx1999.top

[S51] C++：显式类型转换
来源：http://skt.daxiang520.top

static_cast<double>(a) / b
来源：http://buc.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://agd.cucudq.cn

int size() const noexcept { return n_; }
来源：http://zus.jqgfzy.top

[S53] C++：移动语义
来源：http://qsz.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://yoa.pengpengdd.cyou

[S54] C++：异常处理
来源：http://mpu.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jqz.bbcook.cn

[S55] C++：结构化绑定
来源：http://zgn.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://xaw.sufxvd.cn

[S56] C++：optional
来源：http://avv.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iwi.yangfankeji.com

[S57] C++：编译期常量
来源：http://zkp.yj20258.top

constexpr int N = 10;
来源：http://lus.hnxiangtu.top

[S58] C++：命名空间
来源：http://kct.jinyuanbaomall.cn

namespace ns { int f() { return 1; } }
来源：http://bpp.zhongyouzk.top

[S59] C++：静态断言
来源：http://jir.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yoh.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://rxw.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nfs.yuxming.cn

================================================================================
来源：http://dry.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mhy.aibaodan.cn

================================================================================
来源：http://rvj.hammf.cn

[T01] Kotlin：Hello World
来源：http://lnm.ywan-chungtsiang.top

println("Hello")
来源：http://boq.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://piz.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aqz.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://ttf.xziqi.cn

"值: $b"
来源：http://ozn.hywenlv.cn

[T04] Kotlin：空安全
来源：http://cqp.dianchejie.cn

val n: String? = null;  n?.length
来源：http://gxj.havefunace.top

[T05] Kotlin：when 表达式
来源：http://mjv.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ckm.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://anu.havefunace.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kzf.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://dqd.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pzy.gotoacloud.top

[T08] Kotlin：数据类
来源：http://cff.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://smm.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://nnf.pycfn.com

fun String.exclaim() = this + "!"
来源：http://gnu.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://sha.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://koz.316326.xyz

[T11] Kotlin：协程
来源：http://dcq.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mjm.zhiwuduotai.top

[T12] Kotlin：解构声明
来源：http://jwa.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://vrq.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://sss.guannengcc.top

val m = mapOf("a" to 1)
来源：http://eim.aizwys.cn

[T14] Kotlin：循环
来源：http://kgk.yonumen.top

for (i in 1..10) println(i)
来源：http://wit.birdmap.top

[T15] Kotlin：接口
来源：http://wtt.hesvh.cn

interface Shape { fun area(): Double }
来源：http://ztk.quarkkingdee.top

[T16] Swift：Hello World
来源：http://hak.svipenyu.cn

print("Hello")
来源：http://gop.dashuyun.cn

[T17] Swift：变量与常量
来源：http://vuw.hfpthk.cn

var a = 1;  let b = 2
来源：http://hce.jqgfzy.top

[T18] Swift：字符串插值
来源：http://sql.tanke756.top

"值: \(b)"
来源：http://waq.jinqigufen.top

[T19] Swift：可选绑定
来源：http://fdc.bbcook.cn

if let n = opt { print(n) }
来源：http://blm.cheryme.top

[T20] Swift：数组操作
来源：http://bec.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://wsj.yanxiufei.cn

[T21] Swift：遍历
来源：http://kub.yanxiufei.cn

for x in a { print(x) }
来源：http://big.nanxinkj.top

[T22] Swift：字典
来源：http://ujt.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://bdt.pengpengdd.cyou

[T23] Swift：函数
来源：http://kth.fengsongda.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zjb.havefunace.top

[T24] Swift：闭包
来源：http://tel.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ctz.zhijiandao.cn

[T25] Swift：结构体
来源：http://ezw.jyoumei.cn

struct P { var x: Int }
来源：http://opl.kuanghao11.cn

[T26] Swift：类与重写
来源：http://uot.epnwcf.com

class A: Base { override func f() {} }
来源：http://pih.xuanzx.com

[T27] Swift：错误处理
来源：http://mya.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://ins.jyoumei.cn

[T28] Swift：枚举
来源：http://ilv.havefunace.top

enum Color { case red, green }
来源：http://zfd.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://wun.gzhubu.top

guard let x = opt else { return }
来源：http://ipg.zdbjq.cn

[T30] Swift：协议
来源：http://mqo.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://eoy.316326.xyz

[T31] Lua：Hello World
来源：http://bax.uphjek.com

print("Hello")
来源：http://qdd.yonumen.top

[T32] Lua：局部变量
来源：http://vqs.ivvv.top

local a = 1
来源：http://xgb.zdqjudy.top

[T33] Lua：表（数组）
来源：http://ljl.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eox.ctjpmb.com

[T34] Lua：遍历表
来源：http://syt.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fwp.jlsjyb.cn

[T35] Lua：字典表
来源：http://wwv.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://pwb.svipenyu.cn

[T36] Lua：函数
来源：http://vry.nanxuanxn.top

function add(a, b) return a + b end
来源：http://cti.xylfe.cn

[T37] Lua：字符串拼接
来源：http://pyj.cqqwz.cn

"a" .. "b"
来源：http://dyq.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://moq.mhx1999.top

if x > 0 then print("正") end
来源：http://gla.shuidangran.top

[T39] Lua：模式匹配
来源：http://knx.gaohongyu789.top

string.find(s, "%d+")
来源：http://ufu.smart0.xyz

[T40] Lua：元表
来源：http://nin.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://kff.yvedp.cn

[T41] Perl：Hello World
来源：http://mch.xinyue.icu

print "Hello\n";
来源：http://wyj.cheryme.top

[T42] Perl：变量类型
来源：http://qfb.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jzb.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://iew.ppjwa.cn

"值: $a"
来源：http://ngj.havefunace.top

[T44] Perl：条件
来源：http://dmf.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://bzv.uphjek.com

[T45] Perl：数组遍历
来源：http://iqe.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://tzx.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://bsf.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ydg.sxryk.cn

[T47] Perl：正则捕获
来源：http://mzv.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://unn.cucudq.cn

[T48] Perl：正则替换
来源：http://mjs.316326.xyz

$s =~ s/old/new/g;
来源：http://oed.aibaodan.cn

[T49] Perl：函数
来源：http://reo.wangdashe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lmo.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://epo.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xah.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://fje.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://hzc.andypj.xyz

println("Hello")
来源：http://iyf.chenjidiqi.icu

[T52] Scala：变量
来源：http://acq.redwolf501.top

val a = 1;  var b = 2
来源：http://zrb.yj20258888.top

[T53] Scala：字符串插值
来源：http://htu.feifeiyinyue.top

s"值: $b"
来源：http://yez.ydjk.org.cn

[T54] Scala：集合映射
来源：http://yfx.shangyingyoupin.top

List(1, 2, 3).map(_ * 2)
来源：http://pmk.gogol.net.cn

[T55] Scala：集合过滤
来源：http://inz.tarul.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fsp.jianghu66.top

[T56] Scala：样例类
来源：http://akd.cashguo.top

case class User(name: String, age: Int)
来源：http://kvi.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://dyy.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://epv.ehwqpu.com

[T58] Scala：函数定义
来源：http://gxg.sweek.top

def add(a: Int, b: Int): Int = a + b
来源：http://vtz.tianlin.xyz

[T59] Scala：循环
来源：http://vaf.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://cak.gotoacloud.top

[T60] Scala：折叠
来源：http://abg.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aer.daxiang520.top

================================================================================
来源：http://fpa.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wtb.gogol.net.cn

================================================================================
来源：http://gvq.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://pwj.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://sqr.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://yew.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://voi.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://yqt.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://hld.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://hci.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kzj.hesvh.cn

[U05] Py：列表去重且保序
来源：http://atl.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://huw.hammf.cn

[U06] Py：合并两个字典
来源：http://hmm.sysykeji.top

{**a, **b}
来源：http://cfg.shangyingyoupin.top

[U07] Py：反转字典键值
来源：http://kti.0kj1m.cn

{v: k for k, v in d.items()}
来源：http://sxe.zycfv.cn

[U08] Py：展平二维列表
来源：http://quy.sjlbkw.cn

[y for x in nested for y in x]
来源：http://peo.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://vkp.fktsv.cn

max(d, key=d.get)
来源：http://nsq.redwolf501.top

[U10] Py：按值排序字典
来源：http://zuh.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bec.hysaishi.cn

[U11] Py：生成器表达式
来源：http://jvo.birdmap.top

(x * 2 for x in arr)
来源：http://fdq.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://lso.daxiang520.top

Counter(arr).most_common(3)
来源：http://afq.tarul.cn

[U13] Py：固定长度队列
来源：http://tjp.xuanzx.com

deque(maxlen=10)
来源：http://fuz.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://lee.ppjwa.cn

defaultdict(list)
来源：http://fuo.gaohongyu789.top

[U15] Py：高精度计时
来源：http://bpl.mhx1999.top

t = time.perf_counter()
来源：http://msr.sysykeji.top

[U16] Py：命令行参数解析
来源：http://dgo.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rot.ehwqpu.com

[U17] Py：初始化日志
来源：http://qea.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://ukh.xylfe.cn

[U18] Py：预编译正则
来源：http://bje.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://rgo.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://jfv.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sqi.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://tbv.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://say.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://imx.zhijiandao.cn

@contextlib.contextmanager
来源：http://spg.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://aag.hammf.cn

list(zip(*m))
来源：http://fke.gzhubu.top

[U23] Py：分块读取大文件
来源：http://lxi.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cjh.yuanzhike.top

[U24] Py：路径操作
来源：http://frn.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fax.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://sqz.hywenlv.cn

csv.DictReader(f)
来源：http://zwc.aibaodan.cn

[U26] Py：并发下载
来源：http://xia.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ltz.fktsv.cn


<!-- 参考信息 -->