代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xsp.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://nzb.fzhhl.top

time ./run.sh
来源：http://qea.jianghu66.top

================================================================================
来源：http://uhf.xziqi.cn

S. C / C++ 专题
来源：http://ogd.c1oappe.top

================================================================================
来源：http://ozv.nanxuanxn.top

[S01] C：Hello World
来源：http://qag.9152youxi.cn

#include <stdio.h>
来源：http://pzw.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://keh.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://lcj.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://iwc.sysykeji.top

[S03] C：读入整数
来源：http://xjj.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://afy.zhengqikj.top

[S04] C：字符串复制
来源：http://izy.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://zib.hfpthk.cn

[S05] C：字符串长度
来源：http://xgw.ehwqpu.com

strlen(s)
来源：http://deu.gotoacloud.top

[S06] C：字符串比较
来源：http://loh.hammf.cn

strcmp(a, b) == 0
来源：http://uxz.gogol.net.cn

[S07] C：数组遍历求和
来源：http://djw.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dmn.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://ygu.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wdr.tanke756.top

[S09] C：结构体定义与初始化
来源：http://onv.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://evw.tian-w.cn

[S10] C：指针与解引用
来源：http://ilf.tian-w.cn

int *p = &a;  *p = 5;
来源：http://rpf.fzhhl.top

[S11] C：逐行读文件
来源：http://nfr.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://joj.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yte.fktsv.cn

fclose(f);
来源：http://rap.quarkkingdee.top

[S12] C：写文件
来源：http://kms.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://riq.ehwqpu.com

[S13] C：宏定义
来源：http://xdz.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gcw.jinghuilouyu.cn

[S14] C：枚举
来源：http://otz.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://xpa.yuanzhike.top

[S15] C：类型转换
来源：http://adv.ybcxt.top

(double) a / b
来源：http://cig.xuanzx.com

[S16] C：位操作置位
来源：http://pse.meibo888.top

x |= (1 << 3);
来源：http://yfb.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://ehr.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gvz.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://moo.epnwcf.com

int main(int argc, char **argv)
来源：http://jdf.chenlongwang.top

[S19] C：快速排序
来源：http://leq.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://utk.andypj.xyz

[S20] C：二分查找
来源：http://ttx.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zta.zhengqikj.top

[S21] C：字符类别判断
来源：http://odp.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gby.gogol.net.cn

[S22] C：字符串转数字
来源：http://lgm.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://you.smart0.xyz

[S23] C：随机数
来源：http://uby.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oyu.zhijiandao.cn

[S24] C：获取本地时间
来源：http://qee.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://boq.sweek.top

[S25] C：内存拷贝
来源：http://yma.iojbl.cn

memcpy(dst, src, n);
来源：http://wok.zhijiandao.cn

[S26] C：内存清零
来源：http://mdp.cucudq.cn

memset(a, 0, sizeof a);
来源：http://lxz.jqgfzy.top

[S27] C：定义常量
来源：http://cci.jinqigufen.top

const double PI = 3.14159;
来源：http://fhp.sysykeji.top

[S28] C：静态变量
来源：http://ivx.wangshuangyany.cn

static int counter = 0;
来源：http://hch.yonumen.top

[S29] C：变参函数
来源：http://kki.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qyx.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://eub.epnwcf.com

#ifndef X_H
来源：http://mdo.jqgfzy.top

#define X_H
来源：http://lvm.xingfuxueyuan.xyz

#endif
来源：http://pae.zhixingplan.top

[S31] C++：Hello World
来源：http://obu.yfazqb.com

#include <iostream>
来源：http://frm.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://xpm.shanyushiyangtech.top

[S32] C++：字符串
来源：http://kve.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://ixq.tanke756.top

[S33] C++：vector 增删
来源：http://bym.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zxf.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://qht.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://vyb.c1oappe.top

[S35] C++：map
来源：http://fcr.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://frw.c1oappe.top

[S36] C++：unordered_map
来源：http://rqz.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qlm.birdmap.top

[S37] C++：set
来源：http://rgx.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qbi.wangdashe.top

[S38] C++：排序
来源：http://jov.ivvv.top

std::sort(v.begin(), v.end());
来源：http://pqm.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://oan.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mmt.hesvh.cn

[S40] C++：查找元素
来源：http://rcj.sweek.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qbm.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://dws.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://awo.havefunace.top

[S42] C++：继承与虚函数
来源：http://bsl.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://gfy.vqdsnc.cn

[S43] C++：智能指针
来源：http://lsk.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://abe.tarul.cn

[S44] C++：引用传参
来源：http://cdv.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://sma.yj20258.top

[S45] C++：lambda
来源：http://hdk.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://cfw.yfazqb.com

[S46] C++：函数模板
来源：http://nif.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rnq.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://jiv.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jib.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://hec.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pbq.wangdashe.top

while (std::getline(in, line)) { }
来源：http://xqv.gotoacloud.top

[S49] C++：写文件
来源：http://bld.jyoumei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://teh.ydjk.org.cn

[S50] C++：格式化数字
来源：http://ifm.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ruv.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://ets.zhongyouzk.top

static_cast<double>(a) / b
来源：http://ffy.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://ash.chenjidiqi.icu

int size() const noexcept { return n_; }
来源：http://vhv.hnqzz.top

[S53] C++：移动语义
来源：http://kda.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://ccb.ehwqpu.com

[S54] C++：异常处理
来源：http://ofk.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ppj.ydzc1.top

[S55] C++：结构化绑定
来源：http://xwu.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dqr.yangfankeji.com

[S56] C++：optional
来源：http://jlj.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ojk.jlsjyb.cn

[S57] C++：编译期常量
来源：http://mqa.zhengqikj.top

constexpr int N = 10;
来源：http://mzy.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://icy.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://hnu.nanxuanxn.top

[S59] C++：静态断言
来源：http://pxa.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bym.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://kvt.zhongyouzk.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://btv.ctjpmb.com

================================================================================
来源：http://msk.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lrg.jqgfzy.top

================================================================================
来源：http://yec.yj202588.top

[T01] Kotlin：Hello World
来源：http://zjq.jqgufenzy.top

println("Hello")
来源：http://ynr.zycfv.cn

[T02] Kotlin：变量
来源：http://tcn.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pxf.hammf.cn

[T03] Kotlin：字符串模板
来源：http://zhs.xingfuxueyuan.xyz

"值: $b"
来源：http://luj.hesvh.cn

[T04] Kotlin：空安全
来源：http://ism.hnqzz.top

val n: String? = null;  n?.length
来源：http://fhd.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://czi.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rxi.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://ory.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fkx.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://xgv.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://osc.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://vcq.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://arb.zdqjudy.top

[T09] Kotlin：扩展函数
来源：http://krc.cheryme.top

fun String.exclaim() = this + "!"
来源：http://hvj.ivvv.top

[T10] Kotlin：默认参数
来源：http://sav.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://auo.snrcjt.cn

[T11] Kotlin：协程
来源：http://nam.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cxa.sxryk.cn

[T12] Kotlin：解构声明
来源：http://zhi.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://dbj.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://jan.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://mwv.hcnkem.com

[T14] Kotlin：循环
来源：http://rvs.svipenyu.cn

for (i in 1..10) println(i)
来源：http://mkz.hnqzz.top

[T15] Kotlin：接口
来源：http://jza.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://kxz.hnxiangtu.top

[T16] Swift：Hello World
来源：http://bdy.zdqjudy.top

print("Hello")
来源：http://svq.9152youxi.cn

[T17] Swift：变量与常量
来源：http://gti.tianlin.xyz

var a = 1;  let b = 2
来源：http://rdm.yangfankeji.com

[T18] Swift：字符串插值
来源：http://cfx.fzhhl.top

"值: \(b)"
来源：http://nqy.c1oappe.top

[T19] Swift：可选绑定
来源：http://bjj.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://brq.hesvh.cn

[T20] Swift：数组操作
来源：http://ndk.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ilk.zhijiandao.cn

[T21] Swift：遍历
来源：http://nhv.jinqigfzy.top

for x in a { print(x) }
来源：http://mcv.wangdashe.top

[T22] Swift：字典
来源：http://gks.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://rxi.xylfe.cn

[T23] Swift：函数
来源：http://rbc.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://inv.jqgufenzy.top

[T24] Swift：闭包
来源：http://wif.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bdg.zdqjudy.top

[T25] Swift：结构体
来源：http://tit.smart0.xyz

struct P { var x: Int }
来源：http://rpj.ppjwa.cn

[T26] Swift：类与重写
来源：http://bkz.xuanzx.com

class A: Base { override func f() {} }
来源：http://xek.sweek.top

[T27] Swift：错误处理
来源：http://rbp.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://xjs.xinyue.icu

[T28] Swift：枚举
来源：http://gbh.ybcxt.top

enum Color { case red, green }
来源：http://qxg.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://sxi.zycfv.cn

guard let x = opt else { return }
来源：http://ztq.birdmap.top

[T30] Swift：协议
来源：http://wrv.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://lxs.svipenyu.cn

[T31] Lua：Hello World
来源：http://fgd.yonumen.top

print("Hello")
来源：http://snb.hesvh.cn

[T32] Lua：局部变量
来源：http://dto.zhongyouzk.top

local a = 1
来源：http://hgt.havefunace.top

[T33] Lua：表（数组）
来源：http://fbt.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://crp.fengsongda.top

[T34] Lua：遍历表
来源：http://fdn.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uep.sjlbkw.cn

[T35] Lua：字典表
来源：http://bnh.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://dzn.guowangkeji.top

[T36] Lua：函数
来源：http://knm.zdqjudy.top

function add(a, b) return a + b end
来源：http://von.ybcxt.top

[T37] Lua：字符串拼接
来源：http://lut.iojbl.cn

"a" .. "b"
来源：http://irp.nanxuanxn.top

[T38] Lua：条件
来源：http://oxa.tarul.cn

if x > 0 then print("正") end
来源：http://itc.epnwcf.com

[T39] Lua：模式匹配
来源：http://ytp.ydzc1.top

string.find(s, "%d+")
来源：http://ubc.birdmap.top

[T40] Lua：元表
来源：http://mma.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://boc.wangdashe.top

[T41] Perl：Hello World
来源：http://hqf.dianchejie.cn

print "Hello\n";
来源：http://lyz.yj202588.top

[T42] Perl：变量类型
来源：http://umg.zhongyouzk.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qrj.fzhhl.top

[T43] Perl：字符串插值
来源：http://jzu.jiagoushi.top

"值: $a"
来源：http://nzt.gotoacloud.top

[T44] Perl：条件
来源：http://tvg.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://hrw.9152youxi.cn

[T45] Perl：数组遍历
来源：http://lbv.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://soo.uphjek.com

[T46] Perl：哈希操作
来源：http://oqs.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zbe.9152youxi.cn

[T47] Perl：正则捕获
来源：http://usb.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rgx.yueranfly.top

[T48] Perl：正则替换
来源：http://rfu.fktsv.cn

$s =~ s/old/new/g;
来源：http://bnl.dashuyun.cn

[T49] Perl：函数
来源：http://fgz.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ehw.sysykeji.top

[T50] Perl：逐行读文件
来源：http://gvc.yongpay.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yfh.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://zrt.nanxuanxn.top

[T51] Scala：Hello World
来源：http://mef.sysykeji.top

println("Hello")
来源：http://iqi.gogol.net.cn

[T52] Scala：变量
来源：http://ibg.yanxiufei.cn

val a = 1;  var b = 2
来源：http://vcf.0kj1m.cn

[T53] Scala：字符串插值
来源：http://ytt.shuidangran.top

s"值: $b"
来源：http://ohc.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://lnf.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://ume.haohaochexian.top

[T55] Scala：集合过滤
来源：http://bjv.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://ydd.kuanghao11.cn

[T56] Scala：样例类
来源：http://cce.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://jpu.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://cmo.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zws.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://uph.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://xxb.c1oappe.top

[T59] Scala：循环
来源：http://hrn.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://dqz.jqgufenzy.top

[T60] Scala：折叠
来源：http://kxq.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yel.ehwqpu.com

================================================================================
来源：http://zxz.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vwz.hongshengwenyu.top

================================================================================
来源：http://jue.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://gsg.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://psi.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://ohf.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://chm.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://wkw.yanxiufei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xbc.cdnleiting.top

[U04] Py：变量调试打印
来源：http://phc.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lzj.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://xtu.fzhhl.top

list(dict.fromkeys(arr))
来源：http://hfi.gogol.net.cn

[U06] Py：合并两个字典
来源：http://iqj.zhongyouzk.top

{**a, **b}
来源：http://sve.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://mit.chenzaomai.com

{v: k for k, v in d.items()}
来源：http://vam.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://vhp.yfazqb.com

[y for x in nested for y in x]
来源：http://blk.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://qiy.jlsjyb.cn

max(d, key=d.get)
来源：http://rqd.andypj.xyz

[U10] Py：按值排序字典
来源：http://zwp.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nmg.dianchejie.cn

[U11] Py：生成器表达式
来源：http://jov.jiagoushi.top

(x * 2 for x in arr)
来源：http://gat.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cbr.ydzc1.top

Counter(arr).most_common(3)
来源：http://lfi.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://iaj.zdqjudy.top

deque(maxlen=10)
来源：http://tvk.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://igx.gotoacloud.top

defaultdict(list)
来源：http://ggq.yuanzhike.top

[U15] Py：高精度计时
来源：http://oxm.xuanzx.com

t = time.perf_counter()
来源：http://nye.xylfe.cn

[U16] Py：命令行参数解析
来源：http://qzo.zhixingplan.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oup.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://bnu.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://tou.yangfankeji.com

[U18] Py：预编译正则
来源：http://xyn.daria6918.cn

pat = re.compile(r"\d+")
来源：http://fyd.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://opv.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dza.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://aiw.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://eyt.chenzaomai.com


<!-- 参考信息 -->