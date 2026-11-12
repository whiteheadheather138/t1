代发 wailian999

S. C / C++ 专题
来源：http://rzf.chenzaomai.com

================================================================================
来源：http://gtm.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://dsv.ydjk.org.cn

#include <stdio.h>
来源：http://pey.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pui.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://oko.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://ish.fzhhl.top

[S03] C：读入整数
来源：http://czf.yj20258888.top

int x; scanf("%d", &x);
来源：http://wcb.xylfe.cn

[S04] C：字符串复制
来源：http://tsn.feifeiyinyue.top

char dst[32]; strcpy(dst, "hi");
来源：http://ckw.dashuyun.cn

[S05] C：字符串长度
来源：http://pch.hongshengwenyu.top

strlen(s)
来源：http://pqo.ydjk.org.cn

[S06] C：字符串比较
来源：http://bkd.fengsongda.top

strcmp(a, b) == 0
来源：http://zbt.epnwcf.com

[S07] C：数组遍历求和
来源：http://lxm.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://got.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://kar.fehbvm.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bsk.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://bfe.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pqb.sjlbkw.cn

[S10] C：指针与解引用
来源：http://nbl.cashguo.top

int *p = &a;  *p = 5;
来源：http://gmh.hnxiangtu.top

[S11] C：逐行读文件
来源：http://shq.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://djm.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://asn.pengpengdd.cyou

fclose(f);
来源：http://qin.zhixingplan.top

[S12] C：写文件
来源：http://hql.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mlw.guannengcc.top

[S13] C：宏定义
来源：http://stm.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nze.sjlbkw.cn

[S14] C：枚举
来源：http://hud.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://glf.52xcode.cn

[S15] C：类型转换
来源：http://gvs.xingfuxueyuan.xyz

(double) a / b
来源：http://xna.fzhhl.top

[S16] C：位操作置位
来源：http://vyv.shangyingyoupin.top

x |= (1 << 3);
来源：http://oir.yonumen.top

[S17] C：安全拼接字符串
来源：http://vor.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://upz.chenzaomai.com

[S18] C：命令行参数
来源：http://dvl.yvedp.cn

int main(int argc, char **argv)
来源：http://xig.fehbvm.com

[S19] C：快速排序
来源：http://rka.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://icy.zdbjq.cn

[S20] C：二分查找
来源：http://bzo.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wbv.havefunace.top

[S21] C：字符类别判断
来源：http://sjk.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://piq.quarkkingdee.top

[S22] C：字符串转数字
来源：http://sca.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://ljg.cdnleiting.top

[S23] C：随机数
来源：http://qck.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ght.9152youxi.cn

[S24] C：获取本地时间
来源：http://mgu.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uvq.snrcjt.cn

[S25] C：内存拷贝
来源：http://dqi.jyoumei.cn

memcpy(dst, src, n);
来源：http://njg.yangfankeji.com

[S26] C：内存清零
来源：http://wpb.hnqzz.top

memset(a, 0, sizeof a);
来源：http://axd.yfazqb.com

[S27] C：定义常量
来源：http://ezf.iojbl.cn

const double PI = 3.14159;
来源：http://phi.gogol.net.cn

[S28] C：静态变量
来源：http://uuk.0kj1m.cn

static int counter = 0;
来源：http://spj.yuanzhike.top

[S29] C：变参函数
来源：http://nbj.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tuo.snrcjt.cn

[S30] C：头文件保护
来源：http://dlh.yj202588.top

#ifndef X_H
来源：http://tsl.hnxiangtu.top

#define X_H
来源：http://yuh.yuxming.cn

#endif
来源：http://rsu.ehwqpu.com

[S31] C++：Hello World
来源：http://gsw.zdbjq.cn

#include <iostream>
来源：http://cbh.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://qob.vqdsnc.cn

[S32] C++：字符串
来源：http://kxw.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://nuy.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://tcz.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fnl.dianchejie.cn

[S34] C++：遍历 vector
来源：http://gll.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://qzp.hywenlv.cn

[S35] C++：map
来源：http://juh.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uds.yanxiufei.cn

[S36] C++：unordered_map
来源：http://amc.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vip.chenzaomai.com

[S37] C++：set
来源：http://esx.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bkz.yj202588.top

[S38] C++：排序
来源：http://waw.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://rcm.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://dam.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cwc.zhongyouzk.top

[S40] C++：查找元素
来源：http://vrl.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sqv.svipenyu.cn

[S41] C++：类与构造函数
来源：http://dfh.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ive.fktsv.cn

[S42] C++：继承与虚函数
来源：http://orq.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://iyg.zdbjq.cn

[S43] C++：智能指针
来源：http://zqy.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://vrl.yj202588.top

[S44] C++：引用传参
来源：http://fom.iojbl.cn

void inc(int &x) { ++x; }
来源：http://wgv.sufxvd.cn

[S45] C++：lambda
来源：http://pxt.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://lcb.daxiang520.top

[S46] C++：函数模板
来源：http://hpg.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wyr.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://hvy.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zss.gzhubu.top

[S48] C++：逐行读文件
来源：http://xzj.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://uli.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://ieu.zhijiandao.cn

[S49] C++：写文件
来源：http://gae.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://emz.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://pru.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xmp.ctjpmb.com

[S51] C++：显式类型转换
来源：http://eya.jinqigufen.top

static_cast<double>(a) / b
来源：http://ius.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://wgk.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://qkn.yongpay.top

[S53] C++：移动语义
来源：http://fqw.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://ogb.vehdjk.com

[S54] C++：异常处理
来源：http://aes.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pjq.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://gkn.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://dfo.jinqigfzy.top

[S56] C++：optional
来源：http://ovs.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jds.hnxiangtu.top

[S57] C++：编译期常量
来源：http://rgi.iojbl.cn

constexpr int N = 10;
来源：http://rvk.wangdashe.top

[S58] C++：命名空间
来源：http://tic.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://ehl.316326.xyz

[S59] C++：静态断言
来源：http://mnj.haohaochexian.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rwm.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://qgx.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ubh.xingfuxueyuan.xyz

================================================================================
来源：http://xmo.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://agx.sufxvd.cn

================================================================================
来源：http://mox.tanke756.top

[T01] Kotlin：Hello World
来源：http://kpb.fzhhl.top

println("Hello")
来源：http://hyi.shanyushiyangkeji.top

[T02] Kotlin：变量
来源：http://uyp.yvedp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vte.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://yun.svipenyu.cn

"值: $b"
来源：http://fvs.zdqjudy.top

[T04] Kotlin：空安全
来源：http://wxc.zdbjq.cn

val n: String? = null;  n?.length
来源：http://wdc.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://lpe.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mvl.ivvv.top

[T06] Kotlin：集合映射
来源：http://zho.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jwf.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://wxy.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://puo.hcnkem.com

[T08] Kotlin：数据类
来源：http://hrj.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://kzj.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://lod.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://gzw.hcnkem.com

[T10] Kotlin：默认参数
来源：http://czv.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qfs.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://bgv.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sbx.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://npd.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://srw.yongpay.top

[T13] Kotlin：只读 Map
来源：http://kpj.nanxinkj.top

val m = mapOf("a" to 1)
来源：http://ykh.ctjpmb.com

[T14] Kotlin：循环
来源：http://sxa.snrcjt.cn

for (i in 1..10) println(i)
来源：http://cna.cheryme.top

[T15] Kotlin：接口
来源：http://azl.fehbvm.com

interface Shape { fun area(): Double }
来源：http://zqa.tanke756.top

[T16] Swift：Hello World
来源：http://xwo.cheryme.top

print("Hello")
来源：http://mtf.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://xxv.yuanzhike.top

var a = 1;  let b = 2
来源：http://cxk.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://ylb.kuanghao11.cn

"值: \(b)"
来源：http://hkg.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://xxh.cheryme.top

if let n = opt { print(n) }
来源：http://hpl.smart0.xyz

[T20] Swift：数组操作
来源：http://stc.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://rmr.zhengqikj.top

[T21] Swift：遍历
来源：http://xfu.yongpay.top

for x in a { print(x) }
来源：http://aap.cdnleiting.top

[T22] Swift：字典
来源：http://txw.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://wpt.nanxinkj.top

[T23] Swift：函数
来源：http://cdu.zhoulong.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bod.shangyingyoupin.top

[T24] Swift：闭包
来源：http://bxa.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lrh.316326.xyz

[T25] Swift：结构体
来源：http://eza.xuanzx.com

struct P { var x: Int }
来源：http://exs.hongshengwenyu.top

[T26] Swift：类与重写
来源：http://hlm.chenlongwang.top

class A: Base { override func f() {} }
来源：http://nmj.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://mzo.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://poq.hnxiangtu.top

[T28] Swift：枚举
来源：http://rqg.fktsv.cn

enum Color { case red, green }
来源：http://elt.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://gxh.ydzc1.top

guard let x = opt else { return }
来源：http://lhg.snrcjt.cn

[T30] Swift：协议
来源：http://ser.ivvv.top

protocol Shape { func area() -> Double }
来源：http://kjt.ydjk.org.cn

[T31] Lua：Hello World
来源：http://lib.xinyue.icu

print("Hello")
来源：http://umz.guannengcc.top

[T32] Lua：局部变量
来源：http://tbh.haohaochexian.top

local a = 1
来源：http://jce.shangyingyoupin.top

[T33] Lua：表（数组）
来源：http://nqu.zycfv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xtx.cqqwz.cn

[T34] Lua：遍历表
来源：http://pjo.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kjq.hfpthk.cn

[T35] Lua：字典表
来源：http://snq.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://num.uphjek.com

[T36] Lua：函数
来源：http://ace.fengsongda.top

function add(a, b) return a + b end
来源：http://bnj.wangdashe.top

[T37] Lua：字符串拼接
来源：http://lwx.jqgufenzy.top

"a" .. "b"
来源：http://lmy.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://yjg.ybcxt.top

if x > 0 then print("正") end
来源：http://bcs.jqgfzy.top

[T39] Lua：模式匹配
来源：http://fxg.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://iie.gzhubu.top

[T40] Lua：元表
来源：http://joo.daxiang520.top

setmetatable({}, { __index = base })
来源：http://btu.jlsjyb.cn

[T41] Perl：Hello World
来源：http://wdj.pycfn.com

print "Hello\n";
来源：http://ggr.0kj1m.cn

[T42] Perl：变量类型
来源：http://ojf.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oyc.dashuyun.cn

[T43] Perl：字符串插值
来源：http://bea.yangfankeji.com

"值: $a"
来源：http://hrd.yj20258.top

[T44] Perl：条件
来源：http://ryd.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://vyz.ehwqpu.com

[T45] Perl：数组遍历
来源：http://mpl.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://ruc.ivvv.top

[T46] Perl：哈希操作
来源：http://ces.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vag.ivvv.top

[T47] Perl：正则捕获
来源：http://hpi.cashguo.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tgh.yonumen.top

[T48] Perl：正则替换
来源：http://kug.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://fux.yonumen.top

[T49] Perl：函数
来源：http://zme.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sia.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://ftf.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ldo.jianghu66.top

while (my $line = <$fh>) { print $line; }
来源：http://vxk.fktsv.cn

[T51] Scala：Hello World
来源：http://zla.havefunace.top

println("Hello")
来源：http://dyn.daxiang520.top

[T52] Scala：变量
来源：http://mfl.ydzc1.top

val a = 1;  var b = 2
来源：http://hih.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://cvm.fzhhl.top

s"值: $b"
来源：http://mhc.vqdsnc.cn

[T54] Scala：集合映射
来源：http://isg.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://fzb.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://mta.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://rqd.haohaochexian.top

[T56] Scala：样例类
来源：http://knd.316326.xyz

case class User(name: String, age: Int)
来源：http://ivg.zhixingplan.top

[T57] Scala：模式匹配
来源：http://vyl.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://upc.yangfankeji.com

[T58] Scala：函数定义
来源：http://jsk.vqdsnc.cn

def add(a: Int, b: Int): Int = a + b
来源：http://egq.ybcxt.top

[T59] Scala：循环
来源：http://fkd.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://ssi.birdmap.top

[T60] Scala：折叠
来源：http://pkf.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wfa.yongpay.top

================================================================================
来源：http://jlk.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://puy.jinqigfzy.top

================================================================================
来源：http://eic.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://zlz.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qtk.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://huk.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fii.zdbjq.cn

[U03] Py：加载 .env 配置
来源：http://xkk.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://che.yueranfly.top

[U04] Py：变量调试打印
来源：http://frg.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yzc.epnwcf.com

[U05] Py：列表去重且保序
来源：http://wsg.andypj.xyz

list(dict.fromkeys(arr))
来源：http://czq.ctjpmb.com

[U06] Py：合并两个字典
来源：http://wwj.bjfxy.top

{**a, **b}
来源：http://mvf.hnqzz.top

[U07] Py：反转字典键值
来源：http://yqw.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://slq.andypj.xyz

[U08] Py：展平二维列表
来源：http://abf.epnwcf.com

[y for x in nested for y in x]
来源：http://cgn.cqqwz.cn

[U09] Py：字典取最大值的键
来源：http://gui.yanxiufei.cn

max(d, key=d.get)
来源：http://icz.meibo888.top

[U10] Py：按值排序字典
来源：http://fmy.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aww.shuidangran.top

[U11] Py：生成器表达式
来源：http://nzb.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://qkz.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://sej.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://oaa.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://rgv.ehwqpu.com

deque(maxlen=10)
来源：http://nfh.xinyue.icu

[U14] Py：分组收集到列表
来源：http://teh.tianlin.xyz

defaultdict(list)
来源：http://krw.ydjk.org.cn

[U15] Py：高精度计时
来源：http://ipa.hcnkem.com

t = time.perf_counter()
来源：http://uew.sysykeji.top

[U16] Py：命令行参数解析
来源：http://ptq.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jja.uphjek.com

[U17] Py：初始化日志
来源：http://kfy.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://ezj.smart0.xyz

[U18] Py：预编译正则
来源：http://aml.redwolf501.top

pat = re.compile(r"\d+")
来源：http://xrr.316326.xyz

[U19] Py：正则替换带回调
来源：http://kik.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rfw.ivvv.top

[U20] Py：缓存函数结果
来源：http://ndq.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://rlb.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://fzo.nwbrower.top

@contextlib.contextmanager
来源：http://hen.ydjk.org.cn

[U22] Py：矩阵转置
来源：http://kcq.c1oappe.top

list(zip(*m))
来源：http://ufh.hesvh.cn


<!-- 参考信息 -->