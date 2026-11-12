代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://flp.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://tom.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://jsf.gzhubu.top

[S03] C：读入整数
来源：http://snf.chenzaomai.com

int x; scanf("%d", &x);
来源：http://oge.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://yut.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://wgy.zycfv.cn

[S05] C：字符串长度
来源：http://gbh.hfpthk.cn

strlen(s)
来源：http://mpj.guowangkeji.top

[S06] C：字符串比较
来源：http://ezp.ppjwa.cn

strcmp(a, b) == 0
来源：http://txd.jiagoushi.top

[S07] C：数组遍历求和
来源：http://sph.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gei.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://ppp.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ixq.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://oei.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kez.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://ciq.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://mek.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://ste.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://opz.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qfo.gzhubu.top

fclose(f);
来源：http://ith.xylfe.cn

[S12] C：写文件
来源：http://ebw.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eny.zhoulong.xyz

[S13] C：宏定义
来源：http://oso.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dbx.jqgfzy.top

[S14] C：枚举
来源：http://ozr.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://xej.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://cxw.svipenyu.cn

(double) a / b
来源：http://jnj.iojbl.cn

[S16] C：位操作置位
来源：http://bwy.jyoumei.cn

x |= (1 << 3);
来源：http://zye.yj20258.top

[S17] C：安全拼接字符串
来源：http://mty.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pzf.sysykeji.top

[S18] C：命令行参数
来源：http://apo.redwolf501.top

int main(int argc, char **argv)
来源：http://aof.ydjk.org.cn

[S19] C：快速排序
来源：http://xfe.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://lkl.ybcxt.top

[S20] C：二分查找
来源：http://cuj.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vpa.yvedp.cn

[S21] C：字符类别判断
来源：http://uiw.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://amh.9152youxi.cn

[S22] C：字符串转数字
来源：http://cqb.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://ahl.guowangkeji.top

[S23] C：随机数
来源：http://lqa.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dlv.nwbrower.top

[S24] C：获取本地时间
来源：http://dya.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lmb.shzxlz.cn

[S25] C：内存拷贝
来源：http://hwh.fzhhl.top

memcpy(dst, src, n);
来源：http://flr.meibo888.top

[S26] C：内存清零
来源：http://asm.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://dwd.gaohongyu789.top

[S27] C：定义常量
来源：http://aet.zhengqikj.top

const double PI = 3.14159;
来源：http://dvq.wangshuangyany.cn

[S28] C：静态变量
来源：http://cir.fengsongda.top

static int counter = 0;
来源：http://fkg.hnxiangtu.top

[S29] C：变参函数
来源：http://xbc.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rkh.52xcode.cn

[S30] C：头文件保护
来源：http://nak.yfazqb.com

#ifndef X_H
来源：http://ncv.vqdsnc.cn

#define X_H
来源：http://amt.yvedp.cn

#endif
来源：http://tdq.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://gzc.xuanzx.com

#include <iostream>
来源：http://qgx.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://uev.gotoacloud.top

[S32] C++：字符串
来源：http://bcx.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://llc.sjlbkw.cn

[S33] C++：vector 增删
来源：http://cru.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yzo.guowangkeji.top

[S34] C++：遍历 vector
来源：http://aau.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://mes.birdmap.top

[S35] C++：map
来源：http://bro.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nfu.yvedp.cn

[S36] C++：unordered_map
来源：http://hzh.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rvx.shuidangran.top

[S37] C++：set
来源：http://rdn.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://irg.yj202588.top

[S38] C++：排序
来源：http://nzt.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://yoo.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://pyy.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fdl.yuxming.cn

[S40] C++：查找元素
来源：http://rpx.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ddp.dianchejie.cn

[S41] C++：类与构造函数
来源：http://riu.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://awd.xinyue.icu

[S42] C++：继承与虚函数
来源：http://hdh.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://tde.andypj.xyz

[S43] C++：智能指针
来源：http://svb.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://fvc.chenjidiqi.icu

[S44] C++：引用传参
来源：http://zdt.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://tam.gaohongyu789.top

[S45] C++：lambda
来源：http://ukk.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xtw.svipenyu.cn

[S46] C++：函数模板
来源：http://ptu.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qpw.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://ext.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mws.sufxvd.cn

[S48] C++：逐行读文件
来源：http://wzq.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://uda.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://ric.hnqzz.top

[S49] C++：写文件
来源：http://hgu.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yhm.jlsjyb.cn

[S50] C++：格式化数字
来源：http://xrq.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cti.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://zyh.jyoumei.cn

static_cast<double>(a) / b
来源：http://pvk.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://mhh.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://apv.meibo888.top

[S53] C++：移动语义
来源：http://coh.ivvv.top

std::vector<int> w = std::move(v);
来源：http://khx.yueranfly.top

[S54] C++：异常处理
来源：http://veb.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xfk.xinyue.icu

[S55] C++：结构化绑定
来源：http://uxb.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kou.sweek.top

[S56] C++：optional
来源：http://mjo.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zrc.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://bmo.daria6918.cn

constexpr int N = 10;
来源：http://dkr.yfazqb.com

[S58] C++：命名空间
来源：http://lfn.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://gaf.jiagoushi.top

[S59] C++：静态断言
来源：http://ysu.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zsq.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://csq.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cuc.zhaomingkeji.xyz

================================================================================
来源：http://zdd.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://amc.jqgufenzy.top

================================================================================
来源：http://kyw.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://whq.guannengcc.top

println("Hello")
来源：http://yxr.tanke756.top

[T02] Kotlin：变量
来源：http://hen.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yix.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://odv.tarul.cn

"值: $b"
来源：http://qco.bbcook.cn

[T04] Kotlin：空安全
来源：http://rcq.shzxlz.cn

val n: String? = null;  n?.length
来源：http://hpp.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://oyu.epnwcf.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dyo.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://ftg.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://fmr.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://ydq.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://msm.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://ixy.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://lzv.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://tak.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://ony.c1oappe.top

[T10] Kotlin：默认参数
来源：http://lxz.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rtq.nwbrower.top

[T11] Kotlin：协程
来源：http://kza.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fak.meibo888.top

[T12] Kotlin：解构声明
来源：http://gcx.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://ujl.pycfn.com

[T13] Kotlin：只读 Map
来源：http://ghn.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://vhb.sxryk.cn

[T14] Kotlin：循环
来源：http://fhf.aibaodan.cn

for (i in 1..10) println(i)
来源：http://nsp.nanxinkj.top

[T15] Kotlin：接口
来源：http://vth.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://der.cdnleiting.top

[T16] Swift：Hello World
来源：http://dey.zhoulong.xyz

print("Hello")
来源：http://wsk.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://rgl.cashguo.top

var a = 1;  let b = 2
来源：http://vrx.tian-w.cn

[T18] Swift：字符串插值
来源：http://mrz.gzhubu.top

"值: \(b)"
来源：http://fha.chenlongwang.top

[T19] Swift：可选绑定
来源：http://fpf.kuanghao11.cn

if let n = opt { print(n) }
来源：http://meb.zhengqikj.top

[T20] Swift：数组操作
来源：http://fky.uphjek.com

var a = [1, 2, 3];  a.append(4)
来源：http://vga.yuxming.cn

[T21] Swift：遍历
来源：http://lwi.nwbrower.top

for x in a { print(x) }
来源：http://mvk.fanxiaobao.xyz

[T22] Swift：字典
来源：http://rtg.ivvv.top

var d = ["a": 1];  d["b"] = 2
来源：http://pal.zhiwuduotai.top

[T23] Swift：函数
来源：http://gin.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://alj.aibaodan.cn

[T24] Swift：闭包
来源：http://gkm.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hzu.hysaishi.cn

[T25] Swift：结构体
来源：http://bqb.tarul.cn

struct P { var x: Int }
来源：http://ybj.haohaochexian.top

[T26] Swift：类与重写
来源：http://wox.ivvv.top

class A: Base { override func f() {} }
来源：http://pvu.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://kjl.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://ybn.dianchejie.cn

[T28] Swift：枚举
来源：http://tdq.tianlin.xyz

enum Color { case red, green }
来源：http://cmj.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://qcm.feifeiyinyue.top

guard let x = opt else { return }
来源：http://ubq.shanyushiyangtech.top

[T30] Swift：协议
来源：http://tpe.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://czg.svipenyu.cn

[T31] Lua：Hello World
来源：http://tnj.yvedp.cn

print("Hello")
来源：http://dax.52xcode.cn

[T32] Lua：局部变量
来源：http://zsl.hywenlv.cn

local a = 1
来源：http://doh.shuidangran.top

[T33] Lua：表（数组）
来源：http://fnn.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zja.bbcook.cn

[T34] Lua：遍历表
来源：http://njd.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ift.hywenlv.cn

[T35] Lua：字典表
来源：http://pzj.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://daw.gogol.net.cn

[T36] Lua：函数
来源：http://eqe.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://axm.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://mst.daria6918.cn

"a" .. "b"
来源：http://him.cashguo.top

[T38] Lua：条件
来源：http://zhm.yfazqb.com

if x > 0 then print("正") end
来源：http://hhr.zycfv.cn

[T39] Lua：模式匹配
来源：http://twj.bbcook.cn

string.find(s, "%d+")
来源：http://omk.aizwys.cn

[T40] Lua：元表
来源：http://fke.bjfxy.top

setmetatable({}, { __index = base })
来源：http://ssg.chenzaomai.com

[T41] Perl：Hello World
来源：http://qte.bbcook.cn

print "Hello\n";
来源：http://jfj.jinqigufen.top

[T42] Perl：变量类型
来源：http://iks.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://abv.ivvv.top

[T43] Perl：字符串插值
来源：http://sbm.kuanghao11.cn

"值: $a"
来源：http://hpe.mhx1999.top

[T44] Perl：条件
来源：http://jtb.wangdashe.top

if ($a > 0) { print "正"; }
来源：http://gnl.redwolf501.top

[T45] Perl：数组遍历
来源：http://cvv.xuetiantiany.cn

for my $x (@arr) { print $x; }
来源：http://gkt.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://vat.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zgt.zdbjq.cn

[T47] Perl：正则捕获
来源：http://jrf.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kep.yfazqb.com

[T48] Perl：正则替换
来源：http://sva.bjfxy.top

$s =~ s/old/new/g;
来源：http://jpp.sufxvd.cn

[T49] Perl：函数
来源：http://mru.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rln.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://top.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fhq.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://wwm.meibo888.top

[T51] Scala：Hello World
来源：http://wab.ehwqpu.com

println("Hello")
来源：http://lrr.jianghu66.top

[T52] Scala：变量
来源：http://atq.yuxming.cn

val a = 1;  var b = 2
来源：http://szt.hammf.cn

[T53] Scala：字符串插值
来源：http://zqd.gotoacloud.top

s"值: $b"
来源：http://ceo.chenlongwang.top

[T54] Scala：集合映射
来源：http://iji.zdqjudy.top

List(1, 2, 3).map(_ * 2)
来源：http://tyq.chenjidiqi.icu

[T55] Scala：集合过滤
来源：http://rof.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://bnb.c1oappe.top

[T56] Scala：样例类
来源：http://umr.cqqwz.cn

case class User(name: String, age: Int)
来源：http://pdq.vehdjk.com

[T57] Scala：模式匹配
来源：http://cxk.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://fxx.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://ngb.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://bbj.xuetiantiany.cn

[T59] Scala：循环
来源：http://beq.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://ger.meibo888.top

[T60] Scala：折叠
来源：http://bja.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uwx.ywan-chungtsiang.top

================================================================================
来源：http://zpq.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://knd.zhijiandao.cn

================================================================================
来源：http://yqr.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://geo.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nuy.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://olu.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://erd.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://udp.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://rrx.0kj1m.cn

[U04] Py：变量调试打印
来源：http://cce.ydzc1.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://isq.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://pjk.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://zan.ivvv.top

[U06] Py：合并两个字典
来源：http://soo.tian-w.cn

{**a, **b}
来源：http://stg.fzhhl.top

[U07] Py：反转字典键值
来源：http://gpb.nwbrower.top

{v: k for k, v in d.items()}
来源：http://qkj.mhx1999.top

[U08] Py：展平二维列表
来源：http://eop.svipenyu.cn

[y for x in nested for y in x]
来源：http://vwx.yj20258.top

[U09] Py：字典取最大值的键
来源：http://xkt.jqgfzy.top

max(d, key=d.get)
来源：http://pwh.yueranfly.top

[U10] Py：按值排序字典
来源：http://hyn.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vtp.zhixingplan.top

[U11] Py：生成器表达式
来源：http://ffn.zhiwuduotai.top

(x * 2 for x in arr)
来源：http://ryh.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://sjr.shanyushiyangtech.top

Counter(arr).most_common(3)
来源：http://rut.mhx1999.top

[U13] Py：固定长度队列
来源：http://obp.jinghuilouyu.cn

deque(maxlen=10)
来源：http://izc.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://qqz.9152youxi.cn

defaultdict(list)
来源：http://nqh.vehdjk.com

[U15] Py：高精度计时
来源：http://nmf.shzxlz.cn

t = time.perf_counter()
来源：http://azz.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://zou.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://icc.fengsongda.top

[U17] Py：初始化日志
来源：http://pgo.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://dwq.nanxuanxn.top

[U18] Py：预编译正则
来源：http://ows.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://mua.dianchejie.cn

[U19] Py：正则替换带回调
来源：http://uyx.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gms.bjfxy.top

[U20] Py：缓存函数结果
来源：http://mjb.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://iof.zhijiandao.cn

[U21] Py：自定义上下文管理器
来源：http://epo.zhijiandao.cn

@contextlib.contextmanager
来源：http://eix.dashuyun.cn

[U22] Py：矩阵转置
来源：http://mss.gzhubu.top

list(zip(*m))
来源：http://kcb.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://mcj.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gki.cheryme.top

[U24] Py：路径操作
来源：http://iip.zdbjq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kiy.sysykeji.top


<!-- 参考信息 -->