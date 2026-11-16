代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://bwm.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://kjx.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://thx.zhoulong.xyz

[S03] C：读入整数
来源：http://fpq.jinqigufen.top

int x; scanf("%d", &x);
来源：http://rhd.c1oappe.top

[S04] C：字符串复制
来源：http://vbc.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://dbt.zhongyouzk.top

[S05] C：字符串长度
来源：http://zfe.vqdsnc.cn

strlen(s)
来源：http://luy.xuanzx.com

[S06] C：字符串比较
来源：http://hfh.birdmap.top

strcmp(a, b) == 0
来源：http://pwr.havefunace.top

[S07] C：数组遍历求和
来源：http://cic.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gug.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://wne.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://knt.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://gwj.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jkz.9152youxi.cn

[S10] C：指针与解引用
来源：http://zzj.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://nte.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://nit.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://ust.xziqi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cde.sjlbkw.cn

fclose(f);
来源：http://gdd.jqgufenzy.top

[S12] C：写文件
来源：http://zen.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zbf.yuanzhike.top

[S13] C：宏定义
来源：http://efo.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jei.jinqigfzy.top

[S14] C：枚举
来源：http://rfv.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://lrh.fktsv.cn

[S15] C：类型转换
来源：http://hdi.pycfn.com

(double) a / b
来源：http://ozt.cqqwz.cn

[S16] C：位操作置位
来源：http://eno.dashuyun.cn

x |= (1 << 3);
来源：http://ivl.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://phx.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xgx.chenlongwang.top

[S18] C：命令行参数
来源：http://gse.guannengcc.top

int main(int argc, char **argv)
来源：http://xtz.gaohongyu789.top

[S19] C：快速排序
来源：http://xbs.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xei.vehdjk.com

[S20] C：二分查找
来源：http://gdb.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jnq.ppjwa.cn

[S21] C：字符类别判断
来源：http://zbq.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gnd.tanke756.top

[S22] C：字符串转数字
来源：http://mon.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://erc.ydjk.org.cn

[S23] C：随机数
来源：http://miv.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hcr.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://efp.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ztr.xinyue.icu

[S25] C：内存拷贝
来源：http://jyb.jlsjyb.cn

memcpy(dst, src, n);
来源：http://ooq.xziqi.cn

[S26] C：内存清零
来源：http://gnt.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://jxa.xziqi.cn

[S27] C：定义常量
来源：http://ysf.jyoumei.cn

const double PI = 3.14159;
来源：http://bzl.wangshuangyany.cn

[S28] C：静态变量
来源：http://rrw.jlsjyb.cn

static int counter = 0;
来源：http://akh.hammf.cn

[S29] C：变参函数
来源：http://qcr.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qjz.cucudq.cn

[S30] C：头文件保护
来源：http://ssc.iojbl.cn

#ifndef X_H
来源：http://dcn.hesvh.cn

#define X_H
来源：http://xhc.iojbl.cn

#endif
来源：http://fon.fengsongda.top

[S31] C++：Hello World
来源：http://dxu.pycfn.com

#include <iostream>
来源：http://baq.shuidangran.top

int main() { std::cout << "Hello\n"; }
来源：http://yox.ydjk.org.cn

[S32] C++：字符串
来源：http://eyi.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://ybq.fengsongda.top

[S33] C++：vector 增删
来源：http://cgk.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jpn.aizwys.cn

[S34] C++：遍历 vector
来源：http://xpu.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://alb.ydzc1.top

[S35] C++：map
来源：http://oqs.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vza.yangfankeji.com

[S36] C++：unordered_map
来源：http://zpt.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uhw.fanxiaobao.xyz

[S37] C++：set
来源：http://bka.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pkc.yongpay.top

[S38] C++：排序
来源：http://iam.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://fvp.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://iay.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lkc.kuanghao11.cn

[S40] C++：查找元素
来源：http://tho.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://llw.bjfxy.top

[S41] C++：类与构造函数
来源：http://vvy.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xse.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://cbp.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://uvz.yj20258888.top

[S43] C++：智能指针
来源：http://xkr.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://tri.tarul.cn

[S44] C++：引用传参
来源：http://fue.epnwcf.com

void inc(int &x) { ++x; }
来源：http://mgj.zhongyouzk.top

[S45] C++：lambda
来源：http://clw.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zmd.sweek.top

[S46] C++：函数模板
来源：http://hzx.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jqw.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://vft.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cxh.cqqwz.cn

[S48] C++：逐行读文件
来源：http://xuf.zhijiandao.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gps.hammf.cn

while (std::getline(in, line)) { }
来源：http://eky.haohaochexian.top

[S49] C++：写文件
来源：http://gla.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bhf.shzxlz.cn

[S50] C++：格式化数字
来源：http://sft.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zvw.gogol.net.cn

[S51] C++：显式类型转换
来源：http://vlz.fengsongda.top

static_cast<double>(a) / b
来源：http://yib.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://svf.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://ayi.sjlbkw.cn

[S53] C++：移动语义
来源：http://plf.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://mno.c1oappe.top

[S54] C++：异常处理
来源：http://ime.hnxiangtu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://loy.wangdashe.top

[S55] C++：结构化绑定
来源：http://kfp.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://mtv.dianchejie.cn

[S56] C++：optional
来源：http://udc.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rri.zhijiandao.cn

[S57] C++：编译期常量
来源：http://udc.zdbjq.cn

constexpr int N = 10;
来源：http://yek.chenjidiqi.icu

[S58] C++：命名空间
来源：http://dag.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://iqo.yanxiufei.cn

[S59] C++：静态断言
来源：http://wws.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vvu.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://jjw.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qij.daria6918.cn

================================================================================
来源：http://fdr.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pry.sjlbkw.cn

================================================================================
来源：http://qnn.yfazqb.com

[T01] Kotlin：Hello World
来源：http://uyt.snrcjt.cn

println("Hello")
来源：http://pff.epnwcf.com

[T02] Kotlin：变量
来源：http://ifo.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hps.sweek.top

[T03] Kotlin：字符串模板
来源：http://lba.xingfuxueyuan.xyz

"值: $b"
来源：http://ang.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://eeu.birdmap.top

val n: String? = null;  n?.length
来源：http://mzn.cashguo.top

[T05] Kotlin：when 表达式
来源：http://bai.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sze.jianghu66.top

[T06] Kotlin：集合映射
来源：http://gcu.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hyo.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://cod.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://cxn.mhx1999.top

[T08] Kotlin：数据类
来源：http://axj.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://azl.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://cwb.nwbrower.top

fun String.exclaim() = this + "!"
来源：http://dba.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://cco.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://asy.ivvv.top

[T11] Kotlin：协程
来源：http://pes.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gzk.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://bfc.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://zos.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://sad.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://wwn.svipenyu.cn

[T14] Kotlin：循环
来源：http://dui.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://izd.zhixingplan.top

[T15] Kotlin：接口
来源：http://ltb.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://jqm.gzhubu.top

[T16] Swift：Hello World
来源：http://lfk.ydjk.org.cn

print("Hello")
来源：http://prw.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://nye.0kj1m.cn

var a = 1;  let b = 2
来源：http://uiy.tarul.cn

[T18] Swift：字符串插值
来源：http://vvd.gzhubu.top

"值: \(b)"
来源：http://cgp.jianghu66.top

[T19] Swift：可选绑定
来源：http://vjk.yueranfly.top

if let n = opt { print(n) }
来源：http://wbn.kuanghao11.cn

[T20] Swift：数组操作
来源：http://qza.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hrr.ydjk.org.cn

[T21] Swift：遍历
来源：http://ygx.redwolf501.top

for x in a { print(x) }
来源：http://zrq.52xcode.cn

[T22] Swift：字典
来源：http://dws.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://lzo.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://kez.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zum.svipenyu.cn

[T24] Swift：闭包
来源：http://ehq.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wsx.aizwys.cn

[T25] Swift：结构体
来源：http://zoi.tianlin.xyz

struct P { var x: Int }
来源：http://ynx.daxiang520.top

[T26] Swift：类与重写
来源：http://rhr.jiagoushi.top

class A: Base { override func f() {} }
来源：http://msk.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://flt.yj202588.top

do { try f() } catch { print(error) }
来源：http://iib.epnwcf.com

[T28] Swift：枚举
来源：http://pqt.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://auc.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://bti.yfazqb.com

guard let x = opt else { return }
来源：http://unk.shuidangran.top

[T30] Swift：协议
来源：http://eki.cashguo.top

protocol Shape { func area() -> Double }
来源：http://hxv.jinqigufen.top

[T31] Lua：Hello World
来源：http://clp.bjfxy.top

print("Hello")
来源：http://fgt.birdmap.top

[T32] Lua：局部变量
来源：http://dtu.zycfv.cn

local a = 1
来源：http://nau.aizwys.cn

[T33] Lua：表（数组）
来源：http://ggg.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mla.nanxinkj.top

[T34] Lua：遍历表
来源：http://jgb.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gpj.fehbvm.com

[T35] Lua：字典表
来源：http://odt.wangshuangyany.cn

local d = { a = 1 };  d.b = 2
来源：http://ipf.jianghu66.top

[T36] Lua：函数
来源：http://xjx.nanxuanxn.top

function add(a, b) return a + b end
来源：http://wdf.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://ydv.yuxming.cn

"a" .. "b"
来源：http://oiq.gzhubu.top

[T38] Lua：条件
来源：http://kbw.dianchejie.cn

if x > 0 then print("正") end
来源：http://yrv.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://qhe.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://hsl.zhongyouzk.top

[T40] Lua：元表
来源：http://obq.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://qce.tanke756.top

[T41] Perl：Hello World
来源：http://kge.svipenyu.cn

print "Hello\n";
来源：http://xms.ydjk.org.cn

[T42] Perl：变量类型
来源：http://wej.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ozk.shanyushiyangkeji.top

[T43] Perl：字符串插值
来源：http://lmz.jqgufenzy.top

"值: $a"
来源：http://cfw.xingfuxueyuan.xyz

[T44] Perl：条件
来源：http://xjb.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://zwr.hfpthk.cn

[T45] Perl：数组遍历
来源：http://fiw.yj20258.top

for my $x (@arr) { print $x; }
来源：http://nzg.jinghuilouyu.cn

[T46] Perl：哈希操作
来源：http://jjs.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oiv.tanke756.top

[T47] Perl：正则捕获
来源：http://dxw.haohaochexian.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xnd.vehdjk.com

[T48] Perl：正则替换
来源：http://jjv.52xcode.cn

$s =~ s/old/new/g;
来源：http://twr.ppjwa.cn

[T49] Perl：函数
来源：http://yph.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://shf.cheryme.top

[T50] Perl：逐行读文件
来源：http://vyh.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lew.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://zby.iojbl.cn

[T51] Scala：Hello World
来源：http://bwi.iojbl.cn

println("Hello")
来源：http://afw.meibo888.top

[T52] Scala：变量
来源：http://bkd.daria6918.cn

val a = 1;  var b = 2
来源：http://rsp.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://tkx.ywan-chungtsiang.top

s"值: $b"
来源：http://ors.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://cyz.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://rcm.dashuyun.cn

[T55] Scala：集合过滤
来源：http://upn.zdbjq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ffa.yj20258.top

[T56] Scala：样例类
来源：http://ami.chenlongwang.top

case class User(name: String, age: Int)
来源：http://dun.hfpthk.cn

[T57] Scala：模式匹配
来源：http://hng.tian-w.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eaa.hnqzz.top

[T58] Scala：函数定义
来源：http://mqw.sysykeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://ftt.hnqzz.top

[T59] Scala：循环
来源：http://wqb.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://dqm.yj202588.top

[T60] Scala：折叠
来源：http://ltn.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qxl.tian-w.cn

================================================================================
来源：http://bwf.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://meq.yj20258.top

================================================================================
来源：http://ljd.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://eim.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://huz.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://ecq.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://skx.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://gqo.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nfq.tanke756.top

[U04] Py：变量调试打印
来源：http://dbz.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jaw.c1oappe.top

[U05] Py：列表去重且保序
来源：http://sss.fktsv.cn

list(dict.fromkeys(arr))
来源：http://qrj.tarul.cn

[U06] Py：合并两个字典
来源：http://hzm.fehbvm.com

{**a, **b}
来源：http://fhv.jlsjyb.cn

[U07] Py：反转字典键值
来源：http://dcn.nwbrower.top

{v: k for k, v in d.items()}
来源：http://krn.zhengqikj.top

[U08] Py：展平二维列表
来源：http://gmm.ppjwa.cn

[y for x in nested for y in x]
来源：http://hfc.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://ios.ehwqpu.com

max(d, key=d.get)
来源：http://wgv.shzxlz.cn

[U10] Py：按值排序字典
来源：http://pqe.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nly.andypj.xyz

[U11] Py：生成器表达式
来源：http://yuh.jiagoushi.top

(x * 2 for x in arr)
来源：http://uox.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zdq.tian-w.cn

Counter(arr).most_common(3)
来源：http://jui.uphjek.com

[U13] Py：固定长度队列
来源：http://yhb.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://mxr.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://yju.birdmap.top

defaultdict(list)
来源：http://bda.epnwcf.com

[U15] Py：高精度计时
来源：http://rti.epnwcf.com

t = time.perf_counter()
来源：http://hpr.sysykeji.top

[U16] Py：命令行参数解析
来源：http://lon.gotoacloud.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eck.bbcook.cn

[U17] Py：初始化日志
来源：http://peh.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://yzb.yongpay.top

[U18] Py：预编译正则
来源：http://lps.fktsv.cn

pat = re.compile(r"\d+")
来源：http://drf.vehdjk.com

[U19] Py：正则替换带回调
来源：http://rvu.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://puv.zhiwuduotai.top

[U20] Py：缓存函数结果
来源：http://xmu.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://gxc.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://qxq.shuidangran.top

@contextlib.contextmanager
来源：http://cjw.316326.xyz

[U22] Py：矩阵转置
来源：http://aar.guowangkeji.top

list(zip(*m))
来源：http://vrc.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://dqt.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zpy.xinyue.icu

[U24] Py：路径操作
来源：http://qhu.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ppf.xuetiantiany.cn


<!-- 参考信息 -->