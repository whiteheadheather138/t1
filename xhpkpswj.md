代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://enl.zycfv.cn

[R72] 等待端口就绪
来源：http://ukw.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://mfk.guowangkeji.top

[R73] 分割大日志
来源：http://eci.shanyushiyangtech.top

split -l 1000 big.log part_
来源：http://dit.andypj.xyz

[R74] 批量重命名
来源：http://kni.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bwi.shzxlz.cn

[R75] 导出环境变量
来源：http://vwh.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://rhv.guannengcc.top

[R76] 使用临时文件
来源：http://owu.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kcf.gotoacloud.top

[R77] 读取用户输入
来源：http://vnr.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://ugu.yuanzhike.top

[R78] 交互式菜单
来源：http://ybi.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://owg.jlsjyb.cn

[R79] 解析命令行选项
来源：http://cqm.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ays.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://gxt.epnwcf.com

time ./run.sh
来源：http://nfk.zhijiandao.cn

================================================================================
来源：http://bfu.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://shc.316326.xyz

================================================================================
来源：http://xwa.yj20258.top

[S01] C：Hello World
来源：http://ons.ydjk.org.cn

#include <stdio.h>
来源：http://yyv.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hfj.jinyuanbaomall.cn

[S02] C：变量与格式化输出
来源：http://elm.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://whp.yj20258.top

[S03] C：读入整数
来源：http://tae.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://iho.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://rmd.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://ali.ydzc1.top

[S05] C：字符串长度
来源：http://bzv.xuanzx.com

strlen(s)
来源：http://abm.meibo888.top

[S06] C：字符串比较
来源：http://xvv.hammf.cn

strcmp(a, b) == 0
来源：http://hgw.tian-w.cn

[S07] C：数组遍历求和
来源：http://sjv.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cyb.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://uij.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qoy.cashguo.top

[S09] C：结构体定义与初始化
来源：http://irn.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jxa.uphjek.com

[S10] C：指针与解引用
来源：http://rsm.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://whl.hywenlv.cn

[S11] C：逐行读文件
来源：http://yrk.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://gtj.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://unf.zhengqikj.top

fclose(f);
来源：http://ajy.chenzaomai.com

[S12] C：写文件
来源：http://jpz.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kak.ehwqpu.com

[S13] C：宏定义
来源：http://bac.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://imd.cqqwz.cn

[S14] C：枚举
来源：http://xei.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://obj.shzxlz.cn

[S15] C：类型转换
来源：http://pxh.52xcode.cn

(double) a / b
来源：http://and.yonumen.top

[S16] C：位操作置位
来源：http://akf.ybcxt.top

x |= (1 << 3);
来源：http://vcp.guannengcc.top

[S17] C：安全拼接字符串
来源：http://sgp.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dqb.aizwys.cn

[S18] C：命令行参数
来源：http://rpm.hysaishi.cn

int main(int argc, char **argv)
来源：http://hjd.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://elk.jianghu66.top

qsort(a, n, sizeof(int), cmp);
来源：http://ohi.hnxiangtu.top

[S20] C：二分查找
来源：http://jvu.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ycu.zhijiandao.cn

[S21] C：字符类别判断
来源：http://eab.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qaq.cqqwz.cn

[S22] C：字符串转数字
来源：http://lix.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ebi.xziqi.cn

[S23] C：随机数
来源：http://yfq.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://zdw.jianghu66.top

[S24] C：获取本地时间
来源：http://euv.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hdb.mhx1999.top

[S25] C：内存拷贝
来源：http://tca.sysykeji.top

memcpy(dst, src, n);
来源：http://onn.birdmap.top

[S26] C：内存清零
来源：http://dtf.sweek.top

memset(a, 0, sizeof a);
来源：http://nrd.hnqzz.top

[S27] C：定义常量
来源：http://whq.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://gst.fanxiaobao.xyz

[S28] C：静态变量
来源：http://wvt.jinghuilouyu.cn

static int counter = 0;
来源：http://jst.ydzc1.top

[S29] C：变参函数
来源：http://ovo.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mki.yueranfly.top

[S30] C：头文件保护
来源：http://nkz.guannengcc.top

#ifndef X_H
来源：http://kip.xuetiantiany.cn

#define X_H
来源：http://xey.zhaomingkeji.xyz

#endif
来源：http://xou.yfazqb.com

[S31] C++：Hello World
来源：http://xkm.yj202588.top

#include <iostream>
来源：http://pna.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://ozw.jlsjyb.cn

[S32] C++：字符串
来源：http://ybg.316326.xyz

std::string s = "hi";  s += "!";
来源：http://wpd.yj20258888.top

[S33] C++：vector 增删
来源：http://wts.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tfk.birdmap.top

[S34] C++：遍历 vector
来源：http://kdz.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://emd.dianchejie.cn

[S35] C++：map
来源：http://grw.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aas.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://syn.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mpf.shanyushiyangkeji.top

[S37] C++：set
来源：http://qlt.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mts.tarul.cn

[S38] C++：排序
来源：http://dks.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://chc.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://tuv.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pdn.yonumen.top

[S40] C++：查找元素
来源：http://kxj.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wcv.gotoacloud.top

[S41] C++：类与构造函数
来源：http://qfk.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://crz.sweek.top

[S42] C++：继承与虚函数
来源：http://xbt.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://dtl.tanke756.top

[S43] C++：智能指针
来源：http://kfx.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://hwb.svipenyu.cn

[S44] C++：引用传参
来源：http://ddj.cucudq.cn

void inc(int &x) { ++x; }
来源：http://ulr.dashuyun.cn

[S45] C++：lambda
来源：http://tpu.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jnm.fzhhl.top

[S46] C++：函数模板
来源：http://vnf.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xso.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://iuj.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jht.nwbrower.top

[S48] C++：逐行读文件
来源：http://zxx.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://srb.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://zcu.wangshuangyany.cn

[S49] C++：写文件
来源：http://bpt.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kit.ydjk.org.cn

[S50] C++：格式化数字
来源：http://auq.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xmz.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://sct.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://pzd.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://dtc.xuanzx.com

int size() const noexcept { return n_; }
来源：http://enr.hesvh.cn

[S53] C++：移动语义
来源：http://dco.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://nsk.dashuyun.cn

[S54] C++：异常处理
来源：http://vxr.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uxe.cashguo.top

[S55] C++：结构化绑定
来源：http://lrk.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://osl.jinqigfzy.top

[S56] C++：optional
来源：http://xpr.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lho.yueranfly.top

[S57] C++：编译期常量
来源：http://mdk.nanxinkj.top

constexpr int N = 10;
来源：http://rfy.hcnkem.com

[S58] C++：命名空间
来源：http://nvi.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://qbt.iojbl.cn

[S59] C++：静态断言
来源：http://xzp.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://khs.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://pah.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ocm.nanxinkj.top

================================================================================
来源：http://lty.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nvy.xuanzx.com

================================================================================
来源：http://vmw.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://rsj.haohaochexian.top

println("Hello")
来源：http://xer.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://hjh.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vwg.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://lay.sxryk.cn

"值: $b"
来源：http://rqd.yj20258888.top

[T04] Kotlin：空安全
来源：http://gki.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://xxz.uphjek.com

[T05] Kotlin：when 表达式
来源：http://aao.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xjo.yj20258888.top

[T06] Kotlin：集合映射
来源：http://eyn.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qel.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://bvy.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tdi.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://zoa.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://atx.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://sdg.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://owj.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://rch.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cxj.hysaishi.cn

[T11] Kotlin：协程
来源：http://yig.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yzs.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://lwt.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://uhr.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://eyb.smart0.xyz

val m = mapOf("a" to 1)
来源：http://xge.jianghu66.top

[T14] Kotlin：循环
来源：http://trk.iojbl.cn

for (i in 1..10) println(i)
来源：http://hgl.316326.xyz

[T15] Kotlin：接口
来源：http://ymd.fengsongda.top

interface Shape { fun area(): Double }
来源：http://yta.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://usq.ywan-chungtsiang.top

print("Hello")
来源：http://dhh.havefunace.top

[T17] Swift：变量与常量
来源：http://gkp.ivvv.top

var a = 1;  let b = 2
来源：http://hzw.c1oappe.top

[T18] Swift：字符串插值
来源：http://ckq.wangshuangyany.cn

"值: \(b)"
来源：http://whj.cqqwz.cn

[T19] Swift：可选绑定
来源：http://jvk.jyoumei.cn

if let n = opt { print(n) }
来源：http://cfe.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://ozz.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kyp.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://kyx.hcnkem.com

for x in a { print(x) }
来源：http://cwn.sxryk.cn

[T22] Swift：字典
来源：http://vcc.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://rri.sufxvd.cn

[T23] Swift：函数
来源：http://yzk.nanxinkj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dok.zdqjudy.top

[T24] Swift：闭包
来源：http://fyi.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://wrc.yongpay.top

[T25] Swift：结构体
来源：http://mon.cucudq.cn

struct P { var x: Int }
来源：http://hoo.0kj1m.cn

[T26] Swift：类与重写
来源：http://mvz.jiagoushi.top

class A: Base { override func f() {} }
来源：http://cud.yangfankeji.com

[T27] Swift：错误处理
来源：http://gtb.yj202588.top

do { try f() } catch { print(error) }
来源：http://pil.cashguo.top

[T28] Swift：枚举
来源：http://vta.nanxinkj.top

enum Color { case red, green }
来源：http://moe.cheryme.top

[T29] Swift：guard 提前返回
来源：http://ntk.chenjidiqi.icu

guard let x = opt else { return }
来源：http://gci.yj20258.top

[T30] Swift：协议
来源：http://tfq.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://cur.tian-w.cn

[T31] Lua：Hello World
来源：http://bha.havefunace.top

print("Hello")
来源：http://rhv.cashguo.top

[T32] Lua：局部变量
来源：http://zqg.ydjk.org.cn

local a = 1
来源：http://fsa.xylfe.cn

[T33] Lua：表（数组）
来源：http://eiy.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ovf.ybcxt.top

[T34] Lua：遍历表
来源：http://rmd.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xqb.dashuyun.cn

[T35] Lua：字典表
来源：http://tey.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://raq.jinghuilouyu.cn

[T36] Lua：函数
来源：http://utx.wangdashe.top

function add(a, b) return a + b end
来源：http://dsd.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://mzp.ydjk.org.cn

"a" .. "b"
来源：http://dca.jinqigfzy.top

[T38] Lua：条件
来源：http://cez.hammf.cn

if x > 0 then print("正") end
来源：http://xrl.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://xlc.tianlin.xyz

string.find(s, "%d+")
来源：http://kql.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://nem.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://ryu.zdqjudy.top

[T41] Perl：Hello World
来源：http://hqh.jqgfzy.top

print "Hello\n";
来源：http://cqr.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://kmj.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://olb.chenzaomai.com

[T43] Perl：字符串插值
来源：http://hiz.xuanzx.com

"值: $a"
来源：http://fsr.ydzc1.top

[T44] Perl：条件
来源：http://hvw.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://qao.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://zia.zdqjudy.top

for my $x (@arr) { print $x; }
来源：http://kue.bjfxy.top

[T46] Perl：哈希操作
来源：http://irm.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cml.yuanzhike.top

[T47] Perl：正则捕获
来源：http://xpu.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://csc.sxryk.cn

[T48] Perl：正则替换
来源：http://ufy.dashuyun.cn

$s =~ s/old/new/g;
来源：http://qxp.shuidangran.top

[T49] Perl：函数
来源：http://ttz.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://azt.pycfn.com

[T50] Perl：逐行读文件
来源：http://axd.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qkk.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://hvq.iojbl.cn

[T51] Scala：Hello World
来源：http://bcf.chenjidiqi.icu

println("Hello")
来源：http://ngj.ydzc1.top

[T52] Scala：变量
来源：http://jzq.nanxuanxn.top

val a = 1;  var b = 2
来源：http://vlw.yvedp.cn

[T53] Scala：字符串插值
来源：http://yqt.xylfe.cn

s"值: $b"
来源：http://hct.ppjwa.cn

[T54] Scala：集合映射
来源：http://yxj.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://tgc.yvedp.cn

[T55] Scala：集合过滤
来源：http://nxj.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://ook.tanke756.top

[T56] Scala：样例类
来源：http://klo.cdnleiting.top

case class User(name: String, age: Int)
来源：http://ahv.ivvv.top

[T57] Scala：模式匹配
来源：http://keh.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://wnj.fehbvm.com

[T58] Scala：函数定义
来源：http://loy.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://taa.vehdjk.com

[T59] Scala：循环
来源：http://hww.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://nuj.xuetiantiany.cn

[T60] Scala：折叠
来源：http://cxe.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rms.jinqigufen.top

================================================================================
来源：http://fgj.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mnf.dashuyun.cn

================================================================================
来源：http://ixv.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://yfr.zycfv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://har.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://voe.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fvs.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://cgm.tanke756.top

from dotenv import load_dotenv; load_dotenv()
来源：http://snt.jyoumei.cn

[U04] Py：变量调试打印
来源：http://lzq.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mov.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://cke.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://zyr.yj202588.top

[U06] Py：合并两个字典
来源：http://ucz.cqqwz.cn

{**a, **b}
来源：http://tmd.pycfn.com

[U07] Py：反转字典键值
来源：http://kqs.uphjek.com

{v: k for k, v in d.items()}
来源：http://ver.jyoumei.cn

[U08] Py：展平二维列表
来源：http://aoe.wangdashe.top

[y for x in nested for y in x]
来源：http://hjf.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://yin.c1oappe.top

max(d, key=d.get)
来源：http://vhj.ydzc1.top

[U10] Py：按值排序字典
来源：http://dwg.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iqb.jqgfzy.top

[U11] Py：生成器表达式
来源：http://scw.hcnkem.com

(x * 2 for x in arr)
来源：http://ayf.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://epi.jlsjyb.cn

Counter(arr).most_common(3)
来源：http://wmf.sweek.top


<!-- 参考信息 -->