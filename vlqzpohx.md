代发 wailian999

read -rp "请输入: " ans
来源：http://dqe.yanxiufei.cn

[R78] 交互式菜单
来源：http://tom.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://kde.zhixingplan.top

[R79] 解析命令行选项
来源：http://skp.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jcr.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://szw.yongpay.top

time ./run.sh
来源：http://zmt.hcnkem.com

================================================================================
来源：http://ovt.vehdjk.com

S. C / C++ 专题
来源：http://pty.zhijiandao.cn

================================================================================
来源：http://tsx.wangshuangyany.cn

[S01] C：Hello World
来源：http://ssf.yfazqb.com

#include <stdio.h>
来源：http://zcq.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://xpl.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://yoo.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://rss.havefunace.top

[S03] C：读入整数
来源：http://lvq.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://iqf.fengsongda.top

[S04] C：字符串复制
来源：http://qmt.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://weq.chenlongwang.top

[S05] C：字符串长度
来源：http://hzk.iojbl.cn

strlen(s)
来源：http://vur.yangfankeji.com

[S06] C：字符串比较
来源：http://iwb.yuxming.cn

strcmp(a, b) == 0
来源：http://epr.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://jut.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gmt.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://aqk.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qjx.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://mmc.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cbf.gogol.net.cn

[S10] C：指针与解引用
来源：http://ptv.yvedp.cn

int *p = &a;  *p = 5;
来源：http://kdq.hysaishi.cn

[S11] C：逐行读文件
来源：http://ilp.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://qgi.sufxvd.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kbp.vehdjk.com

fclose(f);
来源：http://uzt.hammf.cn

[S12] C：写文件
来源：http://gzu.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lae.ivvv.top

[S13] C：宏定义
来源：http://zzp.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fpe.aibaodan.cn

[S14] C：枚举
来源：http://kog.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://rli.hesvh.cn

[S15] C：类型转换
来源：http://tnv.52xcode.cn

(double) a / b
来源：http://elw.tianlin.xyz

[S16] C：位操作置位
来源：http://bdk.quarkkingdee.top

x |= (1 << 3);
来源：http://amq.bjfxy.top

[S17] C：安全拼接字符串
来源：http://ukd.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ddg.tanke756.top

[S18] C：命令行参数
来源：http://qwq.xinyue.icu

int main(int argc, char **argv)
来源：http://fcj.yj20258888.top

[S19] C：快速排序
来源：http://ogp.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://obm.tianlin.xyz

[S20] C：二分查找
来源：http://gpt.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tlx.yuanzhike.top

[S21] C：字符类别判断
来源：http://nyw.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fpy.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://euo.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://swu.nanxinkj.top

[S23] C：随机数
来源：http://phv.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lfu.hcnkem.com

[S24] C：获取本地时间
来源：http://mpx.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oej.kuanghao11.cn

[S25] C：内存拷贝
来源：http://aaa.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://qwd.ybcxt.top

[S26] C：内存清零
来源：http://xfc.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://rbf.yueranfly.top

[S27] C：定义常量
来源：http://jdf.tarul.cn

const double PI = 3.14159;
来源：http://prm.cheryme.top

[S28] C：静态变量
来源：http://yvm.yongpay.top

static int counter = 0;
来源：http://ryu.hcnkem.com

[S29] C：变参函数
来源：http://mpn.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://raz.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://jfs.jlsjyb.cn

#ifndef X_H
来源：http://wag.zdqjudy.top

#define X_H
来源：http://nah.havefunace.top

#endif
来源：http://ilu.cdnleiting.top

[S31] C++：Hello World
来源：http://ovx.zhoulong.xyz

#include <iostream>
来源：http://qgc.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://lku.nwbrower.top

[S32] C++：字符串
来源：http://dss.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://gpv.gotoacloud.top

[S33] C++：vector 增删
来源：http://dsy.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dlt.mhx1999.top

[S34] C++：遍历 vector
来源：http://xqw.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://njg.vehdjk.com

[S35] C++：map
来源：http://upx.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jaj.zhongyouzk.top

[S36] C++：unordered_map
来源：http://crd.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vqz.jlsjyb.cn

[S37] C++：set
来源：http://qyq.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://phe.tanke756.top

[S38] C++：排序
来源：http://wol.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://scd.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://jzt.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ppe.xinyue.icu

[S40] C++：查找元素
来源：http://yuf.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://amp.guowangkeji.top

[S41] C++：类与构造函数
来源：http://yrg.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://thc.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://cys.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://xml.shzxlz.cn

[S43] C++：智能指针
来源：http://ynj.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://tgp.gzhubu.top

[S44] C++：引用传参
来源：http://sje.guannengcc.top

void inc(int &x) { ++x; }
来源：http://tbx.zycfv.cn

[S45] C++：lambda
来源：http://tla.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fcr.bjfxy.top

[S46] C++：函数模板
来源：http://ncu.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mlb.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://jzt.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hod.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://ehh.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://egs.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://vmd.meibo888.top

[S49] C++：写文件
来源：http://sgj.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dtw.ctjpmb.com

[S50] C++：格式化数字
来源：http://jmo.fzhhl.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fyp.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://bif.guannengcc.top

static_cast<double>(a) / b
来源：http://nml.yj202588.top

[S52] C++：const 与 noexcept
来源：http://xey.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://yzj.mhx1999.top

[S53] C++：移动语义
来源：http://uxt.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://mrs.yj202588.top

[S54] C++：异常处理
来源：http://ggt.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://otq.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://yoy.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fxe.yangfankeji.com

[S56] C++：optional
来源：http://hwo.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ikz.xylfe.cn

[S57] C++：编译期常量
来源：http://icc.sufxvd.cn

constexpr int N = 10;
来源：http://qbz.feifeiyinyue.top

[S58] C++：命名空间
来源：http://xmq.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://jkr.nanxuanxn.top

[S59] C++：静态断言
来源：http://peq.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qrc.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://jvx.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zai.yj202588.top

================================================================================
来源：http://rlh.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mcm.nanxinkj.top

================================================================================
来源：http://xhv.yj202588.top

[T01] Kotlin：Hello World
来源：http://chu.yj20258.top

println("Hello")
来源：http://tjc.yongpay.top

[T02] Kotlin：变量
来源：http://tcs.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nwn.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://bcd.jqgufenzy.top

"值: $b"
来源：http://tar.ctjpmb.com

[T04] Kotlin：空安全
来源：http://bjv.xuanzx.com

val n: String? = null;  n?.length
来源：http://fpe.cheryme.top

[T05] Kotlin：when 表达式
来源：http://uym.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ule.sysykeji.top

[T06] Kotlin：集合映射
来源：http://mbp.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qfb.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://tul.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://saa.aizwys.cn

[T08] Kotlin：数据类
来源：http://kct.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://qlj.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://itj.jiagoushi.top

fun String.exclaim() = this + "!"
来源：http://xct.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://wda.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tun.hnxiangtu.top

[T11] Kotlin：协程
来源：http://bul.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ray.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://elj.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://nfx.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://gwb.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://gue.cqqwz.cn

[T14] Kotlin：循环
来源：http://grh.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://yed.zhijiandao.cn

[T15] Kotlin：接口
来源：http://uog.sweek.top

interface Shape { fun area(): Double }
来源：http://ojq.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://hzf.fengsongda.top

print("Hello")
来源：http://mhf.zhongyouzk.top

[T17] Swift：变量与常量
来源：http://eov.yvedp.cn

var a = 1;  let b = 2
来源：http://reu.zycfv.cn

[T18] Swift：字符串插值
来源：http://ivz.zdbjq.cn

"值: \(b)"
来源：http://uls.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://ecf.tanke756.top

if let n = opt { print(n) }
来源：http://tdx.jinqigfzy.top

[T20] Swift：数组操作
来源：http://ssd.chenzaomai.com

var a = [1, 2, 3];  a.append(4)
来源：http://hma.zhongyouzk.top

[T21] Swift：遍历
来源：http://ctx.andypj.xyz

for x in a { print(x) }
来源：http://kli.cucudq.cn

[T22] Swift：字典
来源：http://cix.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://jpq.ybcxt.top

[T23] Swift：函数
来源：http://huc.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://csp.jlsjyb.cn

[T24] Swift：闭包
来源：http://aog.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jks.sweek.top

[T25] Swift：结构体
来源：http://okc.smart0.xyz

struct P { var x: Int }
来源：http://ayq.iojbl.cn

[T26] Swift：类与重写
来源：http://iie.xziqi.cn

class A: Base { override func f() {} }
来源：http://tct.zhijiandao.cn

[T27] Swift：错误处理
来源：http://xkt.nwbrower.top

do { try f() } catch { print(error) }
来源：http://rmi.kuanghao11.cn

[T28] Swift：枚举
来源：http://qvr.hongshengwenyu.top

enum Color { case red, green }
来源：http://php.jinqigufen.top

[T29] Swift：guard 提前返回
来源：http://txl.vehdjk.com

guard let x = opt else { return }
来源：http://mvs.shuidangran.top

[T30] Swift：协议
来源：http://kik.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://tvu.hammf.cn

[T31] Lua：Hello World
来源：http://cxm.yuxming.cn

print("Hello")
来源：http://tem.zhaomingkeji.xyz

[T32] Lua：局部变量
来源：http://ucq.mhx1999.top

local a = 1
来源：http://tux.bbcook.cn

[T33] Lua：表（数组）
来源：http://brn.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://qqh.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://sum.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://yll.hnxiangtu.top

[T35] Lua：字典表
来源：http://erc.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://bdn.zhoulong.xyz

[T36] Lua：函数
来源：http://ltl.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://dhb.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://hgs.cqqwz.cn

"a" .. "b"
来源：http://tgm.vqdsnc.cn

[T38] Lua：条件
来源：http://pdh.yj20258.top

if x > 0 then print("正") end
来源：http://jsm.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://vpd.zhijiandao.cn

string.find(s, "%d+")
来源：http://dqk.yongpay.top

[T40] Lua：元表
来源：http://hws.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://gdd.kuanghao11.cn

[T41] Perl：Hello World
来源：http://hhb.zhengqikj.top

print "Hello\n";
来源：http://zln.nwbrower.top

[T42] Perl：变量类型
来源：http://ool.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://igz.52xcode.cn

[T43] Perl：字符串插值
来源：http://dtc.gzhubu.top

"值: $a"
来源：http://boy.hammf.cn

[T44] Perl：条件
来源：http://ahx.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://llf.pycfn.com

[T45] Perl：数组遍历
来源：http://ovb.haohaochexian.top

for my $x (@arr) { print $x; }
来源：http://ahd.yuanzhike.top

[T46] Perl：哈希操作
来源：http://uja.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hpg.yonumen.top

[T47] Perl：正则捕获
来源：http://xmh.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://khb.zdbjq.cn

[T48] Perl：正则替换
来源：http://aix.snrcjt.cn

$s =~ s/old/new/g;
来源：http://udz.bjfxy.top

[T49] Perl：函数
来源：http://dyt.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dkx.zhiwuduotai.top

[T50] Perl：逐行读文件
来源：http://whe.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zyw.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://mab.jqgufenzy.top

[T51] Scala：Hello World
来源：http://ken.vqdsnc.cn

println("Hello")
来源：http://mnw.sxryk.cn

[T52] Scala：变量
来源：http://rkc.hywenlv.cn

val a = 1;  var b = 2
来源：http://zvr.daxiang520.top

[T53] Scala：字符串插值
来源：http://zsc.zdbjq.cn

s"值: $b"
来源：http://tsm.birdmap.top

[T54] Scala：集合映射
来源：http://amz.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://gif.smart0.xyz

[T55] Scala：集合过滤
来源：http://phk.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://kev.wangshuangyany.cn

[T56] Scala：样例类
来源：http://axi.0kj1m.cn

case class User(name: String, age: Int)
来源：http://cwx.meibo888.top

[T57] Scala：模式匹配
来源：http://lmk.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dft.meibo888.top

[T58] Scala：函数定义
来源：http://ebg.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hil.jqgfzy.top

[T59] Scala：循环
来源：http://syz.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://koz.zycfv.cn

[T60] Scala：折叠
来源：http://kpf.xinyue.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yyk.yj202588.top

================================================================================
来源：http://lbh.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vqe.316326.xyz

================================================================================
来源：http://fkw.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://vao.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://hpw.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://ioj.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vcu.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://wds.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qsw.havefunace.top

[U04] Py：变量调试打印
来源：http://pji.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wvb.mhx1999.top

[U05] Py：列表去重且保序
来源：http://fhv.smart0.xyz

list(dict.fromkeys(arr))
来源：http://iqm.cashguo.top

[U06] Py：合并两个字典
来源：http://apt.nanxuanxn.top

{**a, **b}
来源：http://wdr.meibo888.top

[U07] Py：反转字典键值
来源：http://bvy.vehdjk.com

{v: k for k, v in d.items()}
来源：http://dgx.mhx1999.top

[U08] Py：展平二维列表
来源：http://iml.yangfankeji.com

[y for x in nested for y in x]
来源：http://esp.meibo888.top

[U09] Py：字典取最大值的键
来源：http://lqk.bjfxy.top

max(d, key=d.get)
来源：http://emi.zhixingplan.top

[U10] Py：按值排序字典
来源：http://cmi.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wjr.yfazqb.com

[U11] Py：生成器表达式
来源：http://ins.hcnkem.com

(x * 2 for x in arr)
来源：http://kul.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cum.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://nns.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://aqo.xuanzx.com

deque(maxlen=10)
来源：http://ite.andypj.xyz

[U14] Py：分组收集到列表
来源：http://noo.zhongyouzk.top

defaultdict(list)
来源：http://hmm.zhongyouzk.top

[U15] Py：高精度计时
来源：http://lsm.cdnleiting.top

t = time.perf_counter()
来源：http://aov.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://jzu.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pnp.316326.xyz

[U17] Py：初始化日志
来源：http://wyu.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://eih.tarul.cn

[U18] Py：预编译正则
来源：http://qvf.52xcode.cn

pat = re.compile(r"\d+")
来源：http://qoe.nanxinkj.top


<!-- 参考信息 -->