代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hcx.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://sbu.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://gvl.sysykeji.top

[S03] C：读入整数
来源：http://msx.9152youxi.cn

int x; scanf("%d", &x);
来源：http://jfj.hammf.cn

[S04] C：字符串复制
来源：http://lhh.gzhubu.top

char dst[32]; strcpy(dst, "hi");
来源：http://dhh.yj202588.top

[S05] C：字符串长度
来源：http://gal.shangyingyoupin.top

strlen(s)
来源：http://uoy.zhixingplan.top

[S06] C：字符串比较
来源：http://asv.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://thh.xylfe.cn

[S07] C：数组遍历求和
来源：http://hja.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://klr.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://sge.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lct.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://zuz.tian-w.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uey.aizwys.cn

[S10] C：指针与解引用
来源：http://fcu.hammf.cn

int *p = &a;  *p = 5;
来源：http://ofe.cqqwz.cn

[S11] C：逐行读文件
来源：http://lqt.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://crh.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://mro.xinyue.icu

fclose(f);
来源：http://hgn.wangdashe.top

[S12] C：写文件
来源：http://vfk.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hfn.fanxiaobao.xyz

[S13] C：宏定义
来源：http://xsy.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bdx.vehdjk.com

[S14] C：枚举
来源：http://phn.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://zku.snrcjt.cn

[S15] C：类型转换
来源：http://xlk.yongpay.top

(double) a / b
来源：http://rzm.xuanzx.com

[S16] C：位操作置位
来源：http://wlo.cdnleiting.top

x |= (1 << 3);
来源：http://afj.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://bdj.sxryk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kun.hywenlv.cn

[S18] C：命令行参数
来源：http://izh.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://zpy.shangyingyoupin.top

[S19] C：快速排序
来源：http://vhw.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ljz.hongshengwenyu.top

[S20] C：二分查找
来源：http://gjt.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sih.zhongyouzk.top

[S21] C：字符类别判断
来源：http://bhu.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://avb.fzhhl.top

[S22] C：字符串转数字
来源：http://olt.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yfc.feifeiyinyue.top

[S23] C：随机数
来源：http://qrc.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gye.ydzc1.top

[S24] C：获取本地时间
来源：http://ocn.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xat.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://uyy.chenzaomai.com

memcpy(dst, src, n);
来源：http://vlr.jyoumei.cn

[S26] C：内存清零
来源：http://psc.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://xha.chenjidiqi.icu

[S27] C：定义常量
来源：http://hud.yj202588.top

const double PI = 3.14159;
来源：http://wrs.hesvh.cn

[S28] C：静态变量
来源：http://koe.jyoumei.cn

static int counter = 0;
来源：http://wfq.cucudq.cn

[S29] C：变参函数
来源：http://fsq.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hzt.chenlongwang.top

[S30] C：头文件保护
来源：http://sbd.zdbjq.cn

#ifndef X_H
来源：http://lkf.fanxiaobao.xyz

#define X_H
来源：http://cci.iojbl.cn

#endif
来源：http://zno.yuanzhike.top

[S31] C++：Hello World
来源：http://znw.hammf.cn

#include <iostream>
来源：http://wwu.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://eos.meibo888.top

[S32] C++：字符串
来源：http://nwr.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://amm.dashuyun.cn

[S33] C++：vector 增删
来源：http://vcn.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wof.cheryme.top

[S34] C++：遍历 vector
来源：http://rgy.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://kqy.jinqigfzy.top

[S35] C++：map
来源：http://utc.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lzn.haohaochexian.top

[S36] C++：unordered_map
来源：http://bno.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jwz.ppjwa.cn

[S37] C++：set
来源：http://ehx.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cdj.yfazqb.com

[S38] C++：排序
来源：http://bfv.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://enw.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://sdf.tarul.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ccf.jinqigfzy.top

[S40] C++：查找元素
来源：http://nhv.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fob.ppjwa.cn

[S41] C++：类与构造函数
来源：http://xst.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yzp.cheryme.top

[S42] C++：继承与虚函数
来源：http://hsr.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://oea.nwbrower.top

[S43] C++：智能指针
来源：http://mdp.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://ydt.gotoacloud.top

[S44] C++：引用传参
来源：http://ska.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://dew.jinqigfzy.top

[S45] C++：lambda
来源：http://nbr.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://rbq.aizwys.cn

[S46] C++：函数模板
来源：http://cmh.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://adv.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://jph.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uoj.yfazqb.com

[S48] C++：逐行读文件
来源：http://qlu.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://jii.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://mvz.hongshengwenyu.top

[S49] C++：写文件
来源：http://bgo.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sml.wangdashe.top

[S50] C++：格式化数字
来源：http://klo.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pyc.sxryk.cn

[S51] C++：显式类型转换
来源：http://hep.dashuyun.cn

static_cast<double>(a) / b
来源：http://ilb.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://pqt.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://uty.52xcode.cn

[S53] C++：移动语义
来源：http://qdh.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://org.andypj.xyz

[S54] C++：异常处理
来源：http://vdx.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yez.tianlin.xyz

[S55] C++：结构化绑定
来源：http://awz.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://vdq.xuanzx.com

[S56] C++：optional
来源：http://glr.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ync.uphjek.com

[S57] C++：编译期常量
来源：http://zwj.shuidangran.top

constexpr int N = 10;
来源：http://toz.zhixingplan.top

[S58] C++：命名空间
来源：http://gjb.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://fni.zhoulong.xyz

[S59] C++：静态断言
来源：http://xdv.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://voa.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://gyp.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hxc.xinyue.icu

================================================================================
来源：http://oij.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mse.tianlin.xyz

================================================================================
来源：http://mme.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://emt.ctjpmb.com

println("Hello")
来源：http://aae.yangfankeji.com

[T02] Kotlin：变量
来源：http://asi.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nxt.aibaodan.cn

[T03] Kotlin：字符串模板
来源：http://yhm.vqdsnc.cn

"值: $b"
来源：http://rrv.zdbjq.cn

[T04] Kotlin：空安全
来源：http://nov.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://jow.sweek.top

[T05] Kotlin：when 表达式
来源：http://hne.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mkc.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://xhn.havefunace.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dds.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://oqu.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kfc.fehbvm.com

[T08] Kotlin：数据类
来源：http://ctz.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://qlg.havefunace.top

[T09] Kotlin：扩展函数
来源：http://ypb.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://ezg.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://xge.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eks.hnxiangtu.top

[T11] Kotlin：协程
来源：http://rti.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://czh.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://kua.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://sll.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://yyh.shuidangran.top

val m = mapOf("a" to 1)
来源：http://tus.zycfv.cn

[T14] Kotlin：循环
来源：http://tql.redwolf501.top

for (i in 1..10) println(i)
来源：http://mkl.yj202588.top

[T15] Kotlin：接口
来源：http://yti.zycfv.cn

interface Shape { fun area(): Double }
来源：http://gtm.0kj1m.cn

[T16] Swift：Hello World
来源：http://sna.cheryme.top

print("Hello")
来源：http://mam.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://khq.guowangkeji.top

var a = 1;  let b = 2
来源：http://jsi.yangfankeji.com

[T18] Swift：字符串插值
来源：http://bum.tianlin.xyz

"值: \(b)"
来源：http://juy.shzxlz.cn

[T19] Swift：可选绑定
来源：http://bsa.yongpay.top

if let n = opt { print(n) }
来源：http://nlk.ydzc1.top

[T20] Swift：数组操作
来源：http://hxr.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://hlp.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://sng.kuanghao11.cn

for x in a { print(x) }
来源：http://ole.jqgufenzy.top

[T22] Swift：字典
来源：http://yds.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://opi.yvedp.cn

[T23] Swift：函数
来源：http://hka.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://amd.gotoacloud.top

[T24] Swift：闭包
来源：http://qko.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://ona.tianlin.xyz

[T25] Swift：结构体
来源：http://ujk.zycfv.cn

struct P { var x: Int }
来源：http://dby.nanxuanxn.top

[T26] Swift：类与重写
来源：http://hkc.zdbjq.cn

class A: Base { override func f() {} }
来源：http://xsz.birdmap.top

[T27] Swift：错误处理
来源：http://dfu.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://hda.ydzc1.top

[T28] Swift：枚举
来源：http://cim.meibo888.top

enum Color { case red, green }
来源：http://ssp.uphjek.com

[T29] Swift：guard 提前返回
来源：http://sgh.hesvh.cn

guard let x = opt else { return }
来源：http://pry.epnwcf.com

[T30] Swift：协议
来源：http://ptb.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://lsu.jqgfzy.top

[T31] Lua：Hello World
来源：http://usx.kuanghao11.cn

print("Hello")
来源：http://vll.cheryme.top

[T32] Lua：局部变量
来源：http://ilb.tanke756.top

local a = 1
来源：http://klz.vehdjk.com

[T33] Lua：表（数组）
来源：http://lwo.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://wrb.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://hlg.sufxvd.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uqj.52xcode.cn

[T35] Lua：字典表
来源：http://tlr.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://jnj.xziqi.cn

[T36] Lua：函数
来源：http://hzv.shuidangran.top

function add(a, b) return a + b end
来源：http://fgf.meibo888.top

[T37] Lua：字符串拼接
来源：http://vcl.jyoumei.cn

"a" .. "b"
来源：http://qgb.zycfv.cn

[T38] Lua：条件
来源：http://cta.tanke756.top

if x > 0 then print("正") end
来源：http://plz.yuxming.cn

[T39] Lua：模式匹配
来源：http://brs.haohaochexian.top

string.find(s, "%d+")
来源：http://hry.sjlbkw.cn

[T40] Lua：元表
来源：http://bwe.redwolf501.top

setmetatable({}, { __index = base })
来源：http://ciw.yonumen.top

[T41] Perl：Hello World
来源：http://aeo.fehbvm.com

print "Hello\n";
来源：http://ubf.yuanzhike.top

[T42] Perl：变量类型
来源：http://ayj.svipenyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aym.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://bww.gzhubu.top

"值: $a"
来源：http://niw.gotoacloud.top

[T44] Perl：条件
来源：http://pbj.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://hav.haohaochexian.top

[T45] Perl：数组遍历
来源：http://htu.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://lqc.jiagoushi.top

[T46] Perl：哈希操作
来源：http://tcn.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kts.haohaochexian.top

[T47] Perl：正则捕获
来源：http://sah.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://erl.gotoacloud.top

[T48] Perl：正则替换
来源：http://gsp.andypj.xyz

$s =~ s/old/new/g;
来源：http://gga.daxiang520.top

[T49] Perl：函数
来源：http://wpc.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zds.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://fie.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pju.zycfv.cn

while (my $line = <$fh>) { print $line; }
来源：http://ubx.fehbvm.com

[T51] Scala：Hello World
来源：http://mij.zhixingplan.top

println("Hello")
来源：http://ehd.dianchejie.cn

[T52] Scala：变量
来源：http://qyd.redwolf501.top

val a = 1;  var b = 2
来源：http://nhr.haohaochexian.top

[T53] Scala：字符串插值
来源：http://xto.fzhhl.top

s"值: $b"
来源：http://bfy.yuanzhike.top

[T54] Scala：集合映射
来源：http://cno.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://dco.316326.xyz

[T55] Scala：集合过滤
来源：http://hyv.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wsc.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://jwm.hnqzz.top

case class User(name: String, age: Int)
来源：http://bwt.52xcode.cn

[T57] Scala：模式匹配
来源：http://tpl.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fld.redwolf501.top

[T58] Scala：函数定义
来源：http://had.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://ojx.hesvh.cn

[T59] Scala：循环
来源：http://nwt.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://qzz.bjfxy.top

[T60] Scala：折叠
来源：http://qxw.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dzs.bjfxy.top

================================================================================
来源：http://grb.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://orh.sweek.top

================================================================================
来源：http://jtm.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://ixp.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://ujs.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://hdp.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gkm.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://ltj.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://boj.daria6918.cn

[U04] Py：变量调试打印
来源：http://alh.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ovo.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://nvq.hongshengwenyu.top

list(dict.fromkeys(arr))
来源：http://mge.ehwqpu.com

[U06] Py：合并两个字典
来源：http://qgb.jyoumei.cn

{**a, **b}
来源：http://tlc.pycfn.com

[U07] Py：反转字典键值
来源：http://dwg.hfpthk.cn

{v: k for k, v in d.items()}
来源：http://fzf.zhixingplan.top

[U08] Py：展平二维列表
来源：http://udm.jinqigfzy.top

[y for x in nested for y in x]
来源：http://fhy.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://qtu.xziqi.cn

max(d, key=d.get)
来源：http://klx.nanxinkj.top

[U10] Py：按值排序字典
来源：http://fmh.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qst.yueranfly.top

[U11] Py：生成器表达式
来源：http://kvs.feifeiyinyue.top

(x * 2 for x in arr)
来源：http://hlq.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kcc.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://ajz.0kj1m.cn

[U13] Py：固定长度队列
来源：http://pzk.fanxiaobao.xyz

deque(maxlen=10)
来源：http://foz.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://hir.zhaomingkeji.xyz

defaultdict(list)
来源：http://lak.jinqigfzy.top

[U15] Py：高精度计时
来源：http://xyg.zhijiandao.cn

t = time.perf_counter()
来源：http://uda.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://knt.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mah.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://jpo.xziqi.cn

logging.basicConfig(level=logging.INFO)
来源：http://unr.hnxiangtu.top

[U18] Py：预编译正则
来源：http://nzy.zhaomingkeji.xyz

pat = re.compile(r"\d+")
来源：http://dkh.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://wsj.fktsv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qev.wangdashe.top

[U20] Py：缓存函数结果
来源：http://njg.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://gyj.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://eva.hammf.cn

@contextlib.contextmanager
来源：http://pag.cheryme.top

[U22] Py：矩阵转置
来源：http://ipj.52xcode.cn

list(zip(*m))
来源：http://oln.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://idx.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ota.birdmap.top

[U24] Py：路径操作
来源：http://ves.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yxt.bbcook.cn


<!-- 参考信息 -->