代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://hpt.sysykeji.top

[R70] 时间戳与互转
来源：http://dwk.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://bti.yfazqb.com

[R71] 日期格式化
来源：http://ggo.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tca.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://gck.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://slr.yvedp.cn

[R73] 分割大日志
来源：http://ymx.sweek.top

split -l 1000 big.log part_
来源：http://mrc.jianghu66.top

[R74] 批量重命名
来源：http://omx.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lqb.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://yvj.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://rds.pycfn.com

[R76] 使用临时文件
来源：http://yol.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aqh.316326.xyz

[R77] 读取用户输入
来源：http://gdy.cashguo.top

read -rp "请输入: " ans
来源：http://roi.fengsongda.top

[R78] 交互式菜单
来源：http://cqt.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ecm.dashuyun.cn

[R79] 解析命令行选项
来源：http://dyr.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rai.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://vzv.zdqjudy.top

time ./run.sh
来源：http://vzq.hnxiangtu.top

================================================================================
来源：http://mos.daria6918.cn

S. C / C++ 专题
来源：http://jvs.dashuyun.cn

================================================================================
来源：http://vuw.zdbjq.cn

[S01] C：Hello World
来源：http://gxc.zhijiandao.cn

#include <stdio.h>
来源：http://cud.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nch.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://mgy.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://fcs.meibo888.top

[S03] C：读入整数
来源：http://qwc.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://pgd.xylfe.cn

[S04] C：字符串复制
来源：http://mck.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://frb.shangyingyoupin.top

[S05] C：字符串长度
来源：http://kkw.nanxuanxn.top

strlen(s)
来源：http://qfb.fehbvm.com

[S06] C：字符串比较
来源：http://tru.c1oappe.top

strcmp(a, b) == 0
来源：http://hin.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://wau.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kuj.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://hkx.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sfu.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://zxn.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hsj.zycfv.cn

[S10] C：指针与解引用
来源：http://zym.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://vts.ctjpmb.com

[S11] C：逐行读文件
来源：http://xfl.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://hxu.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qgv.nwbrower.top

fclose(f);
来源：http://bes.vehdjk.com

[S12] C：写文件
来源：http://fbc.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dkw.wangshuangyany.cn

[S13] C：宏定义
来源：http://tih.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xxt.9152youxi.cn

[S14] C：枚举
来源：http://tcu.smart0.xyz

enum Color { RED, GREEN, BLUE };
来源：http://zwp.hywenlv.cn

[S15] C：类型转换
来源：http://nbl.nwbrower.top

(double) a / b
来源：http://zbj.xuetiantiany.cn

[S16] C：位操作置位
来源：http://qwv.pengpengdd.cyou

x |= (1 << 3);
来源：http://oiz.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://tbg.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cea.hesvh.cn

[S18] C：命令行参数
来源：http://nqn.ivvv.top

int main(int argc, char **argv)
来源：http://cbf.svipenyu.cn

[S19] C：快速排序
来源：http://lgh.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://vxw.yfazqb.com

[S20] C：二分查找
来源：http://ufy.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yut.xinyue.icu

[S21] C：字符类别判断
来源：http://alr.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://frq.cashguo.top

[S22] C：字符串转数字
来源：http://ski.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://npp.dianchejie.cn

[S23] C：随机数
来源：http://rsx.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gzm.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://qkz.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zvl.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://adl.cheryme.top

memcpy(dst, src, n);
来源：http://pdu.hnxiangtu.top

[S26] C：内存清零
来源：http://cmv.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://swl.zdbjq.cn

[S27] C：定义常量
来源：http://kww.kuanghao11.cn

const double PI = 3.14159;
来源：http://juq.yonumen.top

[S28] C：静态变量
来源：http://hkf.52xcode.cn

static int counter = 0;
来源：http://oia.jiagoushi.top

[S29] C：变参函数
来源：http://phs.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xgb.aizwys.cn

[S30] C：头文件保护
来源：http://ehg.sxryk.cn

#ifndef X_H
来源：http://mmy.nanxinkj.top

#define X_H
来源：http://fnq.daria6918.cn

#endif
来源：http://qhe.cashguo.top

[S31] C++：Hello World
来源：http://ccl.havefunace.top

#include <iostream>
来源：http://ucb.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://wgr.mhx1999.top

[S32] C++：字符串
来源：http://bow.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://rrg.shuidangran.top

[S33] C++：vector 增删
来源：http://vla.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://anj.hywenlv.cn

[S34] C++：遍历 vector
来源：http://iuj.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://vad.52xcode.cn

[S35] C++：map
来源：http://vds.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bhc.ydjk.org.cn

[S36] C++：unordered_map
来源：http://gue.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lam.52xcode.cn

[S37] C++：set
来源：http://hvg.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ojt.guannengcc.top

[S38] C++：排序
来源：http://ixt.cheryme.top

std::sort(v.begin(), v.end());
来源：http://xjs.yj202588.top

[S39] C++：自定义比较器排序
来源：http://wau.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eor.bbcook.cn

[S40] C++：查找元素
来源：http://jbo.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zvb.jianghu66.top

[S41] C++：类与构造函数
来源：http://qho.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fcr.tarul.cn

[S42] C++：继承与虚函数
来源：http://rdz.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://yfp.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://gcl.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://vjf.xziqi.cn

[S44] C++：引用传参
来源：http://bvu.daria6918.cn

void inc(int &x) { ++x; }
来源：http://lkd.cashguo.top

[S45] C++：lambda
来源：http://cxh.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pql.bbcook.cn

[S46] C++：函数模板
来源：http://nyl.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fhv.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://plf.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xen.sufxvd.cn

[S48] C++：逐行读文件
来源：http://iri.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://lbg.yfazqb.com

while (std::getline(in, line)) { }
来源：http://kmk.nanxuanxn.top

[S49] C++：写文件
来源：http://jio.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ynn.fzhhl.top

[S50] C++：格式化数字
来源：http://wiv.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bgc.daxiang520.top

[S51] C++：显式类型转换
来源：http://umq.zhengqikj.top

static_cast<double>(a) / b
来源：http://yqd.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://vnl.iojbl.cn

int size() const noexcept { return n_; }
来源：http://xtr.cheryme.top

[S53] C++：移动语义
来源：http://jbr.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://kmo.snrcjt.cn

[S54] C++：异常处理
来源：http://aug.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jsg.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://gzg.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sdx.jqgufenzy.top

[S56] C++：optional
来源：http://gsx.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ppd.yvedp.cn

[S57] C++：编译期常量
来源：http://egv.jqgufenzy.top

constexpr int N = 10;
来源：http://leg.xylfe.cn

[S58] C++：命名空间
来源：http://ula.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://qcd.uphjek.com

[S59] C++：静态断言
来源：http://mws.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wyh.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://ref.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gls.havefunace.top

================================================================================
来源：http://ape.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ebk.sxryk.cn

================================================================================
来源：http://zxp.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://jmd.chenlongwang.top

println("Hello")
来源：http://ozi.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://wxn.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uqs.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://zhq.fzhhl.top

"值: $b"
来源：http://kjn.sufxvd.cn

[T04] Kotlin：空安全
来源：http://zoo.ppjwa.cn

val n: String? = null;  n?.length
来源：http://kuf.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://qam.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jyi.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://beq.svipenyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ick.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://sml.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://anl.andypj.xyz

[T08] Kotlin：数据类
来源：http://nji.bbcook.cn

data class User(val name: String, val age: Int)
来源：http://phj.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://rta.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://vbf.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://stj.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mqb.yanxiufei.cn

[T11] Kotlin：协程
来源：http://quv.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://han.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://ceo.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://wet.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://phy.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://qcd.tarul.cn

[T14] Kotlin：循环
来源：http://pte.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://sof.hcnkem.com

[T15] Kotlin：接口
来源：http://kaf.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://vkn.vqdsnc.cn

[T16] Swift：Hello World
来源：http://ktj.jinqigfzy.top

print("Hello")
来源：http://vbi.meibo888.top

[T17] Swift：变量与常量
来源：http://iid.hfpthk.cn

var a = 1;  let b = 2
来源：http://fcf.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://iws.xuanzx.com

"值: \(b)"
来源：http://aqc.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://unz.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://grv.yuanzhike.top

[T20] Swift：数组操作
来源：http://juo.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://iag.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://emt.chenjidiqi.icu

for x in a { print(x) }
来源：http://mtz.ctjpmb.com

[T22] Swift：字典
来源：http://qlu.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fuw.zycfv.cn

[T23] Swift：函数
来源：http://ccn.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yjv.aizwys.cn

[T24] Swift：闭包
来源：http://psw.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://apr.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://ibd.hongshengwenyu.top

struct P { var x: Int }
来源：http://dgv.nwbrower.top

[T26] Swift：类与重写
来源：http://yjy.smart0.xyz

class A: Base { override func f() {} }
来源：http://ner.gotoacloud.top

[T27] Swift：错误处理
来源：http://mhx.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://dcn.yvedp.cn

[T28] Swift：枚举
来源：http://vgm.dianchejie.cn

enum Color { case red, green }
来源：http://pef.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://jbt.fktsv.cn

guard let x = opt else { return }
来源：http://obg.kuanghao11.cn

[T30] Swift：协议
来源：http://oli.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://cap.nwbrower.top

[T31] Lua：Hello World
来源：http://qry.sxryk.cn

print("Hello")
来源：http://nmh.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://vsb.vehdjk.com

local a = 1
来源：http://epn.hcnkem.com

[T33] Lua：表（数组）
来源：http://zoc.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mhk.havefunace.top

[T34] Lua：遍历表
来源：http://bpr.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ivi.chenjidiqi.icu

[T35] Lua：字典表
来源：http://lkz.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://foi.jiagoushi.top

[T36] Lua：函数
来源：http://xvt.guannengcc.top

function add(a, b) return a + b end
来源：http://shc.sxryk.cn

[T37] Lua：字符串拼接
来源：http://jfd.svipenyu.cn

"a" .. "b"
来源：http://hbn.vqdsnc.cn

[T38] Lua：条件
来源：http://cof.shuidangran.top

if x > 0 then print("正") end
来源：http://mgz.yueranfly.top

[T39] Lua：模式匹配
来源：http://mao.redwolf501.top

string.find(s, "%d+")
来源：http://xoj.vqdsnc.cn

[T40] Lua：元表
来源：http://zlm.epnwcf.com

setmetatable({}, { __index = base })
来源：http://wdy.tianlin.xyz

[T41] Perl：Hello World
来源：http://rsz.ctjpmb.com

print "Hello\n";
来源：http://drd.fktsv.cn

[T42] Perl：变量类型
来源：http://bac.yj202588.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ewe.jianghu66.top

[T43] Perl：字符串插值
来源：http://lhe.hesvh.cn

"值: $a"
来源：http://euc.cucudq.cn

[T44] Perl：条件
来源：http://nqz.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://ioy.xinyue.icu

[T45] Perl：数组遍历
来源：http://haw.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://xlt.zhixingplan.top

[T46] Perl：哈希操作
来源：http://kcl.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://msv.guowangkeji.top

[T47] Perl：正则捕获
来源：http://uqs.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mmz.sysykeji.top

[T48] Perl：正则替换
来源：http://ihk.dianchejie.cn

$s =~ s/old/new/g;
来源：http://cgi.sxryk.cn

[T49] Perl：函数
来源：http://hxv.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vmp.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://clv.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://frm.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://jsg.yj202588.top

[T51] Scala：Hello World
来源：http://fxz.yj202588.top

println("Hello")
来源：http://woj.jyoumei.cn

[T52] Scala：变量
来源：http://fsm.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://xar.zhengqikj.top

[T53] Scala：字符串插值
来源：http://wxv.shanyushiyangkeji.top

s"值: $b"
来源：http://trh.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://uiv.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://own.yfazqb.com

[T55] Scala：集合过滤
来源：http://oqm.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://vhp.andypj.xyz

[T56] Scala：样例类
来源：http://upx.svipenyu.cn

case class User(name: String, age: Int)
来源：http://uzm.nanxinkj.top

[T57] Scala：模式匹配
来源：http://nyl.nanxinkj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tlx.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://gvz.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dxv.shuidangran.top

[T59] Scala：循环
来源：http://siq.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://wpp.aibaodan.cn

[T60] Scala：折叠
来源：http://ycf.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nkp.aizwys.cn

================================================================================
来源：http://pvs.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oog.sweek.top

================================================================================
来源：http://qcl.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://fnq.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://uco.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://yyx.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kqk.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://ccg.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ojs.wangdashe.top

[U04] Py：变量调试打印
来源：http://kyo.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wqy.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://kej.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://gzr.nwbrower.top

[U06] Py：合并两个字典
来源：http://iht.ydzc1.top

{**a, **b}
来源：http://ako.52xcode.cn

[U07] Py：反转字典键值
来源：http://mge.andypj.xyz

{v: k for k, v in d.items()}
来源：http://luq.zhijiandao.cn

[U08] Py：展平二维列表
来源：http://pjr.nanxuanxn.top

[y for x in nested for y in x]
来源：http://rlb.andypj.xyz

[U09] Py：字典取最大值的键
来源：http://jda.daria6918.cn

max(d, key=d.get)
来源：http://etl.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://hzb.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ogx.ppjwa.cn


<!-- 参考信息 -->