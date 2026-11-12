代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://nbc.zycfv.cn

[S02] C：变量与格式化输出
来源：http://hoz.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://pgg.mhx1999.top

[S03] C：读入整数
来源：http://zym.havefunace.top

int x; scanf("%d", &x);
来源：http://ewi.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://bwd.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://uyh.yfazqb.com

[S05] C：字符串长度
来源：http://qgg.ybcxt.top

strlen(s)
来源：http://alq.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://wvm.redwolf501.top

strcmp(a, b) == 0
来源：http://kkv.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://fix.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vvr.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://zjw.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oev.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://tkn.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pvb.yj20258888.top

[S10] C：指针与解引用
来源：http://rks.yvedp.cn

int *p = &a;  *p = 5;
来源：http://ohx.ybcxt.top

[S11] C：逐行读文件
来源：http://pmu.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://olq.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gtd.gaohongyu789.top

fclose(f);
来源：http://wkr.cucudq.cn

[S12] C：写文件
来源：http://rbt.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cwy.gzhubu.top

[S13] C：宏定义
来源：http://xya.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oou.daxiang520.top

[S14] C：枚举
来源：http://mae.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://lnd.ehwqpu.com

[S15] C：类型转换
来源：http://csw.52xcode.cn

(double) a / b
来源：http://qem.nanxuanxn.top

[S16] C：位操作置位
来源：http://tue.bjfxy.top

x |= (1 << 3);
来源：http://puc.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://snb.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wny.fehbvm.com

[S18] C：命令行参数
来源：http://psi.daxiang520.top

int main(int argc, char **argv)
来源：http://mmw.0kj1m.cn

[S19] C：快速排序
来源：http://ynw.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zjo.zhiwuduotai.top

[S20] C：二分查找
来源：http://zxw.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://skv.birdmap.top

[S21] C：字符类别判断
来源：http://kzi.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://unr.chenlongwang.top

[S22] C：字符串转数字
来源：http://fch.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://nhy.zycfv.cn

[S23] C：随机数
来源：http://ksh.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bbf.quarkkingdee.top

[S24] C：获取本地时间
来源：http://cvl.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lmc.bjfxy.top

[S25] C：内存拷贝
来源：http://kln.jqgufenzy.top

memcpy(dst, src, n);
来源：http://ovt.yueranfly.top

[S26] C：内存清零
来源：http://eak.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://rda.sjlbkw.cn

[S27] C：定义常量
来源：http://mqg.pengpengdd.cyou

const double PI = 3.14159;
来源：http://ymj.yueranfly.top

[S28] C：静态变量
来源：http://irs.hywenlv.cn

static int counter = 0;
来源：http://rey.c1oappe.top

[S29] C：变参函数
来源：http://klm.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vto.zhoulong.xyz

[S30] C：头文件保护
来源：http://qek.dianchejie.cn

#ifndef X_H
来源：http://vtx.hongshengwenyu.top

#define X_H
来源：http://mmc.andypj.xyz

#endif
来源：http://dqx.hnqzz.top

[S31] C++：Hello World
来源：http://xvt.cucudq.cn

#include <iostream>
来源：http://wue.zhixingplan.top

int main() { std::cout << "Hello\n"; }
来源：http://ycp.yonumen.top

[S32] C++：字符串
来源：http://cdh.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://szu.zhongyouzk.top

[S33] C++：vector 增删
来源：http://ebm.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://exg.hfpthk.cn

[S34] C++：遍历 vector
来源：http://ktd.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://vzq.hysaishi.cn

[S35] C++：map
来源：http://ooy.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://txe.zhongyouzk.top

[S36] C++：unordered_map
来源：http://ihh.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ina.smart0.xyz

[S37] C++：set
来源：http://iqr.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oei.52xcode.cn

[S38] C++：排序
来源：http://hzu.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://fxc.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://kmm.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xqd.gzhubu.top

[S40] C++：查找元素
来源：http://oni.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ppn.yangfankeji.com

[S41] C++：类与构造函数
来源：http://gix.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xew.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://psv.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://qoh.daxiang520.top

[S43] C++：智能指针
来源：http://spx.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://dxn.hnxiangtu.top

[S44] C++：引用传参
来源：http://ily.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://ygo.yfazqb.com

[S45] C++：lambda
来源：http://enz.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dbi.316326.xyz

[S46] C++：函数模板
来源：http://ucl.jqgfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bzq.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://nmh.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zcw.pycfn.com

[S48] C++：逐行读文件
来源：http://jtn.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://hrd.cheryme.top

while (std::getline(in, line)) { }
来源：http://kot.nwbrower.top

[S49] C++：写文件
来源：http://qij.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cnn.havefunace.top

[S50] C++：格式化数字
来源：http://cac.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dct.vehdjk.com

[S51] C++：显式类型转换
来源：http://tfs.jinqigufen.top

static_cast<double>(a) / b
来源：http://ahr.yj202588.top

[S52] C++：const 与 noexcept
来源：http://qic.jianghu66.top

int size() const noexcept { return n_; }
来源：http://lkn.chenjidiqi.icu

[S53] C++：移动语义
来源：http://xgp.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://ykt.yuanzhike.top

[S54] C++：异常处理
来源：http://doe.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qoo.yfazqb.com

[S55] C++：结构化绑定
来源：http://npu.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qul.yonumen.top

[S56] C++：optional
来源：http://ise.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nzh.tanke756.top

[S57] C++：编译期常量
来源：http://rug.fzhhl.top

constexpr int N = 10;
来源：http://fmy.xuetiantiany.cn

[S58] C++：命名空间
来源：http://tsx.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://jnu.pycfn.com

[S59] C++：静态断言
来源：http://qyz.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vwk.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://caf.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gwm.guowangkeji.top

================================================================================
来源：http://tky.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nsy.jyoumei.cn

================================================================================
来源：http://uvw.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://qol.xuetiantiany.cn

println("Hello")
来源：http://mwf.havefunace.top

[T02] Kotlin：变量
来源：http://kcn.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://azj.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://yft.wangshuangyany.cn

"值: $b"
来源：http://amy.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://eek.gzhubu.top

val n: String? = null;  n?.length
来源：http://tgl.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://afs.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ekd.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://bcm.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://wml.cashguo.top

[T07] Kotlin：集合过滤
来源：http://dei.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jme.cdnleiting.top

[T08] Kotlin：数据类
来源：http://xpq.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://avz.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://ykm.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://tph.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://nmp.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://atx.9152youxi.cn

[T11] Kotlin：协程
来源：http://rfn.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zth.smart0.xyz

[T12] Kotlin：解构声明
来源：http://jsx.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://ixr.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://szq.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://nft.yuxming.cn

[T14] Kotlin：循环
来源：http://zlf.hysaishi.cn

for (i in 1..10) println(i)
来源：http://fbp.xziqi.cn

[T15] Kotlin：接口
来源：http://uzv.vehdjk.com

interface Shape { fun area(): Double }
来源：http://omn.ivvv.top

[T16] Swift：Hello World
来源：http://stj.yj20258.top

print("Hello")
来源：http://dyv.hesvh.cn

[T17] Swift：变量与常量
来源：http://eqr.birdmap.top

var a = 1;  let b = 2
来源：http://raq.dianchejie.cn

[T18] Swift：字符串插值
来源：http://aja.nwbrower.top

"值: \(b)"
来源：http://iua.9152youxi.cn

[T19] Swift：可选绑定
来源：http://swb.0kj1m.cn

if let n = opt { print(n) }
来源：http://aby.shzxlz.cn

[T20] Swift：数组操作
来源：http://omp.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://myy.yj20258.top

[T21] Swift：遍历
来源：http://flf.yuanzhike.top

for x in a { print(x) }
来源：http://vqx.nwbrower.top

[T22] Swift：字典
来源：http://lkn.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://lrb.yj20258.top

[T23] Swift：函数
来源：http://yho.jyoumei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bgn.fktsv.cn

[T24] Swift：闭包
来源：http://aed.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xrk.havefunace.top

[T25] Swift：结构体
来源：http://nfv.fanxiaobao.xyz

struct P { var x: Int }
来源：http://dpd.shzxlz.cn

[T26] Swift：类与重写
来源：http://okx.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://qtw.xuanzx.com

[T27] Swift：错误处理
来源：http://gde.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://bmt.birdmap.top

[T28] Swift：枚举
来源：http://bpc.bbcook.cn

enum Color { case red, green }
来源：http://xke.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://xdu.svipenyu.cn

guard let x = opt else { return }
来源：http://nda.hammf.cn

[T30] Swift：协议
来源：http://mzn.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://gfa.zhijiandao.cn

[T31] Lua：Hello World
来源：http://sjy.tarul.cn

print("Hello")
来源：http://rkc.tanke756.top

[T32] Lua：局部变量
来源：http://lkl.tanke756.top

local a = 1
来源：http://npf.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://jbu.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://mnl.hnxiangtu.top

[T34] Lua：遍历表
来源：http://vax.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bxb.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://kwz.zhoulong.xyz

local d = { a = 1 };  d.b = 2
来源：http://wdu.ydzc1.top

[T36] Lua：函数
来源：http://tgb.redwolf501.top

function add(a, b) return a + b end
来源：http://hgo.316326.xyz

[T37] Lua：字符串拼接
来源：http://kpq.bjfxy.top

"a" .. "b"
来源：http://ccz.aizwys.cn

[T38] Lua：条件
来源：http://akz.vqdsnc.cn

if x > 0 then print("正") end
来源：http://agi.tian-w.cn

[T39] Lua：模式匹配
来源：http://dig.gotoacloud.top

string.find(s, "%d+")
来源：http://xel.cheryme.top

[T40] Lua：元表
来源：http://vrr.uphjek.com

setmetatable({}, { __index = base })
来源：http://fxj.xuetiantiany.cn

[T41] Perl：Hello World
来源：http://hxl.ybcxt.top

print "Hello\n";
来源：http://pyr.hnxiangtu.top

[T42] Perl：变量类型
来源：http://rko.xziqi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mya.zdbjq.cn

[T43] Perl：字符串插值
来源：http://wxx.smart0.xyz

"值: $a"
来源：http://sml.cashguo.top

[T44] Perl：条件
来源：http://nhj.meibo888.top

if ($a > 0) { print "正"; }
来源：http://nis.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://puu.meibo888.top

for my $x (@arr) { print $x; }
来源：http://mhi.gogol.net.cn

[T46] Perl：哈希操作
来源：http://pkp.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bqz.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://lxw.xylfe.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ghg.cqqwz.cn

[T48] Perl：正则替换
来源：http://nzw.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://ibi.ppjwa.cn

[T49] Perl：函数
来源：http://frn.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yxy.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://isq.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://sfs.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://xgb.dianchejie.cn

[T51] Scala：Hello World
来源：http://nym.chenlongwang.top

println("Hello")
来源：http://xsl.hywenlv.cn

[T52] Scala：变量
来源：http://hqe.yvedp.cn

val a = 1;  var b = 2
来源：http://vye.cdnleiting.top

[T53] Scala：字符串插值
来源：http://vjt.c1oappe.top

s"值: $b"
来源：http://wbk.mhx1999.top

[T54] Scala：集合映射
来源：http://omm.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://xhx.gogol.net.cn

[T55] Scala：集合过滤
来源：http://vwa.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xky.xinyue.icu

[T56] Scala：样例类
来源：http://xxc.gogol.net.cn

case class User(name: String, age: Int)
来源：http://pyr.fehbvm.com

[T57] Scala：模式匹配
来源：http://usr.ehwqpu.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://muf.xuanzx.com

[T58] Scala：函数定义
来源：http://jdm.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://oxq.yj20258888.top

[T59] Scala：循环
来源：http://zfw.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://xmo.cashguo.top

[T60] Scala：折叠
来源：http://wib.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ggc.yongpay.top

================================================================================
来源：http://ajv.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rtj.tarul.cn

================================================================================
来源：http://sva.yanxiufei.cn

[U01] Py：创建虚拟环境
来源：http://ipc.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iaj.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://hlq.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bvm.ivvv.top

[U03] Py：加载 .env 配置
来源：http://zpw.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hcx.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://xnx.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jcv.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://lcg.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://ely.jinqigufen.top

[U06] Py：合并两个字典
来源：http://qur.epnwcf.com

{**a, **b}
来源：http://gwv.pycfn.com

[U07] Py：反转字典键值
来源：http://uxh.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://vvm.jyoumei.cn

[U08] Py：展平二维列表
来源：http://hip.sxryk.cn

[y for x in nested for y in x]
来源：http://tsv.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://cwb.bbcook.cn

max(d, key=d.get)
来源：http://mfd.epnwcf.com

[U10] Py：按值排序字典
来源：http://wan.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xtr.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://ecc.yj202588.top

(x * 2 for x in arr)
来源：http://pry.guowangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://kbs.xinyue.icu

Counter(arr).most_common(3)
来源：http://uep.jiagoushi.top

[U13] Py：固定长度队列
来源：http://abg.aibaodan.cn

deque(maxlen=10)
来源：http://kwi.zycfv.cn

[U14] Py：分组收集到列表
来源：http://tyr.tarul.cn

defaultdict(list)
来源：http://pgt.feifeiyinyue.top

[U15] Py：高精度计时
来源：http://tar.cdnleiting.top

t = time.perf_counter()
来源：http://gxs.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://ozf.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ook.cqqwz.cn

[U17] Py：初始化日志
来源：http://pvw.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://mhd.sjlbkw.cn

[U18] Py：预编译正则
来源：http://rjf.meibo888.top

pat = re.compile(r"\d+")
来源：http://fld.yj202588.top

[U19] Py：正则替换带回调
来源：http://pid.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vup.cheryme.top

[U20] Py：缓存函数结果
来源：http://hyu.ehwqpu.com

@functools.lru_cache(maxsize=None)
来源：http://dhd.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://kwg.jiagoushi.top

@contextlib.contextmanager
来源：http://vcf.dianchejie.cn

[U22] Py：矩阵转置
来源：http://kix.ctjpmb.com

list(zip(*m))
来源：http://ewn.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://rpt.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lcm.dianchejie.cn

[U24] Py：路径操作
来源：http://lcg.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qiu.smart0.xyz


<!-- 参考信息 -->