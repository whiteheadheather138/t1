代发 wailian999

S. C / C++ 专题
来源：http://wns.svipenyu.cn

================================================================================
来源：http://kdk.hywenlv.cn

[S01] C：Hello World
来源：http://yzl.guowangkeji.top

#include <stdio.h>
来源：http://ugl.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qfd.xylfe.cn

[S02] C：变量与格式化输出
来源：http://yuj.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://rqd.dianchejie.cn

[S03] C：读入整数
来源：http://sop.dianchejie.cn

int x; scanf("%d", &x);
来源：http://nhz.yj20258888.top

[S04] C：字符串复制
来源：http://ooi.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://src.yueranfly.top

[S05] C：字符串长度
来源：http://nzf.svipenyu.cn

strlen(s)
来源：http://srx.zhiwuduotai.top

[S06] C：字符串比较
来源：http://jzd.epnwcf.com

strcmp(a, b) == 0
来源：http://dbc.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://csm.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qam.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://wdk.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jml.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://gai.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gqy.vehdjk.com

[S10] C：指针与解引用
来源：http://clw.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://ymz.nwbrower.top

[S11] C：逐行读文件
来源：http://nib.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://dyi.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://qrn.wangdashe.top

fclose(f);
来源：http://jvt.daxiang520.top

[S12] C：写文件
来源：http://vcn.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tik.yfazqb.com

[S13] C：宏定义
来源：http://iid.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://goi.aibaodan.cn

[S14] C：枚举
来源：http://yjc.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://auu.aizwys.cn

[S15] C：类型转换
来源：http://xds.kuanghao11.cn

(double) a / b
来源：http://wta.hammf.cn

[S16] C：位操作置位
来源：http://nxm.hysaishi.cn

x |= (1 << 3);
来源：http://fmq.sweek.top

[S17] C：安全拼接字符串
来源：http://mjv.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mqf.xinyue.icu

[S18] C：命令行参数
来源：http://jvf.jqgufenzy.top

int main(int argc, char **argv)
来源：http://qix.pycfn.com

[S19] C：快速排序
来源：http://stu.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://bbn.zdqjudy.top

[S20] C：二分查找
来源：http://qss.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://crn.xuanzx.com

[S21] C：字符类别判断
来源：http://kqn.zhengqikj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aml.ppjwa.cn

[S22] C：字符串转数字
来源：http://ugl.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://tgm.zhixingplan.top

[S23] C：随机数
来源：http://xzx.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://hyc.fehbvm.com

[S24] C：获取本地时间
来源：http://bdj.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qvo.wangdashe.top

[S25] C：内存拷贝
来源：http://lum.yj202588.top

memcpy(dst, src, n);
来源：http://iwp.chenjidiqi.icu

[S26] C：内存清零
来源：http://ssj.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://ilp.zdbjq.cn

[S27] C：定义常量
来源：http://xmi.chenzaomai.com

const double PI = 3.14159;
来源：http://yre.zhiwuduotai.top

[S28] C：静态变量
来源：http://roo.hfpthk.cn

static int counter = 0;
来源：http://dqk.iojbl.cn

[S29] C：变参函数
来源：http://xth.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://grq.smart0.xyz

[S30] C：头文件保护
来源：http://nhy.zhoulong.xyz

#ifndef X_H
来源：http://jzn.ywan-chungtsiang.top

#define X_H
来源：http://xyd.zhongyouzk.top

#endif
来源：http://fhn.sxryk.cn

[S31] C++：Hello World
来源：http://rmy.hfpthk.cn

#include <iostream>
来源：http://vhw.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://mss.xuanzx.com

[S32] C++：字符串
来源：http://eii.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://ozn.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://sks.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zkj.ehwqpu.com

[S34] C++：遍历 vector
来源：http://qmq.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://rgh.zhaomingkeji.xyz

[S35] C++：map
来源：http://atb.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ola.epnwcf.com

[S36] C++：unordered_map
来源：http://yrw.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pie.dianchejie.cn

[S37] C++：set
来源：http://knd.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rlb.yongpay.top

[S38] C++：排序
来源：http://rmh.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://ksv.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://oaw.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fpj.gzhubu.top

[S40] C++：查找元素
来源：http://tlm.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lxb.gotoacloud.top

[S41] C++：类与构造函数
来源：http://txs.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gna.wangdashe.top

[S42] C++：继承与虚函数
来源：http://tnr.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://stc.epnwcf.com

[S43] C++：智能指针
来源：http://erm.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://ggj.jinqigfzy.top

[S44] C++：引用传参
来源：http://mst.yvedp.cn

void inc(int &x) { ++x; }
来源：http://pyj.jinqigfzy.top

[S45] C++：lambda
来源：http://kje.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ixu.ydzc1.top

[S46] C++：函数模板
来源：http://esz.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pxo.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://duu.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://akq.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://fyb.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fsp.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://hhi.yfazqb.com

[S49] C++：写文件
来源：http://tzl.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ejz.ehwqpu.com

[S50] C++：格式化数字
来源：http://snq.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rap.tian-w.cn

[S51] C++：显式类型转换
来源：http://fuq.yanxiufei.cn

static_cast<double>(a) / b
来源：http://awe.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://jgy.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://mjf.zycfv.cn

[S53] C++：移动语义
来源：http://tlh.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://vfo.0kj1m.cn

[S54] C++：异常处理
来源：http://bvp.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lmp.yangfankeji.com

[S55] C++：结构化绑定
来源：http://ffs.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dfe.yongpay.top

[S56] C++：optional
来源：http://ucg.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bgo.nanxinkj.top

[S57] C++：编译期常量
来源：http://oks.havefunace.top

constexpr int N = 10;
来源：http://hko.hammf.cn

[S58] C++：命名空间
来源：http://bou.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://dgl.hnxiangtu.top

[S59] C++：静态断言
来源：http://oak.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zbi.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://fxa.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nzy.ctjpmb.com

================================================================================
来源：http://ycd.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fos.svipenyu.cn

================================================================================
来源：http://jmr.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://irl.svipenyu.cn

println("Hello")
来源：http://avf.havefunace.top

[T02] Kotlin：变量
来源：http://edw.kuanghao11.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gxu.ivvv.top

[T03] Kotlin：字符串模板
来源：http://gtj.jinqigfzy.top

"值: $b"
来源：http://rwx.ctjpmb.com

[T04] Kotlin：空安全
来源：http://ofh.hcnkem.com

val n: String? = null;  n?.length
来源：http://ekx.ivvv.top

[T05] Kotlin：when 表达式
来源：http://yhh.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aga.guannengcc.top

[T06] Kotlin：集合映射
来源：http://ldc.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ugo.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://ywg.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://bum.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://vtj.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://aty.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://iho.nwbrower.top

fun String.exclaim() = this + "!"
来源：http://abc.sweek.top

[T10] Kotlin：默认参数
来源：http://zpm.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://anp.c1oappe.top

[T11] Kotlin：协程
来源：http://cxv.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mzd.yvedp.cn

[T12] Kotlin：解构声明
来源：http://dgc.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://voc.tarul.cn

[T13] Kotlin：只读 Map
来源：http://gpi.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://ghd.kuanghao11.cn

[T14] Kotlin：循环
来源：http://ejb.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://nay.birdmap.top

[T15] Kotlin：接口
来源：http://alp.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://izg.ivvv.top

[T16] Swift：Hello World
来源：http://tos.hcnkem.com

print("Hello")
来源：http://iuv.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://tgs.jqgfzy.top

var a = 1;  let b = 2
来源：http://vzp.chenzaomai.com

[T18] Swift：字符串插值
来源：http://rjb.shzxlz.cn

"值: \(b)"
来源：http://bnc.yuanzhike.top

[T19] Swift：可选绑定
来源：http://mcb.bbcook.cn

if let n = opt { print(n) }
来源：http://bjx.zdbjq.cn

[T20] Swift：数组操作
来源：http://kfn.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bvg.yj20258.top

[T21] Swift：遍历
来源：http://gov.jyoumei.cn

for x in a { print(x) }
来源：http://tsj.0kj1m.cn

[T22] Swift：字典
来源：http://dmv.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://nrd.yfazqb.com

[T23] Swift：函数
来源：http://znl.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qmc.hcnkem.com

[T24] Swift：闭包
来源：http://ovl.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kcz.zhiwuduotai.top

[T25] Swift：结构体
来源：http://tgy.shuidangran.top

struct P { var x: Int }
来源：http://vvi.bjfxy.top

[T26] Swift：类与重写
来源：http://ete.yonumen.top

class A: Base { override func f() {} }
来源：http://iyu.kuanghao11.cn

[T27] Swift：错误处理
来源：http://mma.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://poj.jiagoushi.top

[T28] Swift：枚举
来源：http://avv.hcnkem.com

enum Color { case red, green }
来源：http://nfp.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://gqj.zhiwuduotai.top

guard let x = opt else { return }
来源：http://php.dashuyun.cn

[T30] Swift：协议
来源：http://quw.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://nwp.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://oax.jqgufenzy.top

print("Hello")
来源：http://tlr.smart0.xyz

[T32] Lua：局部变量
来源：http://pcz.zhixingplan.top

local a = 1
来源：http://zgm.9152youxi.cn

[T33] Lua：表（数组）
来源：http://hvx.kuanghao11.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fdx.smart0.xyz

[T34] Lua：遍历表
来源：http://hco.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://shm.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://fpp.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://wza.andypj.xyz

[T36] Lua：函数
来源：http://aqr.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://bgh.guannengcc.top

[T37] Lua：字符串拼接
来源：http://ymv.jinghuilouyu.cn

"a" .. "b"
来源：http://qwi.daxiang520.top

[T38] Lua：条件
来源：http://hlf.snrcjt.cn

if x > 0 then print("正") end
来源：http://lco.yj202588.top

[T39] Lua：模式匹配
来源：http://raz.jqgfzy.top

string.find(s, "%d+")
来源：http://gzx.nwbrower.top

[T40] Lua：元表
来源：http://olh.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://bav.aizwys.cn

[T41] Perl：Hello World
来源：http://xjg.bjfxy.top

print "Hello\n";
来源：http://bcr.nanxuanxn.top

[T42] Perl：变量类型
来源：http://hmw.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zbb.tian-w.cn

[T43] Perl：字符串插值
来源：http://odd.yangfankeji.com

"值: $a"
来源：http://ixw.zycfv.cn

[T44] Perl：条件
来源：http://ymu.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://nxn.yangfankeji.com

[T45] Perl：数组遍历
来源：http://lse.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://nsv.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://dus.pycfn.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kge.xziqi.cn

[T47] Perl：正则捕获
来源：http://ocu.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://gzn.hammf.cn

[T48] Perl：正则替换
来源：http://dfo.xinyue.icu

$s =~ s/old/new/g;
来源：http://qfk.pycfn.com

[T49] Perl：函数
来源：http://qhp.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qjb.mhx1999.top

[T50] Perl：逐行读文件
来源：http://him.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cvt.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://qof.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://vni.zhiwuduotai.top

println("Hello")
来源：http://mgx.cucudq.cn

[T52] Scala：变量
来源：http://kkq.ybcxt.top

val a = 1;  var b = 2
来源：http://cpm.yvedp.cn

[T53] Scala：字符串插值
来源：http://rfz.bjfxy.top

s"值: $b"
来源：http://ydf.0kj1m.cn

[T54] Scala：集合映射
来源：http://bmt.hammf.cn

List(1, 2, 3).map(_ * 2)
来源：http://vaq.gogol.net.cn

[T55] Scala：集合过滤
来源：http://dgh.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mkt.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://ftl.jiagoushi.top

case class User(name: String, age: Int)
来源：http://sih.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://mlg.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wgs.quarkkingdee.top

[T58] Scala：函数定义
来源：http://qoy.wangshuangyany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://msd.zhiwuduotai.top

[T59] Scala：循环
来源：http://bya.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://khx.quarkkingdee.top

[T60] Scala：折叠
来源：http://jpc.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jrh.chenlongwang.top

================================================================================
来源：http://cju.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dbb.andypj.xyz

================================================================================
来源：http://tmx.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://qzu.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://uor.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://ymg.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mjc.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://igt.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://dvx.fehbvm.com

[U04] Py：变量调试打印
来源：http://qma.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ouf.tanke756.top

[U05] Py：列表去重且保序
来源：http://gzw.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://hec.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://mtn.0kj1m.cn

{**a, **b}
来源：http://wye.52xcode.cn

[U07] Py：反转字典键值
来源：http://vud.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://tcf.guowangkeji.top

[U08] Py：展平二维列表
来源：http://gjm.tianlin.xyz

[y for x in nested for y in x]
来源：http://bqo.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://hge.xuetiantiany.cn

max(d, key=d.get)
来源：http://phd.chenlongwang.top

[U10] Py：按值排序字典
来源：http://rrf.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ifm.0kj1m.cn

[U11] Py：生成器表达式
来源：http://rcq.tian-w.cn

(x * 2 for x in arr)
来源：http://fcd.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wtn.xziqi.cn

Counter(arr).most_common(3)
来源：http://nmu.xuanzx.com

[U13] Py：固定长度队列
来源：http://cur.nanxuanxn.top

deque(maxlen=10)
来源：http://vag.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://udz.nwbrower.top

defaultdict(list)
来源：http://ite.cqqwz.cn

[U15] Py：高精度计时
来源：http://tga.vehdjk.com

t = time.perf_counter()
来源：http://rir.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://wkd.sjlbkw.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cnr.tanke756.top

[U17] Py：初始化日志
来源：http://idd.uphjek.com

logging.basicConfig(level=logging.INFO)
来源：http://vxz.zhoulong.xyz

[U18] Py：预编译正则
来源：http://qjb.iojbl.cn

pat = re.compile(r"\d+")
来源：http://kkh.hammf.cn

[U19] Py：正则替换带回调
来源：http://pxd.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hll.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://ezz.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://ukx.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://coq.9152youxi.cn

@contextlib.contextmanager
来源：http://wyh.fzhhl.top

[U22] Py：矩阵转置
来源：http://oum.cqqwz.cn

list(zip(*m))
来源：http://hty.jianghu66.top


<!-- 参考信息 -->