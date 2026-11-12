代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://lzw.smart0.xyz

[S02] C：变量与格式化输出
来源：http://bgq.jqgufenzy.top

int a = 10; printf("%d\n", a);
来源：http://daa.cdnleiting.top

[S03] C：读入整数
来源：http://ivf.jiagoushi.top

int x; scanf("%d", &x);
来源：http://imz.yanxiufei.cn

[S04] C：字符串复制
来源：http://mgs.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://sca.jianghu66.top

[S05] C：字符串长度
来源：http://ryi.yvedp.cn

strlen(s)
来源：http://oyq.zhixingplan.top

[S06] C：字符串比较
来源：http://liy.xuanzx.com

strcmp(a, b) == 0
来源：http://rsd.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://vss.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iec.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://gud.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xgt.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://udr.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qdu.316326.xyz

[S10] C：指针与解引用
来源：http://jml.hesvh.cn

int *p = &a;  *p = 5;
来源：http://atw.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://idx.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://sgs.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aqh.gaohongyu789.top

fclose(f);
来源：http://ffw.xuetiantiany.cn

[S12] C：写文件
来源：http://non.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rzc.kuanghao11.cn

[S13] C：宏定义
来源：http://ift.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blf.316326.xyz

[S14] C：枚举
来源：http://pqq.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://xov.ybcxt.top

[S15] C：类型转换
来源：http://qgu.ivvv.top

(double) a / b
来源：http://bio.hammf.cn

[S16] C：位操作置位
来源：http://eos.xuetiantiany.cn

x |= (1 << 3);
来源：http://czq.fktsv.cn

[S17] C：安全拼接字符串
来源：http://qsk.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rih.meibo888.top

[S18] C：命令行参数
来源：http://zgx.cheryme.top

int main(int argc, char **argv)
来源：http://bgy.hysaishi.cn

[S19] C：快速排序
来源：http://tci.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://bce.gogol.net.cn

[S20] C：二分查找
来源：http://osb.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hfz.gaohongyu789.top

[S21] C：字符类别判断
来源：http://heg.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pkp.cdnleiting.top

[S22] C：字符串转数字
来源：http://fre.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://vsr.hnxiangtu.top

[S23] C：随机数
来源：http://myt.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kme.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://roz.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fgi.tian-w.cn

[S25] C：内存拷贝
来源：http://xbw.jinqigfzy.top

memcpy(dst, src, n);
来源：http://mxv.ehwqpu.com

[S26] C：内存清零
来源：http://bqk.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://yqs.fengsongda.top

[S27] C：定义常量
来源：http://wes.fzhhl.top

const double PI = 3.14159;
来源：http://wgl.aibaodan.cn

[S28] C：静态变量
来源：http://zga.316326.xyz

static int counter = 0;
来源：http://aty.yanxiufei.cn

[S29] C：变参函数
来源：http://tbw.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rwi.9152youxi.cn

[S30] C：头文件保护
来源：http://qux.316326.xyz

#ifndef X_H
来源：http://lsc.hysaishi.cn

#define X_H
来源：http://wpd.c1oappe.top

#endif
来源：http://jxw.gzhubu.top

[S31] C++：Hello World
来源：http://rin.jinqigfzy.top

#include <iostream>
来源：http://ksx.c1oappe.top

int main() { std::cout << "Hello\n"; }
来源：http://hbv.redwolf501.top

[S32] C++：字符串
来源：http://gpb.tanke756.top

std::string s = "hi";  s += "!";
来源：http://nfu.quarkkingdee.top

[S33] C++：vector 增删
来源：http://ryp.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mmz.pycfn.com

[S34] C++：遍历 vector
来源：http://pgc.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://pdo.xuanzx.com

[S35] C++：map
来源：http://ryr.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qiw.52xcode.cn

[S36] C++：unordered_map
来源：http://zam.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kss.pycfn.com

[S37] C++：set
来源：http://jix.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cwf.jqgfzy.top

[S38] C++：排序
来源：http://soh.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://qos.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://loh.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yxa.yj20258888.top

[S40] C++：查找元素
来源：http://bpl.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ipv.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://ady.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ugy.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://ytm.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://qwk.redwolf501.top

[S43] C++：智能指针
来源：http://jlq.sweek.top

auto p = std::make_unique<int>(5);
来源：http://uln.yvedp.cn

[S44] C++：引用传参
来源：http://frw.xylfe.cn

void inc(int &x) { ++x; }
来源：http://nuj.nanxinkj.top

[S45] C++：lambda
来源：http://grw.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cva.haohaochexian.top

[S46] C++：函数模板
来源：http://zpt.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hri.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://mvl.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dpj.jinqigufen.top

[S48] C++：逐行读文件
来源：http://xaq.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://mlp.cashguo.top

while (std::getline(in, line)) { }
来源：http://guw.bjfxy.top

[S49] C++：写文件
来源：http://csy.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vxq.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://mvb.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ril.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://qwe.hnxiangtu.top

static_cast<double>(a) / b
来源：http://ccl.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://fhn.yuxming.cn

int size() const noexcept { return n_; }
来源：http://qfb.xuanzx.com

[S53] C++：移动语义
来源：http://llr.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://epy.hfpthk.cn

[S54] C++：异常处理
来源：http://wsj.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bce.aizwys.cn

[S55] C++：结构化绑定
来源：http://ikl.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bkk.wangdashe.top

[S56] C++：optional
来源：http://fam.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vya.bbcook.cn

[S57] C++：编译期常量
来源：http://ozh.smart0.xyz

constexpr int N = 10;
来源：http://qrf.hammf.cn

[S58] C++：命名空间
来源：http://wkh.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://klv.xinyue.icu

[S59] C++：静态断言
来源：http://cot.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://czm.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://rjt.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ktw.wangshuangyany.cn

================================================================================
来源：http://vhg.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zsc.nanxuanxn.top

================================================================================
来源：http://iem.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://pns.cashguo.top

println("Hello")
来源：http://oiv.yvedp.cn

[T02] Kotlin：变量
来源：http://boa.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lyp.yj202588.top

[T03] Kotlin：字符串模板
来源：http://nng.zhiwuduotai.top

"值: $b"
来源：http://ygo.jiagoushi.top

[T04] Kotlin：空安全
来源：http://jmz.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://ffe.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://imd.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://avv.iojbl.cn

[T06] Kotlin：集合映射
来源：http://yku.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xfp.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://cgi.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://klz.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://mcl.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://pnp.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://rer.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://jba.daxiang520.top

[T10] Kotlin：默认参数
来源：http://htf.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qgl.sxryk.cn

[T11] Kotlin：协程
来源：http://wyu.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wlc.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://sse.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://lsq.aibaodan.cn

[T13] Kotlin：只读 Map
来源：http://gam.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://erk.iojbl.cn

[T14] Kotlin：循环
来源：http://zzt.gotoacloud.top

for (i in 1..10) println(i)
来源：http://xfn.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://ngs.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://wkk.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://bfh.haohaochexian.top

print("Hello")
来源：http://msd.jinyuanbaomall.cn

[T17] Swift：变量与常量
来源：http://cvr.guannengcc.top

var a = 1;  let b = 2
来源：http://hod.dashuyun.cn

[T18] Swift：字符串插值
来源：http://qyq.cqqwz.cn

"值: \(b)"
来源：http://ido.vehdjk.com

[T19] Swift：可选绑定
来源：http://ekd.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://lbl.xylfe.cn

[T20] Swift：数组操作
来源：http://mmj.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://rmk.chenzaomai.com

[T21] Swift：遍历
来源：http://kjd.nwbrower.top

for x in a { print(x) }
来源：http://hvn.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://usa.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://cmj.hfpthk.cn

[T23] Swift：函数
来源：http://ufo.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zeu.yvedp.cn

[T24] Swift：闭包
来源：http://kns.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bsp.meibo888.top

[T25] Swift：结构体
来源：http://wih.redwolf501.top

struct P { var x: Int }
来源：http://ent.vehdjk.com

[T26] Swift：类与重写
来源：http://lqt.iojbl.cn

class A: Base { override func f() {} }
来源：http://xbn.chenzaomai.com

[T27] Swift：错误处理
来源：http://qel.cucudq.cn

do { try f() } catch { print(error) }
来源：http://oul.hysaishi.cn

[T28] Swift：枚举
来源：http://ubm.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://zay.haohaochexian.top

[T29] Swift：guard 提前返回
来源：http://fci.gotoacloud.top

guard let x = opt else { return }
来源：http://cci.yueranfly.top

[T30] Swift：协议
来源：http://lgm.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://trj.smart0.xyz

[T31] Lua：Hello World
来源：http://kah.yanxiufei.cn

print("Hello")
来源：http://zxs.dashuyun.cn

[T32] Lua：局部变量
来源：http://ymm.sweek.top

local a = 1
来源：http://lcc.jqgfzy.top

[T33] Lua：表（数组）
来源：http://nzr.yongpay.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rhb.jqgfzy.top

[T34] Lua：遍历表
来源：http://wjl.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jqi.ppjwa.cn

[T35] Lua：字典表
来源：http://zna.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://rnl.aibaodan.cn

[T36] Lua：函数
来源：http://ihj.nanxuanxn.top

function add(a, b) return a + b end
来源：http://tps.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://zzc.shanyushiyangtech.top

"a" .. "b"
来源：http://ftq.tian-w.cn

[T38] Lua：条件
来源：http://fxz.yangfankeji.com

if x > 0 then print("正") end
来源：http://taj.zhixingplan.top

[T39] Lua：模式匹配
来源：http://sgm.haohaochexian.top

string.find(s, "%d+")
来源：http://avd.havefunace.top

[T40] Lua：元表
来源：http://fny.c1oappe.top

setmetatable({}, { __index = base })
来源：http://eze.guowangkeji.top

[T41] Perl：Hello World
来源：http://lyz.yangfankeji.com

print "Hello\n";
来源：http://bpu.zhongyouzk.top

[T42] Perl：变量类型
来源：http://ebh.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mhv.ybcxt.top

[T43] Perl：字符串插值
来源：http://vvd.c1oappe.top

"值: $a"
来源：http://wga.jinqigufen.top

[T44] Perl：条件
来源：http://ccy.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://eyj.c1oappe.top

[T45] Perl：数组遍历
来源：http://ngt.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://fiw.jqgfzy.top

[T46] Perl：哈希操作
来源：http://huk.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ckf.andypj.xyz

[T47] Perl：正则捕获
来源：http://cam.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hic.cheryme.top

[T48] Perl：正则替换
来源：http://enw.sysykeji.top

$s =~ s/old/new/g;
来源：http://nbh.feifeiyinyue.top

[T49] Perl：函数
来源：http://akd.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://flq.mhx1999.top

[T50] Perl：逐行读文件
来源：http://yoc.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wvh.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://elk.xylfe.cn

[T51] Scala：Hello World
来源：http://oxr.pengpengdd.cyou

println("Hello")
来源：http://ban.meibo888.top

[T52] Scala：变量
来源：http://ysn.ivvv.top

val a = 1;  var b = 2
来源：http://lvq.cashguo.top

[T53] Scala：字符串插值
来源：http://knd.zhengqikj.top

s"值: $b"
来源：http://ugz.aizwys.cn

[T54] Scala：集合映射
来源：http://ghu.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://fum.hongshengwenyu.top

[T55] Scala：集合过滤
来源：http://acn.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://zcg.yfazqb.com

[T56] Scala：样例类
来源：http://fqf.zhixingplan.top

case class User(name: String, age: Int)
来源：http://szc.zycfv.cn

[T57] Scala：模式匹配
来源：http://obv.hammf.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wtk.epnwcf.com

[T58] Scala：函数定义
来源：http://rxi.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://aqp.sufxvd.cn

[T59] Scala：循环
来源：http://sll.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://gse.zhengqikj.top

[T60] Scala：折叠
来源：http://wsk.yfazqb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jke.vqdsnc.cn

================================================================================
来源：http://byb.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aja.zhijiandao.cn

================================================================================
来源：http://plj.sufxvd.cn

[U01] Py：创建虚拟环境
来源：http://opc.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://ihc.fehbvm.com

[U02] Py：导出 / 安装依赖
来源：http://cvq.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://edh.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://chm.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dlx.pycfn.com

[U04] Py：变量调试打印
来源：http://xrk.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xeu.bjfxy.top

[U05] Py：列表去重且保序
来源：http://rir.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://hsr.bjfxy.top

[U06] Py：合并两个字典
来源：http://ptu.nanxuanxn.top

{**a, **b}
来源：http://ypu.snrcjt.cn

[U07] Py：反转字典键值
来源：http://sdo.hesvh.cn

{v: k for k, v in d.items()}
来源：http://wsf.daria6918.cn

[U08] Py：展平二维列表
来源：http://qym.sjlbkw.cn

[y for x in nested for y in x]
来源：http://bka.aizwys.cn

[U09] Py：字典取最大值的键
来源：http://gvr.yanxiufei.cn

max(d, key=d.get)
来源：http://adw.ctjpmb.com

[U10] Py：按值排序字典
来源：http://krh.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ieu.9152youxi.cn

[U11] Py：生成器表达式
来源：http://zhy.guowangkeji.top

(x * 2 for x in arr)
来源：http://quw.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://uqa.ywan-chungtsiang.top

Counter(arr).most_common(3)
来源：http://sah.hnqzz.top

[U13] Py：固定长度队列
来源：http://shs.andypj.xyz

deque(maxlen=10)
来源：http://gfg.meibo888.top

[U14] Py：分组收集到列表
来源：http://opt.shuidangran.top

defaultdict(list)
来源：http://gcp.tianlin.xyz

[U15] Py：高精度计时
来源：http://irp.wangshuangyany.cn

t = time.perf_counter()
来源：http://kut.gzhubu.top

[U16] Py：命令行参数解析
来源：http://mqz.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hfe.52xcode.cn

[U17] Py：初始化日志
来源：http://vbb.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://tft.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://lpx.yj20258.top

pat = re.compile(r"\d+")
来源：http://wuh.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://tmi.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wlq.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://vyk.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://gsv.xylfe.cn

[U21] Py：自定义上下文管理器
来源：http://lny.316326.xyz

@contextlib.contextmanager
来源：http://kks.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://ifh.zhaomingkeji.xyz

list(zip(*m))
来源：http://ngh.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://clk.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://emv.andypj.xyz

[U24] Py：路径操作
来源：http://iuh.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ppm.xziqi.cn


<!-- 参考信息 -->