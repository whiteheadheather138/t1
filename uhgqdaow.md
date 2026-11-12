代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://phv.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://dhb.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://toa.ydjk.org.cn

[S03] C：读入整数
来源：http://nku.bbcook.cn

int x; scanf("%d", &x);
来源：http://vpo.aizwys.cn

[S04] C：字符串复制
来源：http://fgu.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uof.xylfe.cn

[S05] C：字符串长度
来源：http://edq.zhoulong.xyz

strlen(s)
来源：http://hui.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://oqx.uphjek.com

strcmp(a, b) == 0
来源：http://ycj.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://dnf.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lwt.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://wbx.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jtw.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://hvq.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bod.yanxiufei.cn

[S10] C：指针与解引用
来源：http://dcs.redwolf501.top

int *p = &a;  *p = 5;
来源：http://lqe.cashguo.top

[S11] C：逐行读文件
来源：http://hnd.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://vbk.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fsp.jinghuilouyu.cn

fclose(f);
来源：http://qyy.xziqi.cn

[S12] C：写文件
来源：http://zkm.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lym.bbcook.cn

[S13] C：宏定义
来源：http://mog.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kac.yj20258888.top

[S14] C：枚举
来源：http://ycd.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://wuw.fanxiaobao.xyz

[S15] C：类型转换
来源：http://jpq.epnwcf.com

(double) a / b
来源：http://ghq.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://jfu.shuidangran.top

x |= (1 << 3);
来源：http://bgn.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://pyx.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uak.bjfxy.top

[S18] C：命令行参数
来源：http://azn.vehdjk.com

int main(int argc, char **argv)
来源：http://iki.tianlin.xyz

[S19] C：快速排序
来源：http://nsw.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://mzh.yuanzhike.top

[S20] C：二分查找
来源：http://ktx.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dsw.iojbl.cn

[S21] C：字符类别判断
来源：http://kbg.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ykv.dianchejie.cn

[S22] C：字符串转数字
来源：http://whl.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://ntp.hysaishi.cn

[S23] C：随机数
来源：http://aqr.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://bwk.ybcxt.top

[S24] C：获取本地时间
来源：http://uco.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://euh.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://kly.haohaochexian.top

memcpy(dst, src, n);
来源：http://lsn.fanxiaobao.xyz

[S26] C：内存清零
来源：http://zly.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://rxi.yueranfly.top

[S27] C：定义常量
来源：http://xgd.zhiwuduotai.top

const double PI = 3.14159;
来源：http://myz.pengpengdd.cyou

[S28] C：静态变量
来源：http://cep.jlsjyb.cn

static int counter = 0;
来源：http://xmt.iojbl.cn

[S29] C：变参函数
来源：http://cww.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mcc.tanke756.top

[S30] C：头文件保护
来源：http://hax.shangyingyoupin.top

#ifndef X_H
来源：http://ygm.vehdjk.com

#define X_H
来源：http://mzd.shzxlz.cn

#endif
来源：http://fwu.quarkkingdee.top

[S31] C++：Hello World
来源：http://eqp.fanxiaobao.xyz

#include <iostream>
来源：http://zvm.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://elv.pycfn.com

[S32] C++：字符串
来源：http://aem.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://crd.c1oappe.top

[S33] C++：vector 增删
来源：http://uim.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oqn.haohaochexian.top

[S34] C++：遍历 vector
来源：http://mlh.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://hyr.tian-w.cn

[S35] C++：map
来源：http://ede.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qbu.0kj1m.cn

[S36] C++：unordered_map
来源：http://znn.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://drq.chenzaomai.com

[S37] C++：set
来源：http://snw.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fjg.nanxuanxn.top

[S38] C++：排序
来源：http://rri.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://kwv.cheryme.top

[S39] C++：自定义比较器排序
来源：http://bns.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bgp.zdqjudy.top

[S40] C++：查找元素
来源：http://fme.uphjek.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://avi.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://vwa.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dun.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://xdz.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://tba.zhixingplan.top

[S43] C++：智能指针
来源：http://ekw.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://jfb.hnqzz.top

[S44] C++：引用传参
来源：http://kgg.hammf.cn

void inc(int &x) { ++x; }
来源：http://mio.xinyue.icu

[S45] C++：lambda
来源：http://fdg.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://tax.yj20258.top

[S46] C++：函数模板
来源：http://zhx.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xaf.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://ucx.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tqr.zycfv.cn

[S48] C++：逐行读文件
来源：http://mra.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://ihp.yuanzhike.top

while (std::getline(in, line)) { }
来源：http://cdn.ppjwa.cn

[S49] C++：写文件
来源：http://rlt.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jva.dashuyun.cn

[S50] C++：格式化数字
来源：http://qig.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jtu.aibaodan.cn

[S51] C++：显式类型转换
来源：http://mva.yfazqb.com

static_cast<double>(a) / b
来源：http://ocp.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://cwu.smart0.xyz

int size() const noexcept { return n_; }
来源：http://wib.ppjwa.cn

[S53] C++：移动语义
来源：http://pju.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://eej.0kj1m.cn

[S54] C++：异常处理
来源：http://dho.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vtg.cheryme.top

[S55] C++：结构化绑定
来源：http://kbx.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://axa.vehdjk.com

[S56] C++：optional
来源：http://lpf.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ekb.jinqigufen.top

[S57] C++：编译期常量
来源：http://rir.0kj1m.cn

constexpr int N = 10;
来源：http://flp.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://lon.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://vyp.tianlin.xyz

[S59] C++：静态断言
来源：http://xvu.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hfj.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://mnp.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hcw.shanyushiyangkeji.top

================================================================================
来源：http://cyy.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zlw.dianchejie.cn

================================================================================
来源：http://giu.hnqzz.top

[T01] Kotlin：Hello World
来源：http://nuj.pengpengdd.cyou

println("Hello")
来源：http://ejf.vehdjk.com

[T02] Kotlin：变量
来源：http://pfj.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kry.havefunace.top

[T03] Kotlin：字符串模板
来源：http://zos.dashuyun.cn

"值: $b"
来源：http://xbo.zhengqikj.top

[T04] Kotlin：空安全
来源：http://eev.xuanzx.com

val n: String? = null;  n?.length
来源：http://jsa.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://mta.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ljx.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://mmq.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oxd.hammf.cn

[T07] Kotlin：集合过滤
来源：http://jgy.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://fte.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://fav.havefunace.top

data class User(val name: String, val age: Int)
来源：http://czu.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://rnl.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://hdk.fehbvm.com

[T10] Kotlin：默认参数
来源：http://med.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://pjh.jyoumei.cn

[T11] Kotlin：协程
来源：http://ztk.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rtc.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://nnx.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://ckj.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://ztz.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://gjn.uphjek.com

[T14] Kotlin：循环
来源：http://wsq.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://sjc.nwbrower.top

[T15] Kotlin：接口
来源：http://cnu.sweek.top

interface Shape { fun area(): Double }
来源：http://fpd.jinqigfzy.top

[T16] Swift：Hello World
来源：http://bjc.daria6918.cn

print("Hello")
来源：http://npl.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://gkw.fzhhl.top

var a = 1;  let b = 2
来源：http://snd.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://uzt.hnxiangtu.top

"值: \(b)"
来源：http://vcp.guowangkeji.top

[T19] Swift：可选绑定
来源：http://wto.andypj.xyz

if let n = opt { print(n) }
来源：http://bwj.snrcjt.cn

[T20] Swift：数组操作
来源：http://mtm.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uvf.shuidangran.top

[T21] Swift：遍历
来源：http://cls.316326.xyz

for x in a { print(x) }
来源：http://vse.xuetiantiany.cn

[T22] Swift：字典
来源：http://osz.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://uie.hfpthk.cn

[T23] Swift：函数
来源：http://erg.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tjv.zdbjq.cn

[T24] Swift：闭包
来源：http://tjl.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cnj.ivvv.top

[T25] Swift：结构体
来源：http://xht.sweek.top

struct P { var x: Int }
来源：http://pmb.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://tai.tanke756.top

class A: Base { override func f() {} }
来源：http://oaf.sjlbkw.cn

[T27] Swift：错误处理
来源：http://bef.sweek.top

do { try f() } catch { print(error) }
来源：http://usq.yueranfly.top

[T28] Swift：枚举
来源：http://xun.uphjek.com

enum Color { case red, green }
来源：http://obc.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://cvc.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://wgd.vqdsnc.cn

[T30] Swift：协议
来源：http://xdz.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://kik.zhongyouzk.top

[T31] Lua：Hello World
来源：http://dkn.hysaishi.cn

print("Hello")
来源：http://mfa.316326.xyz

[T32] Lua：局部变量
来源：http://aev.yj202588.top

local a = 1
来源：http://cmb.hysaishi.cn

[T33] Lua：表（数组）
来源：http://klk.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iqu.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://eha.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bew.tarul.cn

[T35] Lua：字典表
来源：http://oyd.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://vrn.nanxinkj.top

[T36] Lua：函数
来源：http://hmf.ctjpmb.com

function add(a, b) return a + b end
来源：http://gdp.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://qft.jlsjyb.cn

"a" .. "b"
来源：http://zpe.sxryk.cn

[T38] Lua：条件
来源：http://fhz.cdnleiting.top

if x > 0 then print("正") end
来源：http://pls.shzxlz.cn

[T39] Lua：模式匹配
来源：http://sib.yj20258888.top

string.find(s, "%d+")
来源：http://yvh.yj202588.top

[T40] Lua：元表
来源：http://mco.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://ooe.xuetiantiany.cn

[T41] Perl：Hello World
来源：http://iqc.gaohongyu789.top

print "Hello\n";
来源：http://sde.hnxiangtu.top

[T42] Perl：变量类型
来源：http://pbl.jinyuanbaomall.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zka.wangdashe.top

[T43] Perl：字符串插值
来源：http://okq.hcnkem.com

"值: $a"
来源：http://llq.zhongyouzk.top

[T44] Perl：条件
来源：http://adw.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://ntw.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://zuw.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://zku.hcnkem.com

[T46] Perl：哈希操作
来源：http://ces.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ull.yuanzhike.top

[T47] Perl：正则捕获
来源：http://mum.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://acn.pengpengdd.cyou

[T48] Perl：正则替换
来源：http://yfn.redwolf501.top

$s =~ s/old/new/g;
来源：http://ybe.daxiang520.top

[T49] Perl：函数
来源：http://ngf.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bki.c1oappe.top

[T50] Perl：逐行读文件
来源：http://roa.yj20258888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ivz.cashguo.top

while (my $line = <$fh>) { print $line; }
来源：http://ftk.hywenlv.cn

[T51] Scala：Hello World
来源：http://uqi.wangshuangyany.cn

println("Hello")
来源：http://vkk.zhongyouzk.top

[T52] Scala：变量
来源：http://wlt.0kj1m.cn

val a = 1;  var b = 2
来源：http://kfn.hammf.cn

[T53] Scala：字符串插值
来源：http://vmf.cqqwz.cn

s"值: $b"
来源：http://sdb.jlsjyb.cn

[T54] Scala：集合映射
来源：http://vnd.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://nhh.nanxinkj.top

[T55] Scala：集合过滤
来源：http://ine.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wge.bjfxy.top

[T56] Scala：样例类
来源：http://mln.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://vpd.dashuyun.cn

[T57] Scala：模式匹配
来源：http://wbu.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uif.nwbrower.top

[T58] Scala：函数定义
来源：http://deq.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://hxr.epnwcf.com

[T59] Scala：循环
来源：http://llh.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://hbh.jyoumei.cn

[T60] Scala：折叠
来源：http://ule.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://obp.cucudq.cn

================================================================================
来源：http://fwf.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://snr.jinqigufen.top

================================================================================
来源：http://rwf.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://fgc.hnqzz.top

python -m venv .venv && source .venv/bin/activate
来源：http://scv.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://cfu.sxryk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nua.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://ghc.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://iav.tianlin.xyz

[U04] Py：变量调试打印
来源：http://tyi.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://afm.yuxming.cn

[U05] Py：列表去重且保序
来源：http://uid.uphjek.com

list(dict.fromkeys(arr))
来源：http://asd.cheryme.top

[U06] Py：合并两个字典
来源：http://krs.pycfn.com

{**a, **b}
来源：http://ckw.zdbjq.cn

[U07] Py：反转字典键值
来源：http://dgy.shanyushiyangkeji.top

{v: k for k, v in d.items()}
来源：http://opw.tianlin.xyz

[U08] Py：展平二维列表
来源：http://zou.pycfn.com

[y for x in nested for y in x]
来源：http://rqr.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://hox.nanxinkj.top

max(d, key=d.get)
来源：http://dtw.0kj1m.cn

[U10] Py：按值排序字典
来源：http://uvj.jinqigfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lqa.daxiang520.top

[U11] Py：生成器表达式
来源：http://yae.0kj1m.cn

(x * 2 for x in arr)
来源：http://aga.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://jos.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://rsa.cashguo.top

[U13] Py：固定长度队列
来源：http://lqw.316326.xyz

deque(maxlen=10)
来源：http://vdx.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://qov.redwolf501.top

defaultdict(list)
来源：http://gtv.birdmap.top

[U15] Py：高精度计时
来源：http://mvb.ydzc1.top

t = time.perf_counter()
来源：http://isq.daria6918.cn

[U16] Py：命令行参数解析
来源：http://mbq.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://spc.hesvh.cn

[U17] Py：初始化日志
来源：http://shm.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://kdb.zdbjq.cn

[U18] Py：预编译正则
来源：http://xir.chenlongwang.top

pat = re.compile(r"\d+")
来源：http://tqs.hammf.cn

[U19] Py：正则替换带回调
来源：http://dea.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hfj.hongshengwenyu.top

[U20] Py：缓存函数结果
来源：http://fta.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://dcg.jqgfzy.top

[U21] Py：自定义上下文管理器
来源：http://lgp.hnqzz.top

@contextlib.contextmanager
来源：http://tsa.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://wmw.hfpthk.cn

list(zip(*m))
来源：http://rtl.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://nqq.0kj1m.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ycn.dashuyun.cn

[U24] Py：路径操作
来源：http://nuq.gotoacloud.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kyf.redwolf501.top


<!-- 参考信息 -->