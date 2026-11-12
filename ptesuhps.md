代发 wailian999

read -rp "请输入: " ans
来源：http://lum.xuetiantiany.cn

[R78] 交互式菜单
来源：http://ypm.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mwu.jqgfzy.top

[R79] 解析命令行选项
来源：http://sgm.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cbw.yonumen.top

[R80] 查看脚本执行耗时
来源：http://vkh.sufxvd.cn

time ./run.sh
来源：http://lta.uphjek.com

================================================================================
来源：http://vvk.zhijiandao.cn

S. C / C++ 专题
来源：http://yzl.yj20258.top

================================================================================
来源：http://jcx.tianlin.xyz

[S01] C：Hello World
来源：http://oti.meibo888.top

#include <stdio.h>
来源：http://vxv.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fvz.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://amp.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://vib.uphjek.com

[S03] C：读入整数
来源：http://lcn.nanxinkj.top

int x; scanf("%d", &x);
来源：http://xow.aibaodan.cn

[S04] C：字符串复制
来源：http://etv.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://hyo.zhoulong.xyz

[S05] C：字符串长度
来源：http://wkn.nanxuanxn.top

strlen(s)
来源：http://fjs.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://pdn.0kj1m.cn

strcmp(a, b) == 0
来源：http://mzc.gogol.net.cn

[S07] C：数组遍历求和
来源：http://oej.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://taw.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://qvj.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://snh.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://gji.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://orz.snrcjt.cn

[S10] C：指针与解引用
来源：http://mhx.nwbrower.top

int *p = &a;  *p = 5;
来源：http://lev.hywenlv.cn

[S11] C：逐行读文件
来源：http://yie.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://fgg.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://imv.ydjk.org.cn

fclose(f);
来源：http://nzh.hongshengwenyu.top

[S12] C：写文件
来源：http://gfh.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jgg.fzhhl.top

[S13] C：宏定义
来源：http://kmx.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zkt.yfazqb.com

[S14] C：枚举
来源：http://oap.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://hdv.jinghuilouyu.cn

[S15] C：类型转换
来源：http://qjf.bbcook.cn

(double) a / b
来源：http://ubr.ppjwa.cn

[S16] C：位操作置位
来源：http://cax.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://sky.c1oappe.top

[S17] C：安全拼接字符串
来源：http://xzk.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bsb.jqgufenzy.top

[S18] C：命令行参数
来源：http://zch.wangdashe.top

int main(int argc, char **argv)
来源：http://jbf.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://mnk.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sjp.vqdsnc.cn

[S20] C：二分查找
来源：http://iql.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://chj.hnxiangtu.top

[S21] C：字符类别判断
来源：http://fmd.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fdi.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://caj.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://vbl.snrcjt.cn

[S23] C：随机数
来源：http://yev.zhengqikj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pux.nanxuanxn.top

[S24] C：获取本地时间
来源：http://hjr.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zdm.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://ycu.jqgfzy.top

memcpy(dst, src, n);
来源：http://vlw.sweek.top

[S26] C：内存清零
来源：http://vsy.redwolf501.top

memset(a, 0, sizeof a);
来源：http://kmn.chenzaomai.com

[S27] C：定义常量
来源：http://xva.guannengcc.top

const double PI = 3.14159;
来源：http://ugw.sxryk.cn

[S28] C：静态变量
来源：http://tar.chenjidiqi.icu

static int counter = 0;
来源：http://hbp.smart0.xyz

[S29] C：变参函数
来源：http://mlr.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ppk.hnqzz.top

[S30] C：头文件保护
来源：http://iek.52xcode.cn

#ifndef X_H
来源：http://wbe.jinqigfzy.top

#define X_H
来源：http://laa.feifeiyinyue.top

#endif
来源：http://awg.sxryk.cn

[S31] C++：Hello World
来源：http://rnx.birdmap.top

#include <iostream>
来源：http://ikv.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://xno.havefunace.top

[S32] C++：字符串
来源：http://knz.cashguo.top

std::string s = "hi";  s += "!";
来源：http://mhc.tarul.cn

[S33] C++：vector 增删
来源：http://xna.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ldd.uphjek.com

[S34] C++：遍历 vector
来源：http://vwc.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://lsr.9152youxi.cn

[S35] C++：map
来源：http://ktk.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mcz.jyoumei.cn

[S36] C++：unordered_map
来源：http://csg.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zwg.guowangkeji.top

[S37] C++：set
来源：http://fcv.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jgw.pycfn.com

[S38] C++：排序
来源：http://its.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://uyl.sweek.top

[S39] C++：自定义比较器排序
来源：http://edr.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sfq.zhengqikj.top

[S40] C++：查找元素
来源：http://cbo.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vsx.gzhubu.top

[S41] C++：类与构造函数
来源：http://fxw.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sco.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://kda.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://ktd.ctjpmb.com

[S43] C++：智能指针
来源：http://hgx.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://nhe.feifeiyinyue.top

[S44] C++：引用传参
来源：http://qee.fehbvm.com

void inc(int &x) { ++x; }
来源：http://zdt.cdnleiting.top

[S45] C++：lambda
来源：http://ryd.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://qrh.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://vuw.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dip.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://sam.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lgd.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://fyj.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://pjn.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://fci.shangyingyoupin.top

[S49] C++：写文件
来源：http://xiw.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sat.yuxming.cn

[S50] C++：格式化数字
来源：http://sqq.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gvm.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://vjv.bjfxy.top

static_cast<double>(a) / b
来源：http://iig.birdmap.top

[S52] C++：const 与 noexcept
来源：http://lcm.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://ifz.mhx1999.top

[S53] C++：移动语义
来源：http://hbc.ivvv.top

std::vector<int> w = std::move(v);
来源：http://rve.yueranfly.top

[S54] C++：异常处理
来源：http://fab.chenjidiqi.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qym.aizwys.cn

[S55] C++：结构化绑定
来源：http://ngz.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zpq.ppjwa.cn

[S56] C++：optional
来源：http://wca.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mer.shanyushiyangtech.top

[S57] C++：编译期常量
来源：http://xuc.cashguo.top

constexpr int N = 10;
来源：http://vau.c1oappe.top

[S58] C++：命名空间
来源：http://rak.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://svm.ehwqpu.com

[S59] C++：静态断言
来源：http://wmf.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nuz.uphjek.com

[S60] C++：遍历并删除元素
来源：http://sju.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ygo.hnqzz.top

================================================================================
来源：http://hdx.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yhg.jqgufenzy.top

================================================================================
来源：http://zpu.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://okr.dashuyun.cn

println("Hello")
来源：http://xrw.sufxvd.cn

[T02] Kotlin：变量
来源：http://gop.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://twh.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://mla.redwolf501.top

"值: $b"
来源：http://ahh.cucudq.cn

[T04] Kotlin：空安全
来源：http://aat.jqgfzy.top

val n: String? = null;  n?.length
来源：http://msr.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://scl.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zwe.nwbrower.top

[T06] Kotlin：集合映射
来源：http://goc.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hcq.pycfn.com

[T07] Kotlin：集合过滤
来源：http://xzm.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://fuj.gotoacloud.top

[T08] Kotlin：数据类
来源：http://rut.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://pgd.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://zst.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://qzs.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://rqo.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://agx.c1oappe.top

[T11] Kotlin：协程
来源：http://fyo.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kia.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://zaj.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://sxj.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://gsz.sysykeji.top

val m = mapOf("a" to 1)
来源：http://gfx.ydzc1.top

[T14] Kotlin：循环
来源：http://vfz.xylfe.cn

for (i in 1..10) println(i)
来源：http://lud.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://nsj.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://qth.meibo888.top

[T16] Swift：Hello World
来源：http://awd.bjfxy.top

print("Hello")
来源：http://nxy.jinqigufen.top

[T17] Swift：变量与常量
来源：http://ndd.zhengqikj.top

var a = 1;  let b = 2
来源：http://rjr.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://jub.jqgfzy.top

"值: \(b)"
来源：http://uos.quarkkingdee.top

[T19] Swift：可选绑定
来源：http://szy.jiagoushi.top

if let n = opt { print(n) }
来源：http://spi.uphjek.com

[T20] Swift：数组操作
来源：http://hpr.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://rwx.52xcode.cn

[T21] Swift：遍历
来源：http://fts.yanxiufei.cn

for x in a { print(x) }
来源：http://teu.haohaochexian.top

[T22] Swift：字典
来源：http://wqs.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qcw.redwolf501.top

[T23] Swift：函数
来源：http://usf.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wgi.guowangkeji.top

[T24] Swift：闭包
来源：http://rtp.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://knn.uphjek.com

[T25] Swift：结构体
来源：http://oul.andypj.xyz

struct P { var x: Int }
来源：http://way.cqqwz.cn

[T26] Swift：类与重写
来源：http://hyl.dashuyun.cn

class A: Base { override func f() {} }
来源：http://jhj.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://rns.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://ntc.nwbrower.top

[T28] Swift：枚举
来源：http://wni.fzhhl.top

enum Color { case red, green }
来源：http://tel.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://zur.xuanzx.com

guard let x = opt else { return }
来源：http://gnv.cheryme.top

[T30] Swift：协议
来源：http://keg.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://auf.bjfxy.top

[T31] Lua：Hello World
来源：http://zei.havefunace.top

print("Hello")
来源：http://uld.jqgfzy.top

[T32] Lua：局部变量
来源：http://njf.guannengcc.top

local a = 1
来源：http://idz.yj202588.top

[T33] Lua：表（数组）
来源：http://emz.hcnkem.com

local t = {1, 2, 3};  t[4] = 4
来源：http://onh.vehdjk.com

[T34] Lua：遍历表
来源：http://smf.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://uhm.yfazqb.com

[T35] Lua：字典表
来源：http://xha.wangdashe.top

local d = { a = 1 };  d.b = 2
来源：http://cwf.zhixingplan.top

[T36] Lua：函数
来源：http://qvv.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://yxc.chenzaomai.com

[T37] Lua：字符串拼接
来源：http://rob.yonumen.top

"a" .. "b"
来源：http://bpc.zdqjudy.top

[T38] Lua：条件
来源：http://hek.fzhhl.top

if x > 0 then print("正") end
来源：http://mlr.vehdjk.com

[T39] Lua：模式匹配
来源：http://ykl.quarkkingdee.top

string.find(s, "%d+")
来源：http://dqc.ppjwa.cn

[T40] Lua：元表
来源：http://jux.epnwcf.com

setmetatable({}, { __index = base })
来源：http://fyi.yanxiufei.cn

[T41] Perl：Hello World
来源：http://bvw.yuxming.cn

print "Hello\n";
来源：http://hob.jianghu66.top

[T42] Perl：变量类型
来源：http://uoz.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mrv.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://rsc.cdnleiting.top

"值: $a"
来源：http://mcb.sjlbkw.cn

[T44] Perl：条件
来源：http://gcm.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://tib.hongshengwenyu.top

[T45] Perl：数组遍历
来源：http://eqy.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://jzh.yj20258.top

[T46] Perl：哈希操作
来源：http://oen.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ywn.dashuyun.cn

[T47] Perl：正则捕获
来源：http://dia.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lso.tarul.cn

[T48] Perl：正则替换
来源：http://wyk.bbcook.cn

$s =~ s/old/new/g;
来源：http://sge.yueranfly.top

[T49] Perl：函数
来源：http://kzt.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dxb.shanyushiyangkeji.top

[T50] Perl：逐行读文件
来源：http://vff.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kos.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://vxm.cashguo.top

[T51] Scala：Hello World
来源：http://pru.zdbjq.cn

println("Hello")
来源：http://atr.mhx1999.top

[T52] Scala：变量
来源：http://umi.birdmap.top

val a = 1;  var b = 2
来源：http://adc.sxryk.cn

[T53] Scala：字符串插值
来源：http://qob.daria6918.cn

s"值: $b"
来源：http://mog.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://kni.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://kcm.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://yxp.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://fpj.yonumen.top

[T56] Scala：样例类
来源：http://pdz.ivvv.top

case class User(name: String, age: Int)
来源：http://jqk.aibaodan.cn

[T57] Scala：模式匹配
来源：http://doh.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ymq.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://ygb.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qwy.yangfankeji.com

[T59] Scala：循环
来源：http://hct.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://qgr.zycfv.cn

[T60] Scala：折叠
来源：http://xup.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cam.guowangkeji.top

================================================================================
来源：http://don.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pmb.52xcode.cn

================================================================================
来源：http://gcy.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://hzx.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yrm.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://eog.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xyk.aibaodan.cn

[U03] Py：加载 .env 配置
来源：http://zwb.yanxiufei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xau.cashguo.top

[U04] Py：变量调试打印
来源：http://jhu.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rnf.fengsongda.top

[U05] Py：列表去重且保序
来源：http://emf.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://rqv.dashuyun.cn

[U06] Py：合并两个字典
来源：http://dyu.c1oappe.top

{**a, **b}
来源：http://qbd.wangdashe.top

[U07] Py：反转字典键值
来源：http://rcf.tian-w.cn

{v: k for k, v in d.items()}
来源：http://rpw.cheryme.top

[U08] Py：展平二维列表
来源：http://mmn.jinyuanbaomall.cn

[y for x in nested for y in x]
来源：http://mpi.tarul.cn

[U09] Py：字典取最大值的键
来源：http://mjo.chenzaomai.com

max(d, key=d.get)
来源：http://vxi.zdqjudy.top

[U10] Py：按值排序字典
来源：http://ndf.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://udz.cheryme.top

[U11] Py：生成器表达式
来源：http://eyq.bjfxy.top

(x * 2 for x in arr)
来源：http://sai.shzxlz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://trh.yuxming.cn

Counter(arr).most_common(3)
来源：http://tid.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://xtw.zhongyouzk.top

deque(maxlen=10)
来源：http://gci.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://kbh.9152youxi.cn

defaultdict(list)
来源：http://xpz.shzxlz.cn

[U15] Py：高精度计时
来源：http://ccn.yanxiufei.cn

t = time.perf_counter()
来源：http://nob.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://lul.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ywx.daria6918.cn

[U17] Py：初始化日志
来源：http://uzp.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://tdr.uphjek.com

[U18] Py：预编译正则
来源：http://gaw.yj20258.top

pat = re.compile(r"\d+")
来源：http://gul.guannengcc.top


<!-- 参考信息 -->