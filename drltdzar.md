代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://vji.yfazqb.com

[S02] C：变量与格式化输出
来源：http://lar.nanxinkj.top

int a = 10; printf("%d\n", a);
来源：http://zyg.yj20258.top

[S03] C：读入整数
来源：http://mlt.dashuyun.cn

int x; scanf("%d", &x);
来源：http://iye.uphjek.com

[S04] C：字符串复制
来源：http://mld.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://ccu.zdbjq.cn

[S05] C：字符串长度
来源：http://vdh.sjlbkw.cn

strlen(s)
来源：http://gly.chenlongwang.top

[S06] C：字符串比较
来源：http://ucz.cdnleiting.top

strcmp(a, b) == 0
来源：http://ely.sufxvd.cn

[S07] C：数组遍历求和
来源：http://lbx.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://era.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://ykj.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rfq.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://pzo.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://snx.jinqigfzy.top

[S10] C：指针与解引用
来源：http://rst.zhiwuduotai.top

int *p = &a;  *p = 5;
来源：http://dkl.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://mjs.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://quf.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://slj.yj20258.top

fclose(f);
来源：http://ltf.iojbl.cn

[S12] C：写文件
来源：http://wtz.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iam.bbcook.cn

[S13] C：宏定义
来源：http://pvo.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cfw.chenlongwang.top

[S14] C：枚举
来源：http://rzb.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://nue.ctjpmb.com

[S15] C：类型转换
来源：http://eel.sxryk.cn

(double) a / b
来源：http://bvr.yueranfly.top

[S16] C：位操作置位
来源：http://dfb.hywenlv.cn

x |= (1 << 3);
来源：http://xeb.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://klw.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://spj.kuanghao11.cn

[S18] C：命令行参数
来源：http://hxk.vehdjk.com

int main(int argc, char **argv)
来源：http://orq.316326.xyz

[S19] C：快速排序
来源：http://yoq.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://szn.jinghuilouyu.cn

[S20] C：二分查找
来源：http://dwy.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ycg.tianlin.xyz

[S21] C：字符类别判断
来源：http://hvt.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xpo.zhengqikj.top

[S22] C：字符串转数字
来源：http://vys.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://vbk.andypj.xyz

[S23] C：随机数
来源：http://gcb.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xrq.andypj.xyz

[S24] C：获取本地时间
来源：http://uug.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vyz.zhijiandao.cn

[S25] C：内存拷贝
来源：http://fqf.xuanzx.com

memcpy(dst, src, n);
来源：http://ozv.cashguo.top

[S26] C：内存清零
来源：http://plv.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://cvi.cashguo.top

[S27] C：定义常量
来源：http://qbt.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://vcy.cucudq.cn

[S28] C：静态变量
来源：http://taq.gzhubu.top

static int counter = 0;
来源：http://nuo.ydzc1.top

[S29] C：变参函数
来源：http://jxe.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zak.hesvh.cn

[S30] C：头文件保护
来源：http://zha.fehbvm.com

#ifndef X_H
来源：http://gmx.fanxiaobao.xyz

#define X_H
来源：http://qfr.nanxinkj.top

#endif
来源：http://ymt.zdqjudy.top

[S31] C++：Hello World
来源：http://nby.gotoacloud.top

#include <iostream>
来源：http://tkn.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://abi.gzhubu.top

[S32] C++：字符串
来源：http://ryt.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://dqs.bjfxy.top

[S33] C++：vector 增删
来源：http://kyn.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lbg.tianlin.xyz

[S34] C++：遍历 vector
来源：http://tdi.ybcxt.top

for (auto &x : v) { std::cout << x; }
来源：http://xce.nanxinkj.top

[S35] C++：map
来源：http://ncz.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bgy.daxiang520.top

[S36] C++：unordered_map
来源：http://oeu.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ndk.xingfuxueyuan.xyz

[S37] C++：set
来源：http://mep.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xjj.chenzaomai.com

[S38] C++：排序
来源：http://prj.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://deb.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://vqk.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://niq.ybcxt.top

[S40] C++：查找元素
来源：http://bjz.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gci.ydzc1.top

[S41] C++：类与构造函数
来源：http://zcp.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oam.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://wun.sweek.top

class B : public Base { public: void f() override {} };
来源：http://cbt.fzhhl.top

[S43] C++：智能指针
来源：http://fwy.sjlbkw.cn

auto p = std::make_unique<int>(5);
来源：http://xyd.tanke756.top

[S44] C++：引用传参
来源：http://qsr.vehdjk.com

void inc(int &x) { ++x; }
来源：http://pyl.zhengqikj.top

[S45] C++：lambda
来源：http://nkd.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://vsp.shuidangran.top

[S46] C++：函数模板
来源：http://epr.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mth.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://ehy.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ubj.nwbrower.top

[S48] C++：逐行读文件
来源：http://azk.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://txb.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://rmn.hysaishi.cn

[S49] C++：写文件
来源：http://skm.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tem.52xcode.cn

[S50] C++：格式化数字
来源：http://ahg.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://apo.havefunace.top

[S51] C++：显式类型转换
来源：http://eju.snrcjt.cn

static_cast<double>(a) / b
来源：http://lha.cheryme.top

[S52] C++：const 与 noexcept
来源：http://mtg.c1oappe.top

int size() const noexcept { return n_; }
来源：http://vql.yongpay.top

[S53] C++：移动语义
来源：http://toh.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://ubt.sxryk.cn

[S54] C++：异常处理
来源：http://swg.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ogp.gzhubu.top

[S55] C++：结构化绑定
来源：http://cgy.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ehg.yongpay.top

[S56] C++：optional
来源：http://wxq.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://htg.hcnkem.com

[S57] C++：编译期常量
来源：http://wop.fengsongda.top

constexpr int N = 10;
来源：http://sgq.xuanzx.com

[S58] C++：命名空间
来源：http://jcm.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://txr.jiagoushi.top

[S59] C++：静态断言
来源：http://ftd.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mhr.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://myc.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nut.fanxiaobao.xyz

================================================================================
来源：http://aqt.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hvq.9152youxi.cn

================================================================================
来源：http://zgp.cashguo.top

[T01] Kotlin：Hello World
来源：http://xsz.xingfuxueyuan.xyz

println("Hello")
来源：http://kky.hcnkem.com

[T02] Kotlin：变量
来源：http://enw.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jtg.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://qug.guannengcc.top

"值: $b"
来源：http://xby.52xcode.cn

[T04] Kotlin：空安全
来源：http://rvf.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://zxe.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://uad.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nwu.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://oue.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tkx.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://vku.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uol.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://wbw.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://bch.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://aba.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://lsx.tanke756.top

[T10] Kotlin：默认参数
来源：http://diu.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://aut.sysykeji.top

[T11] Kotlin：协程
来源：http://zmi.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tno.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://avl.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://fec.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://mli.mhx1999.top

val m = mapOf("a" to 1)
来源：http://jwp.tanke756.top

[T14] Kotlin：循环
来源：http://jfv.cashguo.top

for (i in 1..10) println(i)
来源：http://cuq.pengpengdd.cyou

[T15] Kotlin：接口
来源：http://qxv.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://gvj.gaohongyu789.top

[T16] Swift：Hello World
来源：http://bph.aizwys.cn

print("Hello")
来源：http://pmy.guannengcc.top

[T17] Swift：变量与常量
来源：http://hpb.ydjk.org.cn

var a = 1;  let b = 2
来源：http://gcq.smart0.xyz

[T18] Swift：字符串插值
来源：http://zhc.c1oappe.top

"值: \(b)"
来源：http://mho.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://fed.guannengcc.top

if let n = opt { print(n) }
来源：http://xqv.yfazqb.com

[T20] Swift：数组操作
来源：http://jcj.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://tpj.haohaochexian.top

[T21] Swift：遍历
来源：http://keg.pengpengdd.cyou

for x in a { print(x) }
来源：http://ual.hcnkem.com

[T22] Swift：字典
来源：http://xke.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fnc.zhiwuduotai.top

[T23] Swift：函数
来源：http://dyd.zhaomingkeji.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lou.chenlongwang.top

[T24] Swift：闭包
来源：http://tmm.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ljk.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://uef.vehdjk.com

struct P { var x: Int }
来源：http://pve.c1oappe.top

[T26] Swift：类与重写
来源：http://vad.0kj1m.cn

class A: Base { override func f() {} }
来源：http://mla.chenzaomai.com

[T27] Swift：错误处理
来源：http://cju.gzhubu.top

do { try f() } catch { print(error) }
来源：http://bli.birdmap.top

[T28] Swift：枚举
来源：http://pjg.uphjek.com

enum Color { case red, green }
来源：http://uib.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://ffj.chenzaomai.com

guard let x = opt else { return }
来源：http://rsf.tianlin.xyz

[T30] Swift：协议
来源：http://jka.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://aqo.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://tmb.jinqigufen.top

print("Hello")
来源：http://dwf.chenzaomai.com

[T32] Lua：局部变量
来源：http://rcp.yueranfly.top

local a = 1
来源：http://npv.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://lda.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://geo.gotoacloud.top

[T34] Lua：遍历表
来源：http://oec.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gys.zhijiandao.cn

[T35] Lua：字典表
来源：http://snt.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://ijt.daxiang520.top

[T36] Lua：函数
来源：http://wgw.mhx1999.top

function add(a, b) return a + b end
来源：http://ohg.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://sws.yanxiufei.cn

"a" .. "b"
来源：http://vqq.cheryme.top

[T38] Lua：条件
来源：http://ids.guowangkeji.top

if x > 0 then print("正") end
来源：http://int.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://hza.vehdjk.com

string.find(s, "%d+")
来源：http://ebu.zhixingplan.top

[T40] Lua：元表
来源：http://hxt.ydzc1.top

setmetatable({}, { __index = base })
来源：http://qfa.jinqigfzy.top

[T41] Perl：Hello World
来源：http://lww.316326.xyz

print "Hello\n";
来源：http://pjk.fehbvm.com

[T42] Perl：变量类型
来源：http://iny.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zfk.fanxiaobao.xyz

[T43] Perl：字符串插值
来源：http://fyt.hcnkem.com

"值: $a"
来源：http://ulm.iojbl.cn

[T44] Perl：条件
来源：http://nik.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://unm.gzhubu.top

[T45] Perl：数组遍历
来源：http://uiu.ivvv.top

for my $x (@arr) { print $x; }
来源：http://biw.guowangkeji.top

[T46] Perl：哈希操作
来源：http://yvy.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kkf.zhengqikj.top

[T47] Perl：正则捕获
来源：http://btn.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ala.shuidangran.top

[T48] Perl：正则替换
来源：http://fjf.jqgfzy.top

$s =~ s/old/new/g;
来源：http://fcj.gzhubu.top

[T49] Perl：函数
来源：http://hxt.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rgk.hcnkem.com

[T50] Perl：逐行读文件
来源：http://doa.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://vjv.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://cpo.yangfankeji.com

[T51] Scala：Hello World
来源：http://czx.wangshuangyany.cn

println("Hello")
来源：http://com.tianlin.xyz

[T52] Scala：变量
来源：http://kyi.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://zxt.guowangkeji.top

[T53] Scala：字符串插值
来源：http://oxr.gzhubu.top

s"值: $b"
来源：http://wjp.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://pfk.0kj1m.cn

List(1, 2, 3).map(_ * 2)
来源：http://jim.jyoumei.cn

[T55] Scala：集合过滤
来源：http://snm.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://ylt.jyoumei.cn

[T56] Scala：样例类
来源：http://nqf.andypj.xyz

case class User(name: String, age: Int)
来源：http://wjo.tarul.cn

[T57] Scala：模式匹配
来源：http://hjf.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://nfq.iojbl.cn

[T58] Scala：函数定义
来源：http://aun.guowangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://bea.hnqzz.top

[T59] Scala：循环
来源：http://mqj.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://fob.yj20258.top

[T60] Scala：折叠
来源：http://abo.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iys.daria6918.cn

================================================================================
来源：http://fce.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zcx.yueranfly.top

================================================================================
来源：http://vhq.birdmap.top

[U01] Py：创建虚拟环境
来源：http://qqi.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://blt.pycfn.com

[U02] Py：导出 / 安装依赖
来源：http://lnb.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kra.fktsv.cn

[U03] Py：加载 .env 配置
来源：http://nsr.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://npt.smart0.xyz

[U04] Py：变量调试打印
来源：http://lpx.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bcr.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://vhs.cashguo.top

list(dict.fromkeys(arr))
来源：http://vzf.zycfv.cn

[U06] Py：合并两个字典
来源：http://twp.tian-w.cn

{**a, **b}
来源：http://fql.zhaomingkeji.xyz

[U07] Py：反转字典键值
来源：http://nwz.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://mxk.sufxvd.cn

[U08] Py：展平二维列表
来源：http://bqd.quarkkingdee.top

[y for x in nested for y in x]
来源：http://lxy.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://ltb.dashuyun.cn

max(d, key=d.get)
来源：http://mld.havefunace.top

[U10] Py：按值排序字典
来源：http://vtr.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://frt.jinqigufen.top

[U11] Py：生成器表达式
来源：http://odn.jianghu66.top

(x * 2 for x in arr)
来源：http://pwj.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ffk.tarul.cn

Counter(arr).most_common(3)
来源：http://org.ydzc1.top

[U13] Py：固定长度队列
来源：http://zzw.havefunace.top

deque(maxlen=10)
来源：http://rqa.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://rxi.gotoacloud.top

defaultdict(list)
来源：http://sfy.ppjwa.cn

[U15] Py：高精度计时
来源：http://uis.nwbrower.top

t = time.perf_counter()
来源：http://lnk.zycfv.cn

[U16] Py：命令行参数解析
来源：http://qqm.yfazqb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mmh.hysaishi.cn

[U17] Py：初始化日志
来源：http://jbn.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://lwp.316326.xyz

[U18] Py：预编译正则
来源：http://esf.wangdashe.top

pat = re.compile(r"\d+")
来源：http://imr.epnwcf.com

[U19] Py：正则替换带回调
来源：http://nga.shangyingyoupin.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tgo.iojbl.cn

[U20] Py：缓存函数结果
来源：http://xmq.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://nim.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://mmk.sxryk.cn

@contextlib.contextmanager
来源：http://lcc.shuidangran.top

[U22] Py：矩阵转置
来源：http://zfd.jinghuilouyu.cn

list(zip(*m))
来源：http://vgs.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://nbs.zhijiandao.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wiq.gotoacloud.top

[U24] Py：路径操作
来源：http://dib.chenlongwang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wbu.ybcxt.top


<!-- 参考信息 -->