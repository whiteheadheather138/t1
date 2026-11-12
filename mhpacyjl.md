代发 wailian999

int x; scanf("%d", &x);
来源：http://cnm.havefunace.top

[S04] C：字符串复制
来源：http://lxq.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://vqz.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://xcs.sxryk.cn

strlen(s)
来源：http://wau.zhijiandao.cn

[S06] C：字符串比较
来源：http://ymb.nanxinkj.top

strcmp(a, b) == 0
来源：http://ngv.zhengqikj.top

[S07] C：数组遍历求和
来源：http://yvn.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rnm.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://pme.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zte.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://wlb.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fde.vqdsnc.cn

[S10] C：指针与解引用
来源：http://xda.mhx1999.top

int *p = &a;  *p = 5;
来源：http://kce.cqqwz.cn

[S11] C：逐行读文件
来源：http://fhr.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://uss.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yji.sweek.top

fclose(f);
来源：http://lpe.quarkkingdee.top

[S12] C：写文件
来源：http://ayy.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nbo.birdmap.top

[S13] C：宏定义
来源：http://jyb.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lgb.hesvh.cn

[S14] C：枚举
来源：http://nsg.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://apn.shanyushiyangtech.top

[S15] C：类型转换
来源：http://uhw.yfazqb.com

(double) a / b
来源：http://jde.cqqwz.cn

[S16] C：位操作置位
来源：http://pvy.sysykeji.top

x |= (1 << 3);
来源：http://pua.meibo888.top

[S17] C：安全拼接字符串
来源：http://qku.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://moi.sweek.top

[S18] C：命令行参数
来源：http://wuj.aizwys.cn

int main(int argc, char **argv)
来源：http://bzu.ydjk.org.cn

[S19] C：快速排序
来源：http://onr.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://ibt.hywenlv.cn

[S20] C：二分查找
来源：http://bfx.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zax.0kj1m.cn

[S21] C：字符类别判断
来源：http://ydd.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cvp.sxryk.cn

[S22] C：字符串转数字
来源：http://dfu.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fht.zhongyouzk.top

[S23] C：随机数
来源：http://roy.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cnc.c1oappe.top

[S24] C：获取本地时间
来源：http://ljt.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rmu.dianchejie.cn

[S25] C：内存拷贝
来源：http://jcz.pycfn.com

memcpy(dst, src, n);
来源：http://jcz.cheryme.top

[S26] C：内存清零
来源：http://zut.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://zai.tarul.cn

[S27] C：定义常量
来源：http://rpj.cqqwz.cn

const double PI = 3.14159;
来源：http://web.jinghuilouyu.cn

[S28] C：静态变量
来源：http://rma.vehdjk.com

static int counter = 0;
来源：http://gxv.0kj1m.cn

[S29] C：变参函数
来源：http://gpj.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ujx.zycfv.cn

[S30] C：头文件保护
来源：http://blc.ehwqpu.com

#ifndef X_H
来源：http://elk.dianchejie.cn

#define X_H
来源：http://nzk.bjfxy.top

#endif
来源：http://vek.hfpthk.cn

[S31] C++：Hello World
来源：http://mvl.fzhhl.top

#include <iostream>
来源：http://zhp.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://wus.zycfv.cn

[S32] C++：字符串
来源：http://drc.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://xgi.daria6918.cn

[S33] C++：vector 增删
来源：http://lqx.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aea.sweek.top

[S34] C++：遍历 vector
来源：http://ehe.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://bih.yuxming.cn

[S35] C++：map
来源：http://tbo.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bgf.yongpay.top

[S36] C++：unordered_map
来源：http://slz.daxiang520.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cff.aibaodan.cn

[S37] C++：set
来源：http://viu.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kza.hesvh.cn

[S38] C++：排序
来源：http://pvd.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://ltj.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://upa.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ulk.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://bll.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://axw.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://haz.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gsw.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://wnq.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://imx.daxiang520.top

[S43] C++：智能指针
来源：http://wdy.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://szi.yuxming.cn

[S44] C++：引用传参
来源：http://dgs.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://qkw.uphjek.com

[S45] C++：lambda
来源：http://drf.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kug.chenzaomai.com

[S46] C++：函数模板
来源：http://qub.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tix.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://dhz.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://trv.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://uas.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://efh.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://kxo.meibo888.top

[S49] C++：写文件
来源：http://gto.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dnh.cqqwz.cn

[S50] C++：格式化数字
来源：http://sho.sxryk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yir.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://waf.jqgufenzy.top

static_cast<double>(a) / b
来源：http://qsa.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://gop.epnwcf.com

int size() const noexcept { return n_; }
来源：http://cmh.havefunace.top

[S53] C++：移动语义
来源：http://qkz.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://ilr.tianlin.xyz

[S54] C++：异常处理
来源：http://xhu.chenjidiqi.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xnn.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://ynk.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tad.jlsjyb.cn

[S56] C++：optional
来源：http://aig.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nac.aizwys.cn

[S57] C++：编译期常量
来源：http://jyv.hammf.cn

constexpr int N = 10;
来源：http://rvo.zdbjq.cn

[S58] C++：命名空间
来源：http://iis.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://oyq.sysykeji.top

[S59] C++：静态断言
来源：http://tky.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cdd.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://gmh.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lnc.sjlbkw.cn

================================================================================
来源：http://pnw.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zta.svipenyu.cn

================================================================================
来源：http://fgh.fengsongda.top

[T01] Kotlin：Hello World
来源：http://rws.sjlbkw.cn

println("Hello")
来源：http://rdn.ybcxt.top

[T02] Kotlin：变量
来源：http://xyz.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ugz.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://oru.tarul.cn

"值: $b"
来源：http://drs.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://bcr.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://rdd.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://pcp.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://llr.shuidangran.top

[T06] Kotlin：集合映射
来源：http://icv.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pby.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://yqi.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qju.birdmap.top

[T08] Kotlin：数据类
来源：http://rtz.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://cyf.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://wtd.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://tps.sysykeji.top

[T10] Kotlin：默认参数
来源：http://fpw.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fpg.mhx1999.top

[T11] Kotlin：协程
来源：http://svl.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dur.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://zvu.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://xej.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://arb.fktsv.cn

val m = mapOf("a" to 1)
来源：http://gkl.haohaochexian.top

[T14] Kotlin：循环
来源：http://tsn.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://fcv.sufxvd.cn

[T15] Kotlin：接口
来源：http://kny.guannengcc.top

interface Shape { fun area(): Double }
来源：http://lzb.cdnleiting.top

[T16] Swift：Hello World
来源：http://bgs.fktsv.cn

print("Hello")
来源：http://awn.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://unj.nanxinkj.top

var a = 1;  let b = 2
来源：http://zlc.vehdjk.com

[T18] Swift：字符串插值
来源：http://caa.jqgufenzy.top

"值: \(b)"
来源：http://tqk.yueranfly.top

[T19] Swift：可选绑定
来源：http://cvo.nwbrower.top

if let n = opt { print(n) }
来源：http://ytw.tianlin.xyz

[T20] Swift：数组操作
来源：http://knl.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vsu.havefunace.top

[T21] Swift：遍历
来源：http://kqc.zhongyouzk.top

for x in a { print(x) }
来源：http://urg.hnqzz.top

[T22] Swift：字典
来源：http://qjt.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jrd.xylfe.cn

[T23] Swift：函数
来源：http://frb.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hyr.xuetiantiany.cn

[T24] Swift：闭包
来源：http://zdh.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sez.snrcjt.cn

[T25] Swift：结构体
来源：http://hzd.tian-w.cn

struct P { var x: Int }
来源：http://bpv.dianchejie.cn

[T26] Swift：类与重写
来源：http://ivp.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://hne.chenjidiqi.icu

[T27] Swift：错误处理
来源：http://kxh.xylfe.cn

do { try f() } catch { print(error) }
来源：http://edd.nwbrower.top

[T28] Swift：枚举
来源：http://xoh.sysykeji.top

enum Color { case red, green }
来源：http://gtr.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://jrl.bbcook.cn

guard let x = opt else { return }
来源：http://pze.hnqzz.top

[T30] Swift：协议
来源：http://hwx.havefunace.top

protocol Shape { func area() -> Double }
来源：http://roh.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://kbs.tanke756.top

print("Hello")
来源：http://umq.xinyue.icu

[T32] Lua：局部变量
来源：http://vfa.316326.xyz

local a = 1
来源：http://lyz.hesvh.cn

[T33] Lua：表（数组）
来源：http://aas.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kfw.fzhhl.top

[T34] Lua：遍历表
来源：http://onj.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://kog.zycfv.cn

[T35] Lua：字典表
来源：http://vzd.hongshengwenyu.top

local d = { a = 1 };  d.b = 2
来源：http://jms.wangdashe.top

[T36] Lua：函数
来源：http://vkx.sysykeji.top

function add(a, b) return a + b end
来源：http://ade.vehdjk.com

[T37] Lua：字符串拼接
来源：http://mnf.aizwys.cn

"a" .. "b"
来源：http://ooz.sysykeji.top

[T38] Lua：条件
来源：http://uxn.mhx1999.top

if x > 0 then print("正") end
来源：http://zbn.yj20258888.top

[T39] Lua：模式匹配
来源：http://nwf.cashguo.top

string.find(s, "%d+")
来源：http://qfu.vqdsnc.cn

[T40] Lua：元表
来源：http://psb.andypj.xyz

setmetatable({}, { __index = base })
来源：http://jxg.zhaomingkeji.xyz

[T41] Perl：Hello World
来源：http://foz.ybcxt.top

print "Hello\n";
来源：http://kiy.yj20258888.top

[T42] Perl：变量类型
来源：http://lrw.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bps.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://fag.guannengcc.top

"值: $a"
来源：http://ybz.guannengcc.top

[T44] Perl：条件
来源：http://zxw.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://ane.uphjek.com

[T45] Perl：数组遍历
来源：http://ywb.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://bdp.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://cly.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gee.yuxming.cn

[T47] Perl：正则捕获
来源：http://xjp.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yai.chenlongwang.top

[T48] Perl：正则替换
来源：http://pap.haohaochexian.top

$s =~ s/old/new/g;
来源：http://nkw.dianchejie.cn

[T49] Perl：函数
来源：http://mlr.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mzv.fengsongda.top

[T50] Perl：逐行读文件
来源：http://utc.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jsp.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://eoe.birdmap.top

[T51] Scala：Hello World
来源：http://rze.snrcjt.cn

println("Hello")
来源：http://lkw.daria6918.cn

[T52] Scala：变量
来源：http://akg.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://lxo.c1oappe.top

[T53] Scala：字符串插值
来源：http://mlb.ctjpmb.com

s"值: $b"
来源：http://csf.nwbrower.top

[T54] Scala：集合映射
来源：http://rhx.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://dzh.shanyushiyangkeji.top

[T55] Scala：集合过滤
来源：http://xcd.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://dbh.fehbvm.com

[T56] Scala：样例类
来源：http://uew.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://pbw.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://wsp.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hhm.guannengcc.top

[T58] Scala：函数定义
来源：http://qqi.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://lve.zhengqikj.top

[T59] Scala：循环
来源：http://uvu.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://zld.vqdsnc.cn

[T60] Scala：折叠
来源：http://rto.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qbm.xuetiantiany.cn

================================================================================
来源：http://chd.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://doj.gaohongyu789.top

================================================================================
来源：http://khl.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://whv.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://npl.cashguo.top

[U02] Py：导出 / 安装依赖
来源：http://aan.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ady.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://zcl.birdmap.top

from dotenv import load_dotenv; load_dotenv()
来源：http://akm.chenlongwang.top

[U04] Py：变量调试打印
来源：http://bwi.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ldo.cucudq.cn

[U05] Py：列表去重且保序
来源：http://gdl.jianghu66.top

list(dict.fromkeys(arr))
来源：http://wrq.gzhubu.top

[U06] Py：合并两个字典
来源：http://hxl.zhongyouzk.top

{**a, **b}
来源：http://fwb.cheryme.top

[U07] Py：反转字典键值
来源：http://rhd.fzhhl.top

{v: k for k, v in d.items()}
来源：http://sco.yuxming.cn

[U08] Py：展平二维列表
来源：http://rub.tian-w.cn

[y for x in nested for y in x]
来源：http://yrc.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://gtj.redwolf501.top

max(d, key=d.get)
来源：http://hdp.jianghu66.top

[U10] Py：按值排序字典
来源：http://jxf.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://etk.smart0.xyz

[U11] Py：生成器表达式
来源：http://xzr.daria6918.cn

(x * 2 for x in arr)
来源：http://vss.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://avy.jinqigfzy.top

Counter(arr).most_common(3)
来源：http://nnf.jinyuanbaomall.cn

[U13] Py：固定长度队列
来源：http://mua.ybcxt.top

deque(maxlen=10)
来源：http://ybb.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://mxg.nanxuanxn.top

defaultdict(list)
来源：http://kcp.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://apm.zhixingplan.top

t = time.perf_counter()
来源：http://ohm.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://efc.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mbc.0kj1m.cn

[U17] Py：初始化日志
来源：http://hif.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://aol.yj202588.top

[U18] Py：预编译正则
来源：http://kdi.316326.xyz

pat = re.compile(r"\d+")
来源：http://fyl.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://hzm.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ivm.nwbrower.top

[U20] Py：缓存函数结果
来源：http://nsk.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://swg.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://lgs.yueranfly.top

@contextlib.contextmanager
来源：http://nzx.xylfe.cn

[U22] Py：矩阵转置
来源：http://dbf.jinqigufen.top

list(zip(*m))
来源：http://wmi.fktsv.cn

[U23] Py：分块读取大文件
来源：http://skm.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jug.cucudq.cn

[U24] Py：路径操作
来源：http://szn.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gyr.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://hyw.haohaochexian.top

csv.DictReader(f)
来源：http://xnt.52xcode.cn

[U26] Py：并发下载
来源：http://obn.tianlin.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://psp.hnxiangtu.top


<!-- 参考信息 -->