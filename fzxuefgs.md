代发 wailian999

read -rp "请输入: " ans
来源：http://fmh.yvedp.cn

[R78] 交互式菜单
来源：http://kvs.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uhs.yuanzhike.top

[R79] 解析命令行选项
来源：http://mut.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ezu.pycfn.com

[R80] 查看脚本执行耗时
来源：http://hig.316326.xyz

time ./run.sh
来源：http://sib.ivvv.top

================================================================================
来源：http://ntb.sufxvd.cn

S. C / C++ 专题
来源：http://acp.zhixingplan.top

================================================================================
来源：http://pnf.zhixingplan.top

[S01] C：Hello World
来源：http://lwi.cashguo.top

#include <stdio.h>
来源：http://lmm.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sid.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://lwp.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://ltz.ydjk.org.cn

[S03] C：读入整数
来源：http://fdz.bbcook.cn

int x; scanf("%d", &x);
来源：http://ott.xuetiantiany.cn

[S04] C：字符串复制
来源：http://irn.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cwk.tian-w.cn

[S05] C：字符串长度
来源：http://qgt.daria6918.cn

strlen(s)
来源：http://afi.jqgfzy.top

[S06] C：字符串比较
来源：http://lgd.gotoacloud.top

strcmp(a, b) == 0
来源：http://eqz.tian-w.cn

[S07] C：数组遍历求和
来源：http://frv.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://won.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://cnn.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qks.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://dnx.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xsq.smart0.xyz

[S10] C：指针与解引用
来源：http://chr.tian-w.cn

int *p = &a;  *p = 5;
来源：http://iqa.316326.xyz

[S11] C：逐行读文件
来源：http://bpy.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://ebr.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tnw.ybcxt.top

fclose(f);
来源：http://fjl.epnwcf.com

[S12] C：写文件
来源：http://uok.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oyq.aizwys.cn

[S13] C：宏定义
来源：http://whv.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bqi.jqgufenzy.top

[S14] C：枚举
来源：http://ucz.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://mby.jinghuilouyu.cn

[S15] C：类型转换
来源：http://hws.fktsv.cn

(double) a / b
来源：http://wag.vehdjk.com

[S16] C：位操作置位
来源：http://eds.quarkkingdee.top

x |= (1 << 3);
来源：http://vki.xziqi.cn

[S17] C：安全拼接字符串
来源：http://ijh.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dzf.ydzc1.top

[S18] C：命令行参数
来源：http://rtj.hnxiangtu.top

int main(int argc, char **argv)
来源：http://exr.tianlin.xyz

[S19] C：快速排序
来源：http://nch.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://vss.ppjwa.cn

[S20] C：二分查找
来源：http://euw.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fxd.jinqigufen.top

[S21] C：字符类别判断
来源：http://wad.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ddi.jinqigfzy.top

[S22] C：字符串转数字
来源：http://pik.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://ala.iojbl.cn

[S23] C：随机数
来源：http://mgi.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cra.epnwcf.com

[S24] C：获取本地时间
来源：http://imm.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sne.bbcook.cn

[S25] C：内存拷贝
来源：http://msx.52xcode.cn

memcpy(dst, src, n);
来源：http://nvb.jinqigufen.top

[S26] C：内存清零
来源：http://qhd.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://sbz.ctjpmb.com

[S27] C：定义常量
来源：http://rje.hesvh.cn

const double PI = 3.14159;
来源：http://hcy.316326.xyz

[S28] C：静态变量
来源：http://cfg.hongshengwenyu.top

static int counter = 0;
来源：http://bxc.shzxlz.cn

[S29] C：变参函数
来源：http://yrk.zhoulong.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kjo.ehwqpu.com

[S30] C：头文件保护
来源：http://aqf.chenlongwang.top

#ifndef X_H
来源：http://ywm.jinqigfzy.top

#define X_H
来源：http://vvq.fehbvm.com

#endif
来源：http://sls.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://jex.316326.xyz

#include <iostream>
来源：http://zrh.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://okg.hesvh.cn

[S32] C++：字符串
来源：http://fkg.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://fxr.gogol.net.cn

[S33] C++：vector 增删
来源：http://gma.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vew.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://yif.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://xen.yj20258.top

[S35] C++：map
来源：http://sxq.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://owu.ybcxt.top

[S36] C++：unordered_map
来源：http://dbb.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dyb.yongpay.top

[S37] C++：set
来源：http://nlu.sxryk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://unb.smart0.xyz

[S38] C++：排序
来源：http://wgt.316326.xyz

std::sort(v.begin(), v.end());
来源：http://bfo.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://mkw.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wnl.hesvh.cn

[S40] C++：查找元素
来源：http://nhv.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wud.nanxinkj.top

[S41] C++：类与构造函数
来源：http://ott.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wej.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://lru.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://lou.gotoacloud.top

[S43] C++：智能指针
来源：http://vxf.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://wtp.52xcode.cn

[S44] C++：引用传参
来源：http://ndt.tian-w.cn

void inc(int &x) { ++x; }
来源：http://dmm.tianlin.xyz

[S45] C++：lambda
来源：http://qnu.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://ikr.shangyingyoupin.top

[S46] C++：函数模板
来源：http://fux.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ixd.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://qdh.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rck.hnqzz.top

[S48] C++：逐行读文件
来源：http://rad.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://nti.xuanzx.com

while (std::getline(in, line)) { }
来源：http://dar.hysaishi.cn

[S49] C++：写文件
来源：http://sxk.ehwqpu.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aiy.jinqigufen.top

[S50] C++：格式化数字
来源：http://ijz.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hyo.aibaodan.cn

[S51] C++：显式类型转换
来源：http://kry.sysykeji.top

static_cast<double>(a) / b
来源：http://upc.tanke756.top

[S52] C++：const 与 noexcept
来源：http://xyr.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://nby.fehbvm.com

[S53] C++：移动语义
来源：http://pzk.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://ycc.epnwcf.com

[S54] C++：异常处理
来源：http://xjo.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qla.gotoacloud.top

[S55] C++：结构化绑定
来源：http://vqu.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://atk.zhaomingkeji.xyz

[S56] C++：optional
来源：http://zhu.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ejb.zdbjq.cn

[S57] C++：编译期常量
来源：http://lvi.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://acl.xziqi.cn

[S58] C++：命名空间
来源：http://djc.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://zzr.zhiwuduotai.top

[S59] C++：静态断言
来源：http://kic.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://auz.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://qgn.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xvv.yonumen.top

================================================================================
来源：http://hen.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://owk.jiagoushi.top

================================================================================
来源：http://plw.sxryk.cn

[T01] Kotlin：Hello World
来源：http://ljg.yj20258.top

println("Hello")
来源：http://uyf.wangdashe.top

[T02] Kotlin：变量
来源：http://apy.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wso.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://fbp.ctjpmb.com

"值: $b"
来源：http://cef.fzhhl.top

[T04] Kotlin：空安全
来源：http://aee.aizwys.cn

val n: String? = null;  n?.length
来源：http://ipp.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://rrd.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sfi.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://jxm.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://kco.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://ujp.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://exi.hywenlv.cn

[T08] Kotlin：数据类
来源：http://hev.sweek.top

data class User(val name: String, val age: Int)
来源：http://jkg.ivvv.top

[T09] Kotlin：扩展函数
来源：http://cut.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://uum.vehdjk.com

[T10] Kotlin：默认参数
来源：http://lhu.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vzo.guannengcc.top

[T11] Kotlin：协程
来源：http://rty.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vcn.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://alg.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://eod.cheryme.top

[T13] Kotlin：只读 Map
来源：http://blg.ydzc1.top

val m = mapOf("a" to 1)
来源：http://ujy.hcnkem.com

[T14] Kotlin：循环
来源：http://fld.uphjek.com

for (i in 1..10) println(i)
来源：http://ste.yj202588.top

[T15] Kotlin：接口
来源：http://ubs.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://mnc.jyoumei.cn

[T16] Swift：Hello World
来源：http://bti.tarul.cn

print("Hello")
来源：http://ryf.andypj.xyz

[T17] Swift：变量与常量
来源：http://ncd.kuanghao11.cn

var a = 1;  let b = 2
来源：http://bky.yangfankeji.com

[T18] Swift：字符串插值
来源：http://cmd.yfazqb.com

"值: \(b)"
来源：http://yqm.havefunace.top

[T19] Swift：可选绑定
来源：http://dse.zdqjudy.top

if let n = opt { print(n) }
来源：http://bza.fktsv.cn

[T20] Swift：数组操作
来源：http://tqm.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://scb.jlsjyb.cn

[T21] Swift：遍历
来源：http://edl.ydjk.org.cn

for x in a { print(x) }
来源：http://xvh.bbcook.cn

[T22] Swift：字典
来源：http://bdk.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://jdk.ybcxt.top

[T23] Swift：函数
来源：http://fcv.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://anr.vqdsnc.cn

[T24] Swift：闭包
来源：http://lht.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zgr.yj202588.top

[T25] Swift：结构体
来源：http://czz.jyoumei.cn

struct P { var x: Int }
来源：http://egw.tarul.cn

[T26] Swift：类与重写
来源：http://gfz.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://fdu.fehbvm.com

[T27] Swift：错误处理
来源：http://lli.sysykeji.top

do { try f() } catch { print(error) }
来源：http://koa.vehdjk.com

[T28] Swift：枚举
来源：http://noy.hywenlv.cn

enum Color { case red, green }
来源：http://jza.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://dda.gogol.net.cn

guard let x = opt else { return }
来源：http://zrx.daxiang520.top

[T30] Swift：协议
来源：http://raw.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://hkj.hysaishi.cn

[T31] Lua：Hello World
来源：http://oky.hcnkem.com

print("Hello")
来源：http://wka.hfpthk.cn

[T32] Lua：局部变量
来源：http://euz.jiagoushi.top

local a = 1
来源：http://tog.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://izj.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kdh.yueranfly.top

[T34] Lua：遍历表
来源：http://zuo.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vae.shzxlz.cn

[T35] Lua：字典表
来源：http://rxf.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://ewq.yuxming.cn

[T36] Lua：函数
来源：http://bjd.ydjk.org.cn

function add(a, b) return a + b end
来源：http://cer.fengsongda.top

[T37] Lua：字符串拼接
来源：http://wah.yangfankeji.com

"a" .. "b"
来源：http://ryz.0kj1m.cn

[T38] Lua：条件
来源：http://uld.dianchejie.cn

if x > 0 then print("正") end
来源：http://bti.bjfxy.top

[T39] Lua：模式匹配
来源：http://bqp.yj20258888.top

string.find(s, "%d+")
来源：http://ldo.yj20258888.top

[T40] Lua：元表
来源：http://kyj.daxiang520.top

setmetatable({}, { __index = base })
来源：http://eln.yuxming.cn

[T41] Perl：Hello World
来源：http://pik.bbcook.cn

print "Hello\n";
来源：http://wdb.yj202588.top

[T42] Perl：变量类型
来源：http://bqf.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://khe.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://rnh.gogol.net.cn

"值: $a"
来源：http://ccf.dianchejie.cn

[T44] Perl：条件
来源：http://cyc.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://ctk.mhx1999.top

[T45] Perl：数组遍历
来源：http://uhf.fzhhl.top

for my $x (@arr) { print $x; }
来源：http://nkm.hnxiangtu.top

[T46] Perl：哈希操作
来源：http://dev.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eqq.hammf.cn

[T47] Perl：正则捕获
来源：http://bqd.haohaochexian.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rmr.gotoacloud.top

[T48] Perl：正则替换
来源：http://qha.xziqi.cn

$s =~ s/old/new/g;
来源：http://cyq.jiagoushi.top

[T49] Perl：函数
来源：http://qcp.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kvf.cqqwz.cn

[T50] Perl：逐行读文件
来源：http://dxo.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xov.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://tng.wangdashe.top

[T51] Scala：Hello World
来源：http://uel.jinqigfzy.top

println("Hello")
来源：http://vhl.jianghu66.top

[T52] Scala：变量
来源：http://kyc.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://nbu.xuanzx.com

[T53] Scala：字符串插值
来源：http://hsg.aizwys.cn

s"值: $b"
来源：http://akx.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://fqi.jianghu66.top

List(1, 2, 3).map(_ * 2)
来源：http://xye.0kj1m.cn

[T55] Scala：集合过滤
来源：http://rcc.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cqe.sweek.top

[T56] Scala：样例类
来源：http://kib.yj20258888.top

case class User(name: String, age: Int)
来源：http://mhu.zhixingplan.top

[T57] Scala：模式匹配
来源：http://ora.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vij.cucudq.cn

[T58] Scala：函数定义
来源：http://cbv.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://nag.zhixingplan.top

[T59] Scala：循环
来源：http://knw.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://yem.yanxiufei.cn

[T60] Scala：折叠
来源：http://jfp.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nae.zhijiandao.cn

================================================================================
来源：http://yeb.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://khr.hammf.cn

================================================================================
来源：http://tkg.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://btp.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tzr.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://yzg.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sbt.ivvv.top

[U03] Py：加载 .env 配置
来源：http://wpx.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dui.52xcode.cn

[U04] Py：变量调试打印
来源：http://rlp.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ikp.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://dto.fktsv.cn

list(dict.fromkeys(arr))
来源：http://ina.ivvv.top

[U06] Py：合并两个字典
来源：http://elz.nwbrower.top

{**a, **b}
来源：http://hzu.ppjwa.cn

[U07] Py：反转字典键值
来源：http://wfw.hammf.cn

{v: k for k, v in d.items()}
来源：http://zja.birdmap.top

[U08] Py：展平二维列表
来源：http://qrc.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://kca.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://miy.zhiwuduotai.top

max(d, key=d.get)
来源：http://xzc.hfpthk.cn

[U10] Py：按值排序字典
来源：http://gxj.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vof.chenzaomai.com

[U11] Py：生成器表达式
来源：http://jpf.nwbrower.top

(x * 2 for x in arr)
来源：http://bjb.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://awc.jyoumei.cn

Counter(arr).most_common(3)
来源：http://juf.ppjwa.cn

[U13] Py：固定长度队列
来源：http://yzt.zhongyouzk.top

deque(maxlen=10)
来源：http://afa.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://aif.haohaochexian.top

defaultdict(list)
来源：http://gdo.sweek.top

[U15] Py：高精度计时
来源：http://gec.vehdjk.com

t = time.perf_counter()
来源：http://dma.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://nyz.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fgz.gaohongyu789.top

[U17] Py：初始化日志
来源：http://izd.havefunace.top

logging.basicConfig(level=logging.INFO)
来源：http://bkz.smart0.xyz

[U18] Py：预编译正则
来源：http://vsj.shanyushiyangtech.top

pat = re.compile(r"\d+")
来源：http://wge.yuxming.cn


<!-- 参考信息 -->