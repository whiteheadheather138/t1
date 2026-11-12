代发 wailian999

S. C / C++ 专题
来源：http://fhm.redwolf501.top

================================================================================
来源：http://inn.nanxuanxn.top

[S01] C：Hello World
来源：http://lcy.cheryme.top

#include <stdio.h>
来源：http://izo.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hrk.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://fdj.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://rxb.sweek.top

[S03] C：读入整数
来源：http://tbs.jinqigufen.top

int x; scanf("%d", &x);
来源：http://xrd.daria6918.cn

[S04] C：字符串复制
来源：http://ddl.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ril.meibo888.top

[S05] C：字符串长度
来源：http://zhu.hammf.cn

strlen(s)
来源：http://hqq.havefunace.top

[S06] C：字符串比较
来源：http://tvv.bbcook.cn

strcmp(a, b) == 0
来源：http://ufz.cheryme.top

[S07] C：数组遍历求和
来源：http://pve.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nwu.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://bej.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://afn.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://bsj.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cin.gaohongyu789.top

[S10] C：指针与解引用
来源：http://cxo.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://gat.quarkkingdee.top

[S11] C：逐行读文件
来源：http://lbz.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://kiq.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://elu.zhengqikj.top

fclose(f);
来源：http://amj.nwbrower.top

[S12] C：写文件
来源：http://fxh.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fbb.52xcode.cn

[S13] C：宏定义
来源：http://ujm.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ehj.gzhubu.top

[S14] C：枚举
来源：http://olq.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://qwy.dashuyun.cn

[S15] C：类型转换
来源：http://llo.vehdjk.com

(double) a / b
来源：http://pee.jinqigufen.top

[S16] C：位操作置位
来源：http://fjm.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://dgn.fzhhl.top

[S17] C：安全拼接字符串
来源：http://pmk.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jqa.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://bvx.uphjek.com

int main(int argc, char **argv)
来源：http://czl.hesvh.cn

[S19] C：快速排序
来源：http://gmp.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://hma.jinyuanbaomall.cn

[S20] C：二分查找
来源：http://ymo.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sgw.hysaishi.cn

[S21] C：字符类别判断
来源：http://kbq.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://auu.nwbrower.top

[S22] C：字符串转数字
来源：http://ldz.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ydn.andypj.xyz

[S23] C：随机数
来源：http://roh.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eqe.xinyue.icu

[S24] C：获取本地时间
来源：http://qtt.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hdz.xuanzx.com

[S25] C：内存拷贝
来源：http://iok.quarkkingdee.top

memcpy(dst, src, n);
来源：http://nyc.aizwys.cn

[S26] C：内存清零
来源：http://cai.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://xxd.ehwqpu.com

[S27] C：定义常量
来源：http://ysp.yfazqb.com

const double PI = 3.14159;
来源：http://pku.gotoacloud.top

[S28] C：静态变量
来源：http://xqv.c1oappe.top

static int counter = 0;
来源：http://cku.tarul.cn

[S29] C：变参函数
来源：http://cwy.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://koq.yfazqb.com

[S30] C：头文件保护
来源：http://ojk.sufxvd.cn

#ifndef X_H
来源：http://ctx.fktsv.cn

#define X_H
来源：http://zwl.epnwcf.com

#endif
来源：http://bks.hysaishi.cn

[S31] C++：Hello World
来源：http://wyt.xuanzx.com

#include <iostream>
来源：http://dfa.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://hpn.shuidangran.top

[S32] C++：字符串
来源：http://bub.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://uym.nanxinkj.top

[S33] C++：vector 增删
来源：http://iiz.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jrp.havefunace.top

[S34] C++：遍历 vector
来源：http://keb.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://xlj.aibaodan.cn

[S35] C++：map
来源：http://bnn.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jgz.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://hpo.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yun.daria6918.cn

[S37] C++：set
来源：http://rzn.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oky.fehbvm.com

[S38] C++：排序
来源：http://irv.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://wjv.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://kiu.9152youxi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wam.chenlongwang.top

[S40] C++：查找元素
来源：http://rwc.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bbk.hnqzz.top

[S41] C++：类与构造函数
来源：http://sae.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xlx.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://yzn.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://hqo.zhoulong.xyz

[S43] C++：智能指针
来源：http://voi.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://dcz.kuanghao11.cn

[S44] C++：引用传参
来源：http://zzx.xuanzx.com

void inc(int &x) { ++x; }
来源：http://pkw.fktsv.cn

[S45] C++：lambda
来源：http://jmy.jinqigfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://yms.pycfn.com

[S46] C++：函数模板
来源：http://klu.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mvw.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://uiu.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uoi.9152youxi.cn

[S48] C++：逐行读文件
来源：http://mxq.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hhz.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://bls.sysykeji.top

[S49] C++：写文件
来源：http://myl.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lws.ivvv.top

[S50] C++：格式化数字
来源：http://wtq.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dmw.sweek.top

[S51] C++：显式类型转换
来源：http://uyf.svipenyu.cn

static_cast<double>(a) / b
来源：http://ksu.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://epg.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://gcq.jqgfzy.top

[S53] C++：移动语义
来源：http://cpl.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://ffu.ivvv.top

[S54] C++：异常处理
来源：http://xvq.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dxr.epnwcf.com

[S55] C++：结构化绑定
来源：http://zhq.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ayd.sufxvd.cn

[S56] C++：optional
来源：http://wjb.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qeq.uphjek.com

[S57] C++：编译期常量
来源：http://gwf.zycfv.cn

constexpr int N = 10;
来源：http://auq.quarkkingdee.top

[S58] C++：命名空间
来源：http://mkc.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://pst.tian-w.cn

[S59] C++：静态断言
来源：http://olj.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ejn.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://fmq.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qpr.dashuyun.cn

================================================================================
来源：http://pnf.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xbc.vehdjk.com

================================================================================
来源：http://emx.bbcook.cn

[T01] Kotlin：Hello World
来源：http://mst.ydzc1.top

println("Hello")
来源：http://wmw.sysykeji.top

[T02] Kotlin：变量
来源：http://qhd.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kae.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://usl.sxryk.cn

"值: $b"
来源：http://ywg.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://zot.jyoumei.cn

val n: String? = null;  n?.length
来源：http://iga.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://oyh.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kuw.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://xwa.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cib.shanyushiyangtech.top

[T07] Kotlin：集合过滤
来源：http://dkg.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://llv.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://exk.uphjek.com

data class User(val name: String, val age: Int)
来源：http://fdo.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://ing.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://oau.zdbjq.cn

[T10] Kotlin：默认参数
来源：http://tbi.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://osa.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://lbb.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rye.andypj.xyz

[T12] Kotlin：解构声明
来源：http://hro.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://ojt.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://zru.tarul.cn

val m = mapOf("a" to 1)
来源：http://rmu.haohaochexian.top

[T14] Kotlin：循环
来源：http://ecm.andypj.xyz

for (i in 1..10) println(i)
来源：http://zyj.bjfxy.top

[T15] Kotlin：接口
来源：http://dpb.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://lay.yangfankeji.com

[T16] Swift：Hello World
来源：http://hfy.yonumen.top

print("Hello")
来源：http://sjg.xziqi.cn

[T17] Swift：变量与常量
来源：http://fox.yuxming.cn

var a = 1;  let b = 2
来源：http://ywf.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://iti.chenjidiqi.icu

"值: \(b)"
来源：http://ljb.hesvh.cn

[T19] Swift：可选绑定
来源：http://imd.ydzc1.top

if let n = opt { print(n) }
来源：http://ovk.cqqwz.cn

[T20] Swift：数组操作
来源：http://kko.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zls.ehwqpu.com

[T21] Swift：遍历
来源：http://pep.zdqjudy.top

for x in a { print(x) }
来源：http://rfx.pycfn.com

[T22] Swift：字典
来源：http://qpx.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jmk.yuxming.cn

[T23] Swift：函数
来源：http://kpk.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yiq.fehbvm.com

[T24] Swift：闭包
来源：http://hks.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://rju.yvedp.cn

[T25] Swift：结构体
来源：http://yex.gogol.net.cn

struct P { var x: Int }
来源：http://odv.guannengcc.top

[T26] Swift：类与重写
来源：http://abp.yuanzhike.top

class A: Base { override func f() {} }
来源：http://wlc.52xcode.cn

[T27] Swift：错误处理
来源：http://vza.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://hzq.zdbjq.cn

[T28] Swift：枚举
来源：http://sqr.zhengqikj.top

enum Color { case red, green }
来源：http://akc.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://hvd.zdqjudy.top

guard let x = opt else { return }
来源：http://odv.nanxuanxn.top

[T30] Swift：协议
来源：http://chp.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://xcp.hfpthk.cn

[T31] Lua：Hello World
来源：http://vvv.zhijiandao.cn

print("Hello")
来源：http://duv.tian-w.cn

[T32] Lua：局部变量
来源：http://emw.aibaodan.cn

local a = 1
来源：http://umy.zdqjudy.top

[T33] Lua：表（数组）
来源：http://ryn.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tjd.tarul.cn

[T34] Lua：遍历表
来源：http://hss.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bhp.epnwcf.com

[T35] Lua：字典表
来源：http://twi.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://lvy.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://ytt.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://slw.zycfv.cn

[T37] Lua：字符串拼接
来源：http://qzj.meibo888.top

"a" .. "b"
来源：http://bmy.hongshengwenyu.top

[T38] Lua：条件
来源：http://nqg.uphjek.com

if x > 0 then print("正") end
来源：http://ksp.ybcxt.top

[T39] Lua：模式匹配
来源：http://xqh.xziqi.cn

string.find(s, "%d+")
来源：http://gwy.gaohongyu789.top

[T40] Lua：元表
来源：http://fja.316326.xyz

setmetatable({}, { __index = base })
来源：http://qcc.redwolf501.top

[T41] Perl：Hello World
来源：http://omg.hfpthk.cn

print "Hello\n";
来源：http://tfq.vehdjk.com

[T42] Perl：变量类型
来源：http://yao.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dil.jianghu66.top

[T43] Perl：字符串插值
来源：http://omb.ydzc1.top

"值: $a"
来源：http://jay.guowangkeji.top

[T44] Perl：条件
来源：http://ofe.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://mrw.sufxvd.cn

[T45] Perl：数组遍历
来源：http://qdb.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://hmr.tarul.cn

[T46] Perl：哈希操作
来源：http://zir.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bvr.epnwcf.com

[T47] Perl：正则捕获
来源：http://yvg.zhengqikj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wwr.chenzaomai.com

[T48] Perl：正则替换
来源：http://qva.cdnleiting.top

$s =~ s/old/new/g;
来源：http://pwy.cdnleiting.top

[T49] Perl：函数
来源：http://szb.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jim.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://vti.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://cdk.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://tuy.gotoacloud.top

[T51] Scala：Hello World
来源：http://nrv.jinyuanbaomall.cn

println("Hello")
来源：http://jjs.zdbjq.cn

[T52] Scala：变量
来源：http://fmy.bjfxy.top

val a = 1;  var b = 2
来源：http://bic.svipenyu.cn

[T53] Scala：字符串插值
来源：http://odc.fktsv.cn

s"值: $b"
来源：http://ifq.vehdjk.com

[T54] Scala：集合映射
来源：http://qnj.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://ccz.chenlongwang.top

[T55] Scala：集合过滤
来源：http://jbz.hongshengwenyu.top

List(1, 2, 3).filter(_ > 1)
来源：http://dkb.hammf.cn

[T56] Scala：样例类
来源：http://yzo.fengsongda.top

case class User(name: String, age: Int)
来源：http://ems.ivvv.top

[T57] Scala：模式匹配
来源：http://ufy.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sjz.shuidangran.top

[T58] Scala：函数定义
来源：http://sam.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vor.yj20258888.top

[T59] Scala：循环
来源：http://zdm.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://oti.shuidangran.top

[T60] Scala：折叠
来源：http://jhp.chenjidiqi.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dsq.ehwqpu.com

================================================================================
来源：http://zok.gzhubu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jpv.jinqigufen.top

================================================================================
来源：http://qle.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://ubi.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://erz.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://qox.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xgz.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://czo.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://pcw.aibaodan.cn

[U04] Py：变量调试打印
来源：http://uvo.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://udn.xingfuxueyuan.xyz

[U05] Py：列表去重且保序
来源：http://ndf.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://gjz.epnwcf.com

[U06] Py：合并两个字典
来源：http://who.sysykeji.top

{**a, **b}
来源：http://dnb.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://eda.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://qoi.bbcook.cn

[U08] Py：展平二维列表
来源：http://jkd.shuidangran.top

[y for x in nested for y in x]
来源：http://dja.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://rpf.jiagoushi.top

max(d, key=d.get)
来源：http://mux.daria6918.cn

[U10] Py：按值排序字典
来源：http://mun.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rbb.yuxming.cn

[U11] Py：生成器表达式
来源：http://plr.hfpthk.cn

(x * 2 for x in arr)
来源：http://mkn.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://pct.nanxuanxn.top

Counter(arr).most_common(3)
来源：http://axb.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://sgn.birdmap.top

deque(maxlen=10)
来源：http://tqz.zhaomingkeji.xyz

[U14] Py：分组收集到列表
来源：http://ppw.zhoulong.xyz

defaultdict(list)
来源：http://yuy.chenzaomai.com

[U15] Py：高精度计时
来源：http://scv.jianghu66.top

t = time.perf_counter()
来源：http://oqz.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://agg.nanxuanxn.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cfz.yfazqb.com

[U17] Py：初始化日志
来源：http://mbs.bbcook.cn

logging.basicConfig(level=logging.INFO)
来源：http://pby.316326.xyz

[U18] Py：预编译正则
来源：http://lrw.hcnkem.com

pat = re.compile(r"\d+")
来源：http://nxm.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://lfj.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gbf.shuidangran.top

[U20] Py：缓存函数结果
来源：http://hdj.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://pbh.ivvv.top

[U21] Py：自定义上下文管理器
来源：http://fau.iojbl.cn

@contextlib.contextmanager
来源：http://vii.chenlongwang.top

[U22] Py：矩阵转置
来源：http://cij.zhengqikj.top

list(zip(*m))
来源：http://ful.gogol.net.cn


<!-- 参考信息 -->